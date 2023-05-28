# Comparing `tmp/draggan-1.0.7.tar.gz` & `tmp/draggan-1.1.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/media/exthdd/laizeqiang/lzq/projects/generated_model/DragGAN/dist/.tmp-4bgohtzq/draggan-1.0.7.tar", last modified: Fri May 26 01:22:27 2023, max compression
+gzip compressed data, was "/media/exthdd/laizeqiang/lzq/projects/generated_model/DragGAN/dist/.tmp-fxfe41i8/draggan-1.1.0b1.tar", last modified: Sun May 28 15:16:35 2023, max compression
```

## Comparing `draggan-1.0.7.tar` & `draggan-1.1.0b1.tar`

### file list

```diff
@@ -1,52 +1,36 @@
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-26 01:22:27.000000 draggan-1.0.7/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       51 2023-05-26 01:22:27.000000 draggan-1.0.7/PKG-INFO
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     5302 2023-05-25 15:13:46.000000 draggan-1.0.7/README.md
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-26 01:22:27.000000 draggan-1.0.7/draggan/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       42 2023-05-25 07:27:46.000000 draggan-1.0.7/draggan/__init__.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     7959 2023-05-25 07:39:21.000000 draggan-1.0.7/draggan/api.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      873 2023-05-25 08:31:09.000000 draggan-1.0.7/draggan/app.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-26 01:22:27.000000 draggan-1.0.7/draggan/stylegan2/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-25 06:58:32.000000 draggan-1.0.7/draggan/stylegan2/__init__.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     5029 2023-05-25 06:58:32.000000 draggan-1.0.7/draggan/stylegan2/inversion.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-26 01:22:27.000000 draggan-1.0.7/draggan/stylegan2/lpips/
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)      111 2023-05-25 06:58:32.000000 draggan-1.0.7/draggan/stylegan2/lpips/__init__.py
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     1618 2023-05-25 06:58:32.000000 draggan-1.0.7/draggan/stylegan2/lpips/base_model.py
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)    12782 2023-05-25 06:58:32.000000 draggan-1.0.7/draggan/stylegan2/lpips/dist_model.py
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     7482 2023-05-25 06:58:32.000000 draggan-1.0.7/draggan/stylegan2/lpips/networks_basic.py
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     6533 2023-05-25 06:58:32.000000 draggan-1.0.7/draggan/stylegan2/lpips/pretrained_networks.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     5699 2023-05-25 06:58:32.000000 draggan-1.0.7/draggan/stylegan2/lpips/util.py
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)    19612 2023-05-25 07:21:59.000000 draggan-1.0.7/draggan/stylegan2/model.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-26 01:22:27.000000 draggan-1.0.7/draggan/stylegan2/op/
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)      155 2023-05-25 07:09:27.000000 draggan-1.0.7/draggan/stylegan2/op/__init__.py
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     6626 2023-05-25 07:16:40.000000 draggan-1.0.7/draggan/stylegan2/op/conv2d_gradfix.py
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     4282 2023-05-26 01:18:57.000000 draggan-1.0.7/draggan/stylegan2/op/fused_act.py
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     1333 2023-05-25 06:58:33.000000 draggan-1.0.7/draggan/stylegan2/op/fused_bias_act.cpp
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     2828 2023-05-25 06:58:33.000000 draggan-1.0.7/draggan/stylegan2/op/fused_bias_act_kernel.cu
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     1343 2023-05-25 06:58:33.000000 draggan-1.0.7/draggan/stylegan2/op/upfirdn2d.cpp
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     6679 2023-05-26 01:19:03.000000 draggan-1.0.7/draggan/stylegan2/op/upfirdn2d.py
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)    12070 2023-05-25 06:58:33.000000 draggan-1.0.7/draggan/stylegan2/op/upfirdn2d_kernel.cu
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)    12874 2023-05-26 01:21:39.000000 draggan-1.0.7/draggan/web.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-26 01:22:27.000000 draggan-1.0.7/draggan.egg-info/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       51 2023-05-26 01:22:27.000000 draggan-1.0.7/draggan.egg-info/PKG-INFO
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     1217 2023-05-26 01:22:27.000000 draggan-1.0.7/draggan.egg-info/SOURCES.txt
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)        1 2023-05-26 01:22:27.000000 draggan-1.0.7/draggan.egg-info/dependency_links.txt
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      104 2023-05-26 01:22:27.000000 draggan-1.0.7/draggan.egg-info/requires.txt
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)        8 2023-05-26 01:22:27.000000 draggan-1.0.7/draggan.egg-info/top_level.txt
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       38 2023-05-26 01:22:27.000000 draggan-1.0.7/setup.cfg
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      616 2023-05-26 00:56:39.000000 draggan-1.0.7/setup.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-26 01:22:27.000000 draggan-1.0.7/stylegan2/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-20 10:47:42.000000 draggan-1.0.7/stylegan2/__init__.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     5029 2023-05-22 12:03:04.000000 draggan-1.0.7/stylegan2/inversion.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-26 01:22:27.000000 draggan-1.0.7/stylegan2/lpips/
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)      111 2023-05-22 12:03:04.000000 draggan-1.0.7/stylegan2/lpips/__init__.py
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     1618 2023-05-22 12:03:04.000000 draggan-1.0.7/stylegan2/lpips/base_model.py
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)    12782 2023-05-22 12:03:04.000000 draggan-1.0.7/stylegan2/lpips/dist_model.py
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     7482 2023-05-22 12:03:04.000000 draggan-1.0.7/stylegan2/lpips/networks_basic.py
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     6533 2023-05-22 12:03:04.000000 draggan-1.0.7/stylegan2/lpips/pretrained_networks.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     5699 2023-05-22 12:03:04.000000 draggan-1.0.7/stylegan2/lpips/util.py
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)    19630 2023-05-25 07:48:55.000000 draggan-1.0.7/stylegan2/model.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-26 01:22:27.000000 draggan-1.0.7/stylegan2/op/
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)      155 2023-05-25 14:03:01.000000 draggan-1.0.7/stylegan2/op/__init__.py
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     6626 2023-05-25 07:49:06.000000 draggan-1.0.7/stylegan2/op/conv2d_gradfix.py
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     4282 2023-05-26 01:19:24.000000 draggan-1.0.7/stylegan2/op/fused_act.py
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     6679 2023-05-26 01:19:32.000000 draggan-1.0.7/stylegan2/op/upfirdn2d.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-28 15:16:35.000000 draggan-1.1.0b1/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       53 2023-05-28 15:16:35.000000 draggan-1.1.0b1/PKG-INFO
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     5960 2023-05-28 15:08:51.000000 draggan-1.1.0b1/README.md
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-28 15:16:35.000000 draggan-1.1.0b1/draggan/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       44 2023-05-28 12:23:03.000000 draggan-1.1.0b1/draggan/__init__.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     7733 2023-05-28 13:06:42.000000 draggan-1.1.0b1/draggan/api.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-28 15:16:35.000000 draggan-1.1.0b1/draggan/stylegan2/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-25 06:58:32.000000 draggan-1.1.0b1/draggan/stylegan2/__init__.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     5029 2023-05-25 06:58:32.000000 draggan-1.1.0b1/draggan/stylegan2/inversion.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-28 15:16:35.000000 draggan-1.1.0b1/draggan/stylegan2/lpips/
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)      111 2023-05-25 06:58:32.000000 draggan-1.1.0b1/draggan/stylegan2/lpips/__init__.py
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     1618 2023-05-25 06:58:32.000000 draggan-1.1.0b1/draggan/stylegan2/lpips/base_model.py
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)    12782 2023-05-25 06:58:32.000000 draggan-1.1.0b1/draggan/stylegan2/lpips/dist_model.py
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     7482 2023-05-25 06:58:32.000000 draggan-1.1.0b1/draggan/stylegan2/lpips/networks_basic.py
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     6533 2023-05-25 06:58:32.000000 draggan-1.1.0b1/draggan/stylegan2/lpips/pretrained_networks.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     5699 2023-05-25 06:58:32.000000 draggan-1.1.0b1/draggan/stylegan2/lpips/util.py
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)    19711 2023-05-28 02:36:05.000000 draggan-1.1.0b1/draggan/stylegan2/model.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-28 15:16:35.000000 draggan-1.1.0b1/draggan/stylegan2/op/
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)      155 2023-05-25 07:09:27.000000 draggan-1.1.0b1/draggan/stylegan2/op/__init__.py
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     6626 2023-05-25 07:16:40.000000 draggan-1.1.0b1/draggan/stylegan2/op/conv2d_gradfix.py
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     4282 2023-05-26 01:18:57.000000 draggan-1.1.0b1/draggan/stylegan2/op/fused_act.py
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     1333 2023-05-25 06:58:33.000000 draggan-1.1.0b1/draggan/stylegan2/op/fused_bias_act.cpp
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     2828 2023-05-25 06:58:33.000000 draggan-1.1.0b1/draggan/stylegan2/op/fused_bias_act_kernel.cu
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     1343 2023-05-25 06:58:33.000000 draggan-1.1.0b1/draggan/stylegan2/op/upfirdn2d.cpp
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     6679 2023-05-26 01:19:03.000000 draggan-1.1.0b1/draggan/stylegan2/op/upfirdn2d.py
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)    12070 2023-05-25 06:58:33.000000 draggan-1.1.0b1/draggan/stylegan2/op/upfirdn2d_kernel.cu
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     7296 2023-05-28 14:55:40.000000 draggan-1.1.0b1/draggan/utils.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)    11723 2023-05-28 13:54:13.000000 draggan-1.1.0b1/draggan/web.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-28 15:16:35.000000 draggan-1.1.0b1/draggan.egg-info/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       53 2023-05-28 15:16:35.000000 draggan-1.1.0b1/draggan.egg-info/PKG-INFO
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      862 2023-05-28 15:16:35.000000 draggan-1.1.0b1/draggan.egg-info/SOURCES.txt
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)        1 2023-05-28 15:16:35.000000 draggan-1.1.0b1/draggan.egg-info/dependency_links.txt
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      104 2023-05-28 15:16:35.000000 draggan-1.1.0b1/draggan.egg-info/requires.txt
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)        8 2023-05-28 15:16:35.000000 draggan-1.1.0b1/draggan.egg-info/top_level.txt
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       38 2023-05-28 15:16:35.000000 draggan-1.1.0b1/setup.cfg
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      618 2023-05-28 15:16:28.000000 draggan-1.1.0b1/setup.py
```

### Comparing `draggan-1.0.7/README.md` & `draggan-1.1.0b1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,12 @@
 # DragGAN
 [![PyPI](https://img.shields.io/pypi/v/draggan)](https://pypi.org/project/draggan/) 
 
-:boom:  [`Colab Demo`](https://colab.research.google.com/github/Zeqiang-Lai/DragGAN/blob/master/colab.ipynb) | [`InternGPT Free Online Demo`](https://github.com/OpenGVLab/InternGPT)
+:boom:  [`Colab Demo`](https://colab.research.google.com/github/Zeqiang-Lai/DragGAN/blob/master/colab.ipynb) | [`InternGPT Free Online Demo`](https://github.com/OpenGVLab/InternGPT) | [`Local Deployment`](#running-locally)
 
-```bash
-pip install draggan
-```
 <!-- pip install draggan -i https://pypi.org/simple/ -->
 
 > **An out-of-box online demo is integrated in [InternGPT](https://github.com/OpenGVLab/InternGPT) - a super cool pointing-language-driven visual interactive system. Enjoy for free.:lollipop:**
 > 
 > Note for Colab, remember to select a GPU via `Runtime/Change runtime type` (`代码执行程序/更改运行时类型`).
 
 Implementation of [Drag Your GAN: Interactive Point-based Manipulation on the Generative Image Manifold](https://vcai.mpi-inf.mpg.de/projects/DragGAN/)
@@ -38,37 +35,36 @@
 
 - [2023/5/25] DragGAN is on PyPI, simple install via `pip install draggan`. Also addressed the common CUDA problems https://github.com/Zeqiang-Lai/DragGAN/issues/38  https://github.com/Zeqiang-Lai/DragGAN/issues/12
 - [2023/5/25] We now support StyleGAN2-ada with much higher quality and more types of images. Try it by selecting models started with "ada".
 - [2023/5/24] Custom Image with GAN inversion is supported, but it is possible that your custom images are distorted  due to the limitation of GAN inversion. Besides, it is also possible the manipulations fail due to the limitation of our implementation.
 
 :star2: **Changelog**
 
-- [ ] Tweak performance.
+- [x] Tweak performance.
 - [x] Improving installation experience, DragGAN is now on [PyPI](https://pypi.org/project/draggan).
-- [ ] Automatically determining the number of iterations.
+- [x] Automatically determining the number of iterations.
+- [ ] Allow to save video without point annotations, custom image size.
 - [x] Support StyleGAN2-ada.
 - [x] Integrate into [InternGPT](https://github.com/OpenGVLab/InternGPT)
 - [x] Custom Image with GAN inversion.
 - [x] Download generated image and generation trajectory.
 - [x] Controlling generation process with GUI.
 - [x] Automatically download stylegan2 checkpoint.
 - [x] Support movable region, multiple handle points.
 - [x] Gradio and Colab Demo.
 
 > This project is now a sub-project of [InternGPT](https://github.com/OpenGVLab/InternGPT) for interactive image editing. Future updates of more cool tools beyond DragGAN would be added in [InternGPT](https://github.com/OpenGVLab/InternGPT). 
 
 
-
-
-
-
 ## Running Locally
 
 ### With PyPI
 
+📑 [Step by Step Tutorial](https://zeqiang-lai.github.io/blog/en/posts/drag_gan/) | [中文部署教程](https://zeqiang-lai.github.io/blog/posts/ai/drag_gan/)
+
 We recommend to use Conda to install requirements.
 
 ```bash
 conda create -n draggan python=3.7
 conda activate draggan
 ```
 
@@ -76,14 +72,16 @@
 ```bash
 conda install pytorch torchvision torchaudio pytorch-cuda=11.7 -c pytorch -c nvidia 
 ```
 
 Install DragGAN
 ```bash
 pip install draggan
+# If you meet ERROR: Could not find a version that satisfies the requirement draggan (from versions: none), use
+pip install draggan -i https://pypi.org/simple/
 ```
 
 Launch the Gradio demo
 
 ```bash
 python -m draggan.web
 # running on cpu
@@ -124,16 +122,16 @@
     year={2023}
 }
 ```
 
 
 ## Acknowledgement
 
-[Official DragGAN](https://github.com/XingangPan/DragGAN) &ensp; [StyleGAN2](https://github.com/NVlabs/stylegan2)  &ensp; [StyleGAN2-pytorch](https://github.com/rosinality/stylegan2-pytorch)  &ensp; [StyleGAN2-Ada](https://github.com/NVlabs/stylegan2-ada-pytorch)
-
+[Official DragGAN](https://github.com/XingangPan/DragGAN) &ensp; [DragGAN-Streamlit](https://github.com/skimai/DragGAN) &ensp; [StyleGAN2](https://github.com/NVlabs/stylegan2)  &ensp; [StyleGAN2-pytorch](https://github.com/rosinality/stylegan2-pytorch)  &ensp; [StyleGAN2-Ada](https://github.com/NVlabs/stylegan2-ada-pytorch)   &ensp;  [StyleGAN-Human](https://github.com/stylegan-human/StyleGAN-Human) &ensp;  [Self-Distilled-StyleGAN](https://github.com/self-distilled-stylegan/self-distilled-internet-photos)
 
 Welcome to discuss with us and continuously improve the user experience of DragGAN.
 Reach us with this WeChat QR Code.
 
-<p align="left"><img width="300" alt="image" src="https://pjlab-gvm-data.oss-cn-shanghai.aliyuncs.com/papers/media/wechat_group.jpg"></p> 
+<p align="left"><img width="300" alt="image" src="https://github.com/Zeqiang-Lai/DragGAN/assets/26198430/cd6b1602-dc19-442f-9ced-a441d4c81aec"></p> 
+
```

### Comparing `draggan-1.0.7/draggan/api.py` & `draggan-1.1.0b1/draggan/api.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,47 +1,17 @@
 import copy
-import os
 import random
-import urllib.request
 
 import torch
 import torch.nn.functional as FF
 import torch.optim
-from torchvision import utils
-from tqdm import tqdm
 
+from . import utils
 from .stylegan2.model import Generator
 
-BASE_DIR = os.path.join(os.path.expanduser('~'), 'draggan', 'checkpoints')
-
-
-class DownloadProgressBar(tqdm):
-    def update_to(self, b=1, bsize=1, tsize=None):
-        if tsize is not None:
-            self.total = tsize
-        self.update(b * bsize - self.n)
-
-
-def get_path(base_path):
-    save_path = os.path.join(BASE_DIR, base_path)
-    if not os.path.exists(save_path):
-        url = f"https://huggingface.co/aaronb/StyleGAN2/resolve/main/{base_path}"
-        print(f'{base_path} not found')
-        print('Try to download from huggingface: ', url)
-        os.makedirs(os.path.dirname(save_path), exist_ok=True)
-        download_url(url, save_path)
-        print('Downloaded to ', save_path)
-    return save_path
-
-
-def download_url(url, output_path):
-    with DownloadProgressBar(unit='B', unit_scale=True,
-                             miniters=1, desc=url.split('/')[-1]) as t:
-        urllib.request.urlretrieve(url, filename=output_path, reporthook=t.update_to)
-
 
 class CustomGenerator(Generator):
     def prepare(
         self,
         styles,
         inject_index=None,
         truncation=1,
@@ -118,123 +88,155 @@
 def stylegan2(
     size=1024,
     channel_multiplier=2,
     latent=512,
     n_mlp=8,
     ckpt='stylegan2-ffhq-config-f.pt'
 ):
-    g_ema = CustomGenerator(size, latent, n_mlp, channel_multiplier=channel_multiplier)
-    checkpoint = torch.load(get_path(ckpt))
+    g_ema = CustomGenerator(size, latent, n_mlp, channel_multiplier=channel_multiplier, human='human' in ckpt)
+    checkpoint = torch.load(utils.get_path(ckpt))
     g_ema.load_state_dict(checkpoint["g_ema"], strict=False)
     g_ema.requires_grad_(False)
     g_ema.eval()
     return g_ema
 
 
-def bilinear_interpolate_torch(im, y, x):
-    """
-    im : B,C,H,W
-    y : 1,numPoints -- pixel location y float
-    x : 1,numPOints -- pixel location y float
-    """
-    device = im.device
-
-    x0 = torch.floor(x).long().to(device)
-    x1 = x0 + 1
-
-    y0 = torch.floor(y).long().to(device)
-    y1 = y0 + 1
-
-    wa = ((x1.float() - x) * (y1.float() - y)).to(device)
-    wb = ((x1.float() - x) * (y - y0.float())).to(device)
-    wc = ((x - x0.float()) * (y1.float() - y)).to(device)
-    wd = ((x - x0.float()) * (y - y0.float())).to(device)
-    # Instead of clamp
-    x1 = x1 - torch.floor(x1 / im.shape[3]).int().to(device)
-    y1 = y1 - torch.floor(y1 / im.shape[2]).int().to(device)
-    Ia = im[:, :, y0, x0]
-    Ib = im[:, :, y1, x0]
-    Ic = im[:, :, y0, x1]
-    Id = im[:, :, y1, x1]
-
-    return Ia * wa + Ib * wb + Ic * wc + Id * wd
-
-
-def drag_gan(g_ema, latent: torch.Tensor, noise, F, handle_points, target_points, mask, max_iters=1000):
+def drag_gan(
+    g_ema,
+    latent: torch.Tensor,
+    noise,
+    F,
+    handle_points,
+    target_points,
+    mask,
+    max_iters=1000,
+    r1=3,
+    r2=12,
+    lam=20,
+    d=2
+):
     handle_points0 = copy.deepcopy(handle_points)
-    n = len(handle_points)
-    r1, r2, lam, d = 3, 12, 20, 1
-
-    def neighbor(x, y, d):
-        points = []
-        for i in range(x - d, x + d):
-            for j in range(y - d, y + d):
-                points.append(torch.tensor([i, j]).float().cuda())
-        return points
+    handle_points = torch.stack(handle_points)
+    handle_points0 = torch.stack(handle_points0)
+    target_points = torch.stack(target_points)
 
     F0 = F.detach().clone()
+    device = latent.device
 
     latent_trainable = latent[:, :6, :].detach().clone().requires_grad_(True)
     latent_untrainable = latent[:, 6:, :].detach().clone().requires_grad_(False)
     optimizer = torch.optim.Adam([latent_trainable], lr=2e-3)
-    for iter in range(max_iters):
-        for s in range(1):
-            optimizer.zero_grad()
-            latent = torch.cat([latent_trainable, latent_untrainable], dim=1)
-            sample2, F2 = g_ema.generate(latent, noise)
+    for _ in range(max_iters):
+        if torch.allclose(handle_points, target_points, atol=d):
+            break
+
+        optimizer.zero_grad()
+        latent = torch.cat([latent_trainable, latent_untrainable], dim=1)
+        sample2, F2 = g_ema.generate(latent, noise)
 
-            # motion supervision
-            loss = 0
-            for i in range(n):
-                pi, ti = handle_points[i], target_points[i]
-                di = (ti - pi) / torch.sum((ti - pi)**2)
-
-                for qi in neighbor(int(pi[0]), int(pi[1]), r1):
-                    # f1 = F[..., int(qi[0]), int(qi[1])]
-                    # f2 = F2[..., int(qi[0] + di[0]), int(qi[1] + di[1])]
-                    f1 = bilinear_interpolate_torch(F2, qi[0], qi[1]).detach()
-                    f2 = bilinear_interpolate_torch(F2, qi[0] + di[0], qi[1] + di[1])
-                    loss += FF.l1_loss(f2, f1)
+        # motion supervision
+        loss = motion_supervison(handle_points, target_points, F2, r1, device)
 
-            if mask is not None:
-                loss += ((F2 - F0) * (1 - mask)).abs().mean() * lam
+        if mask is not None:
+            loss += ((F2 - F0) * (1 - mask)).abs().mean() * lam
 
-            loss.backward()
-            optimizer.step()
+        loss.backward()
+        optimizer.step()
 
-        # point tracking
         with torch.no_grad():
             sample2, F2 = g_ema.generate(latent, noise)
-            for i in range(n):
-                pi = handle_points0[i]
-                # f = F0[..., int(pi[0]), int(pi[1])]
-                f0 = bilinear_interpolate_torch(F0, pi[0], pi[1])
-                minv = 1e9
-                minx = 1e9
-                miny = 1e9
-                for qi in neighbor(int(handle_points[i][0]), int(handle_points[i][1]), r2):
-                    # f2 = F2[..., int(qi[0]), int(qi[1])]
-                    try:
-                        f2 = bilinear_interpolate_torch(F2, qi[0], qi[1])
-                    except:
-                        import ipdb
-                        ipdb.set_trace()
-                    v = torch.norm(f2 - f0, p=1)
-                    if v < minv:
-                        minv = v
-                        minx = int(qi[0])
-                        miny = int(qi[1])
-                handle_points[i][0] = minx
-                handle_points[i][1] = miny
+            handle_points = point_tracking(F2, F0, handle_points, handle_points0, r2, device)
 
         F = F2.detach().clone()
-        if iter % 1 == 0:
-            print(iter, loss.item(), handle_points, target_points)
-            # p = handle_points[0].int()
-            # sample2[0, :, p[0] - 5:p[0] + 5, p[1] - 5:p[1] + 5] = sample2[0, :, p[0] - 5:p[0] + 5, p[1] - 5:p[1] + 5] * 0
-            # t = target_points[0].int()
-            # sample2[0, :, t[0] - 5:t[0] + 5, t[1] - 5:t[1] + 5] = sample2[0, :, t[0] - 5:t[0] + 5, t[1] - 5:t[1] + 5] * 255
-
-            # sample2[0, :, 210, 134] = sample2[0, :, 210, 134] * 0
-            # utils.save_image(sample2, "test2.png", normalize=True, range=(-1, 1))
+        # if iter % 1 == 0:
+        #     print(iter, loss.item(), handle_points, target_points)
 
         yield sample2, latent, F2, handle_points
+
+
+def motion_supervison(handle_points, target_points, F2, r1, device):
+    loss = 0
+    n = len(handle_points)
+    for i in range(n):
+        target2handle = target_points[i] - handle_points[i]
+        d_i = target2handle / (torch.norm(target2handle) + 1e-7)
+        if torch.norm(d_i) > torch.norm(target2handle):
+            d_i = target2handle
+
+        mask = utils.create_circular_mask(
+            F2.shape[2], F2.shape[3], center=handle_points[i].tolist(), radius=r1
+        ).to(device)
+
+        coordinates = torch.nonzero(mask).float()  # shape [num_points, 2]
+
+        # Shift the coordinates in the direction d_i
+        shifted_coordinates = coordinates + d_i[None]
+
+        h, w = F2.shape[2], F2.shape[3]
+
+        # Extract features in the mask region and compute the loss
+        F_qi = F2[:, :, mask]  # shape: [C, H*W]
+
+        # Sample shifted patch from F
+        normalized_shifted_coordinates = shifted_coordinates.clone()
+        normalized_shifted_coordinates[:, 0] = (
+            2.0 * shifted_coordinates[:, 0] / (h - 1)
+        ) - 1  # for height
+        normalized_shifted_coordinates[:, 1] = (
+            2.0 * shifted_coordinates[:, 1] / (w - 1)
+        ) - 1  # for width
+        # Add extra dimensions for batch and channels (required by grid_sample)
+        normalized_shifted_coordinates = normalized_shifted_coordinates.unsqueeze(
+            0
+        ).unsqueeze(
+            0
+        )  # shape [1, 1, num_points, 2]
+        normalized_shifted_coordinates = normalized_shifted_coordinates.flip(
+            -1
+        )  # grid_sample expects [x, y] instead of [y, x]
+        normalized_shifted_coordinates = normalized_shifted_coordinates.clamp(-1, 1)
+
+        # Use grid_sample to interpolate the feature map F at the shifted patch coordinates
+        F_qi_plus_di = torch.nn.functional.grid_sample(
+            F2, normalized_shifted_coordinates, mode="bilinear", align_corners=True
+        )
+        # Output has shape [1, C, 1, num_points] so squeeze it
+        F_qi_plus_di = F_qi_plus_di.squeeze(2)  # shape [1, C, num_points]
+
+        loss += torch.nn.functional.l1_loss(F_qi.detach(), F_qi_plus_di)
+    return loss
+
+
+def point_tracking(
+    F: torch.Tensor,
+    F0: torch.Tensor,
+    handle_points: torch.Tensor,
+    handle_points0: torch.Tensor,
+    r2: int = 3,
+    device: torch.device = torch.device("cuda"),
+) -> torch.Tensor:
+
+    n = handle_points.shape[0]  # Number of handle points
+    new_handle_points = torch.zeros_like(handle_points)
+
+    for i in range(n):
+        # Compute the patch around the handle point
+        patch = utils.create_square_mask(
+            F.shape[2], F.shape[3], center=handle_points[i].tolist(), radius=r2
+        ).to(device)
+
+        # Find indices where the patch is True
+        patch_coordinates = torch.nonzero(patch)  # shape [num_points, 2]
+
+        # Extract features in the patch
+        F_qi = F[:, :, patch_coordinates[:, 0], patch_coordinates[:, 1]]
+        # Extract feature of the initial handle point
+        f_i = F0[:, :, handle_points0[i][0].long(), handle_points0[i][1].long()]
+
+        # Compute the L1 distance between the patch features and the initial handle point feature
+        distances = torch.norm(F_qi - f_i[:, :, None], p=1, dim=1)
+
+        # Find the new handle point as the one with minimum distance
+        min_index = torch.argmin(distances)
+        new_handle_points[i] = patch_coordinates[min_index]
+
+    return new_handle_points
```

### Comparing `draggan-1.0.7/draggan/stylegan2/inversion.py` & `draggan-1.1.0b1/draggan/stylegan2/inversion.py`

 * *Files identical despite different names*

### Comparing `draggan-1.0.7/draggan/stylegan2/lpips/base_model.py` & `draggan-1.1.0b1/draggan/stylegan2/lpips/base_model.py`

 * *Files identical despite different names*

### Comparing `draggan-1.0.7/draggan/stylegan2/lpips/dist_model.py` & `draggan-1.1.0b1/draggan/stylegan2/lpips/dist_model.py`

 * *Files identical despite different names*

### Comparing `draggan-1.0.7/draggan/stylegan2/lpips/networks_basic.py` & `draggan-1.1.0b1/draggan/stylegan2/lpips/networks_basic.py`

 * *Files identical despite different names*

### Comparing `draggan-1.0.7/draggan/stylegan2/lpips/pretrained_networks.py` & `draggan-1.1.0b1/draggan/stylegan2/lpips/pretrained_networks.py`

 * *Files identical despite different names*

### Comparing `draggan-1.0.7/draggan/stylegan2/lpips/util.py` & `draggan-1.1.0b1/draggan/stylegan2/lpips/util.py`

 * *Files identical despite different names*

### Comparing `draggan-1.0.7/draggan/stylegan2/model.py` & `draggan-1.1.0b1/draggan/stylegan2/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -328,18 +328,18 @@
             batch, _, height, width = image.shape
             noise = image.new_empty(batch, 1, height, width).normal_()
 
         return image + self.weight * noise
 
 
 class ConstantInput(nn.Module):
-    def __init__(self, channel, size=4):
+    def __init__(self, channel, size_in=4, size_out=4):
         super().__init__()
 
-        self.input = nn.Parameter(torch.randn(1, channel, size, size))
+        self.input = nn.Parameter(torch.randn(1, channel, size_in, size_out))
 
     def forward(self, input):
         batch = input.shape[0]
         out = self.input.repeat(batch, 1, 1, 1)
 
         return out
 
@@ -408,14 +408,15 @@
         self,
         size,
         style_dim,
         n_mlp,
         channel_multiplier=2,
         blur_kernel=[1, 3, 3, 1],
         lr_mlp=0.01,
+        human=False,
     ):
         super().__init__()
 
         self.size = size
 
         self.style_dim = style_dim
 
@@ -438,15 +439,15 @@
             64: 256 * channel_multiplier,
             128: 128 * channel_multiplier,
             256: 64 * channel_multiplier,
             512: 32 * channel_multiplier,
             1024: 16 * channel_multiplier,
         }
 
-        self.input = ConstantInput(self.channels[4])
+        self.input = ConstantInput(self.channels[4], size_in=4, size_out=4 if not human else 2)
         self.conv1 = StyledConv(
             self.channels[4], self.channels[4], 3, style_dim, blur_kernel=blur_kernel
         )
         self.to_rgb1 = ToRGB(self.channels[4], style_dim, upsample=False)
 
         self.log_size = int(math.log(size, 2))
         self.num_layers = (self.log_size - 2) * 2 + 1
@@ -456,15 +457,15 @@
         self.to_rgbs = nn.ModuleList()
         self.noises = nn.Module()
 
         in_channel = self.channels[4]
 
         for layer_idx in range(self.num_layers):
             res = (layer_idx + 5) // 2
-            shape = [1, 1, 2 ** res, 2 ** res]
+            shape = [1, 1, 2 ** res, 2 ** (res-int(human))]
             self.noises.register_buffer(f"noise_{layer_idx}", torch.randn(*shape))
 
         for i in range(3, self.log_size + 1):
             out_channel = self.channels[2 ** i]
 
             self.convs.append(
                 StyledConv(
```

### Comparing `draggan-1.0.7/draggan/stylegan2/op/conv2d_gradfix.py` & `draggan-1.1.0b1/draggan/stylegan2/op/conv2d_gradfix.py`

 * *Files identical despite different names*

### Comparing `draggan-1.0.7/draggan/stylegan2/op/fused_act.py` & `draggan-1.1.0b1/draggan/stylegan2/op/fused_act.py`

 * *Files identical despite different names*

### Comparing `draggan-1.0.7/draggan/stylegan2/op/fused_bias_act.cpp` & `draggan-1.1.0b1/draggan/stylegan2/op/fused_bias_act.cpp`

 * *Files identical despite different names*

### Comparing `draggan-1.0.7/draggan/stylegan2/op/fused_bias_act_kernel.cu` & `draggan-1.1.0b1/draggan/stylegan2/op/fused_bias_act_kernel.cu`

 * *Files identical despite different names*

### Comparing `draggan-1.0.7/draggan/stylegan2/op/upfirdn2d.cpp` & `draggan-1.1.0b1/draggan/stylegan2/op/upfirdn2d.cpp`

 * *Files identical despite different names*

### Comparing `draggan-1.0.7/draggan/stylegan2/op/upfirdn2d.py` & `draggan-1.1.0b1/draggan/stylegan2/op/upfirdn2d.py`

 * *Files identical despite different names*

### Comparing `draggan-1.0.7/draggan/stylegan2/op/upfirdn2d_kernel.cu` & `draggan-1.1.0b1/draggan/stylegan2/op/upfirdn2d_kernel.cu`

 * *Files identical despite different names*

### Comparing `draggan-1.0.7/draggan/web.py` & `draggan-1.1.0b1/draggan/web.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import numpy as np
 import imageio
 from PIL import Image
 import uuid
 
 from .api import drag_gan, stylegan2
 from .stylegan2.inversion import inverse_image
+from . import utils
 
 device = 'cuda'
 
 
 SIZE_TO_CLICK_SIZE = {
     1024: 8,
     512: 5,
@@ -25,56 +26,26 @@
     'stylegan2-horse-config-f.pt': 256,
     'ada/ffhq.pt': 1024,
     'ada/afhqcat.pt': 512,
     'ada/afhqdog.pt': 512,
     'ada/afhqwild.pt': 512,
     'ada/brecahad.pt': 512,
     'ada/metfaces.pt': 512,
+    'human/v2_512.pt': 512,
+    'human/v2_1024.pt': 1024,
+    'self_distill/bicycles_256.pt': 256,
+    'self_distill/dogs_1024.pt': 1024,
+    'self_distill/elephants_512.pt': 512,
+    'self_distill/giraffes_512.pt': 512,
+    'self_distill/horses_256.pt': 256,
+    'self_distill/lions_512.pt': 512,
+    'self_distill/parrots_512.pt': 512,
 }
 
-DEFAULT_CKPT = 'stylegan2-ffhq-config-f.pt'
-
-
-class grImage(gr.components.Image):
-    is_template = True
-
-    def preprocess(self, x):
-        if x is None:
-            return x
-        if self.tool == "sketch" and self.source in ["upload", "webcam"]:
-            decode_image = gr.processing_utils.decode_base64_to_image(x)
-            width, height = decode_image.size
-            mask = np.zeros((height, width, 4), dtype=np.uint8)
-            mask[..., -1] = 255
-            mask = self.postprocess(mask)
-            x = {'image': x, 'mask': mask}
-        return super().preprocess(x)
-
-
-class ImageMask(gr.components.Image):
-    """
-    Sets: source="canvas", tool="sketch"
-    """
-
-    is_template = True
-
-    def __init__(self, **kwargs):
-        super().__init__(source="upload", tool="sketch", interactive=True, **kwargs)
-
-    def preprocess(self, x):
-        if x is None:
-            return x
-        if self.tool == "sketch" and self.source in ["upload", "webcam"] and type(x) != dict:
-            decode_image = gr.processing_utils.decode_base64_to_image(x)
-            width, height = decode_image.size
-            mask = np.zeros((height, width, 4), dtype=np.uint8)
-            mask[..., -1] = 255
-            mask = self.postprocess(mask)
-            x = {'image': x, 'mask': mask}
-        return super().preprocess(x)
+DEFAULT_CKPT = 'self_distill/lions_512.pt'
 
 
 class ModelWrapper:
     def __init__(self, **kwargs):
         self.g_ema = stylegan2(**kwargs).to(device)
 
 
@@ -83,46 +54,40 @@
     arr = tensor.detach().cpu().numpy()
     arr = (arr - arr.min()) / (arr.max() - arr.min())
     arr = arr * 255
     return arr.astype('uint8')
 
 
 def add_points_to_image(image, points, size=5):
-    h, w, = image.shape[:2]
-
-    for x, y in points['target']:
-        image[max(0, x - size):min(x + size, h - 1), max(0, y - size):min(y + size, w), :] = [255, 0, 0]
-    for x, y in points['handle']:
-        image[max(0, x - size):min(x + size, h - 1), max(0, y - size):min(y + size, w), :] = [0, 0, 255]
-
+    image = utils.draw_handle_target_points(image, points['handle'], points['target'], size)
     return image
 
 
 def on_click(image, target_point, points, size, evt: gr.SelectData):
     if target_point:
         points['target'].append([evt.index[1], evt.index[0]])
         image = add_points_to_image(image, points, size=SIZE_TO_CLICK_SIZE[size])
-        return image, str(evt.index), not target_point
+        return image, not target_point
     points['handle'].append([evt.index[1], evt.index[0]])
     image = add_points_to_image(image, points, size=SIZE_TO_CLICK_SIZE[size])
-    return image, str(evt.index), not target_point
+    return image, not target_point
 
 
 def on_drag(model, points, max_iters, state, size, mask):
     if len(points['handle']) == 0:
         raise gr.Error('You must select at least one handle point and target point.')
     if len(points['handle']) != len(points['target']):
         raise gr.Error('You have uncompleted handle points, try to selct a target point or undo the handle point.')
     max_iters = int(max_iters)
     latent = state['latent']
     noise = state['noise']
     F = state['F']
 
-    handle_points = [torch.tensor(p).float() for p in points['handle']]
-    target_points = [torch.tensor(p).float() for p in points['target']]
+    handle_points = [torch.tensor(p, device=device).float() for p in points['handle']]
+    target_points = [torch.tensor(p, device=device).float() for p in points['target']]
 
     if mask.get('mask') is not None:
         mask = Image.fromarray(mask['mask']).convert('L')
         mask = np.array(mask) == 255
 
         mask = torch.from_numpy(mask).float().to(device)
         mask = mask.unsqueeze(0).unsqueeze(0)
@@ -135,36 +100,36 @@
                                                       max_iters=max_iters):
         image = to_image(sample2)
 
         state['F'] = F
         state['latent'] = latent
         state['sample'] = sample2
         points['handle'] = [p.cpu().numpy().astype('int') for p in handle_points]
-        add_points_to_image(image, points, size=SIZE_TO_CLICK_SIZE[size])
+        image = add_points_to_image(image, points, size=SIZE_TO_CLICK_SIZE[size])
 
         state['history'].append(image)
         step += 1
         yield image, state, step
 
 
 def on_reset(points, image, state):
-    return {'target': [], 'handle': []}, to_image(state['sample'])
+    return {'target': [], 'handle': []}, to_image(state['sample']), False
 
 
 def on_undo(points, image, state, size):
     image = to_image(state['sample'])
 
     if len(points['target']) < len(points['handle']):
         points['handle'] = points['handle'][:-1]
     else:
         points['handle'] = points['handle'][:-1]
         points['target'] = points['target'][:-1]
 
-    add_points_to_image(image, points, size=SIZE_TO_CLICK_SIZE[size])
-    return points, image
+    image = add_points_to_image(image, points, size=SIZE_TO_CLICK_SIZE[size])
+    return points, image, False
 
 
 def on_change_model(selected, model):
     size = CKPT_SIZE[selected]
     model = ModelWrapper(size=size, ckpt=selected)
     g_ema = model.g_ema
     sample_z = torch.randn([1, 512], device=device)
@@ -230,14 +195,19 @@
     return image, image, result, points, target_point
 
 
 def on_mask_change(mask):
     return mask['image']
 
 
+def on_select_mask_tab(state):
+    img = to_image(state['sample'])
+    return img
+
+
 def main():
     torch.cuda.manual_seed(25)
 
     with gr.Blocks() as demo:
         wrapped_model = ModelWrapper(ckpt=DEFAULT_CKPT, size=CKPT_SIZE[DEFAULT_CKPT])
         model = gr.State(wrapped_model)
         sample_z = torch.randn([1, 512], device=device)
@@ -281,28 +251,25 @@
             'noise': noise,
             'F': F,
             'sample': sample,
             'history': []
         })
         points = gr.State({'target': [], 'handle': []})
         size = gr.State(CKPT_SIZE[DEFAULT_CKPT])
+        target_point = gr.State(False)
 
         with gr.Row():
             with gr.Column(scale=0.3):
                 with gr.Accordion("Model"):
                     model_dropdown = gr.Dropdown(choices=list(CKPT_SIZE.keys()), value=DEFAULT_CKPT,
                                                  label='StyleGAN2 model')
                     max_iters = gr.Slider(1, 500, 20, step=1, label='Max Iterations')
                     new_btn = gr.Button('New Image')
                 with gr.Accordion('Drag'):
-                    with gr.Row():
-                        with gr.Column(min_width=100):
-                            text = gr.Textbox(label='Selected Point', interactive=False)
-                        with gr.Column(min_width=100):
-                            target_point = gr.Checkbox(label='Target Point', interactive=False)
+
                     with gr.Row():
                         with gr.Column(min_width=100):
                             reset_btn = gr.Button('Reset All')
                         with gr.Column(min_width=100):
                             undo_btn = gr.Button('Undo Last')
                     with gr.Row():
                         btn = gr.Button('Drag it', variant='primary')
@@ -310,31 +277,33 @@
                 with gr.Accordion('Save', visible=False) as save_panel:
                     files = gr.Files(value=[])
 
                 progress = gr.Slider(value=0, maximum=20, label='Progress', interactive=False)
 
             with gr.Column():
                 with gr.Tabs():
-                    with gr.Tab('Draw a Mask', id='mask'):
-                        mask = ImageMask(value=to_image(sample), label='Mask').style(height=768, width=768)
+                    img = to_image(sample)
                     with gr.Tab('Setup Handle Points', id='input'):
-                        image = grImage(to_image(sample)).style(height=768, width=768)
+                        image = gr.Image(img).style(height=512, width=512)
+                    with gr.Tab('Draw a Mask', id='mask') as masktab:
+                        mask = gr.ImageMask(img, label='Mask').style(height=512, width=512)
 
-        image.select(on_click, [image, target_point, points, size], [image, text, target_point])
+        image.select(on_click, [image, target_point, points, size], [image, target_point])
         image.upload(on_image_change, [model, size, image], [image, mask, state, points, target_point])
         mask.upload(on_mask_change, [mask], [image])
         btn.click(on_drag, inputs=[model, points, max_iters, state, size, mask], outputs=[image, state, progress]).then(
             on_show_save, outputs=save_panel).then(
             on_save_files, inputs=[image, state], outputs=[files]
         )
-        reset_btn.click(on_reset, inputs=[points, image, state], outputs=[points, image])
-        undo_btn.click(on_undo, inputs=[points, image, state, size], outputs=[points, image])
+        reset_btn.click(on_reset, inputs=[points, image, state], outputs=[points, image, target_point])
+        undo_btn.click(on_undo, inputs=[points, image, state, size], outputs=[points, image, target_point])
         model_dropdown.change(on_change_model, inputs=[model_dropdown, model], outputs=[model, state, image, mask, size])
         new_btn.click(on_new_image, inputs=[model], outputs=[image, mask, state, points, target_point])
         max_iters.change(on_max_iter_change, inputs=max_iters, outputs=progress)
+        masktab.select(lambda: gr.update(value=None), outputs=[mask]).then(on_select_mask_tab, inputs=[state], outputs=[mask])
     return demo
 
 
 if __name__ == '__main__':
     import argparse
     parser = argparse.ArgumentParser()
     parser.add_argument('--device', default='cuda')
```

### Comparing `draggan-1.0.7/draggan.egg-info/SOURCES.txt` & `draggan-1.1.0b1/draggan.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 README.md
 setup.py
 draggan/__init__.py
 draggan/api.py
-draggan/app.py
+draggan/utils.py
 draggan/web.py
 draggan.egg-info/PKG-INFO
 draggan.egg-info/SOURCES.txt
 draggan.egg-info/dependency_links.txt
 draggan.egg-info/requires.txt
 draggan.egg-info/top_level.txt
 draggan/stylegan2/__init__.py
@@ -21,21 +21,8 @@
 draggan/stylegan2/op/__init__.py
 draggan/stylegan2/op/conv2d_gradfix.py
 draggan/stylegan2/op/fused_act.py
 draggan/stylegan2/op/fused_bias_act.cpp
 draggan/stylegan2/op/fused_bias_act_kernel.cu
 draggan/stylegan2/op/upfirdn2d.cpp
 draggan/stylegan2/op/upfirdn2d.py
-draggan/stylegan2/op/upfirdn2d_kernel.cu
-stylegan2/__init__.py
-stylegan2/inversion.py
-stylegan2/model.py
-stylegan2/lpips/__init__.py
-stylegan2/lpips/base_model.py
-stylegan2/lpips/dist_model.py
-stylegan2/lpips/networks_basic.py
-stylegan2/lpips/pretrained_networks.py
-stylegan2/lpips/util.py
-stylegan2/op/__init__.py
-stylegan2/op/conv2d_gradfix.py
-stylegan2/op/fused_act.py
-stylegan2/op/upfirdn2d.py
+draggan/stylegan2/op/upfirdn2d_kernel.cu
```

### Comparing `draggan-1.0.7/setup.py` & `draggan-1.1.0b1/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
     name='draggan',
     packages=['draggan'],
-    version='1.0.7',
+    version='1.1.0b1',
     package_data={
         'draggan': ['stylegan2/op/fused_bias_act.cpp', 'stylegan2/op/upfirdn2d.cpp',
                     'stylegan2/op/fused_bias_act_kernel.cu', 'stylegan2/op/upfirdn2d_kernel.cu'], 
     },
     include_package_data=True,
     install_requires=[
         'gradio==3.28.1',
```

