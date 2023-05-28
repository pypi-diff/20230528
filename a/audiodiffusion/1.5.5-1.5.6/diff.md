# Comparing `tmp/audiodiffusion-1.5.5.tar.gz` & `tmp/audiodiffusion-1.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audiodiffusion-1.5.5.tar", last modified: Tue May 23 13:40:14 2023, max compression
+gzip compressed data, was "audiodiffusion-1.5.6.tar", last modified: Sun May 28 16:02:21 2023, max compression
```

## Comparing `audiodiffusion-1.5.5.tar` & `audiodiffusion-1.5.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 teticio   (1000) teticio   (1000)        0 2023-05-23 13:40:14.824090 audiodiffusion-1.5.5/
--rw-rw-r--   0 teticio   (1000) teticio   (1000)    35149 2022-08-16 17:16:58.000000 audiodiffusion-1.5.5/LICENSE
--rw-rw-r--   0 teticio   (1000) teticio   (1000)    13485 2023-05-23 13:40:14.824090 audiodiffusion-1.5.5/PKG-INFO
--rw-rw-r--   0 teticio   (1000) teticio   (1000)    13229 2023-02-05 11:03:03.000000 audiodiffusion-1.5.5/README.md
-drwxrwxr-x   0 teticio   (1000) teticio   (1000)        0 2023-05-23 13:40:14.816090 audiodiffusion-1.5.5/audiodiffusion/
--rw-rw-r--   0 teticio   (1000) teticio   (1000)     5296 2023-05-23 13:39:29.000000 audiodiffusion-1.5.5/audiodiffusion/__init__.py
--rw-rw-r--   0 teticio   (1000) teticio   (1000)     3738 2023-05-23 13:33:43.000000 audiodiffusion-1.5.5/audiodiffusion/audio_encoder.py
--rw-rw-r--   0 teticio   (1000) teticio   (1000)     5680 2023-05-17 15:12:31.000000 audiodiffusion-1.5.5/audiodiffusion/mel.py
--rw-rw-r--   0 teticio   (1000) teticio   (1000)    10809 2023-04-22 08:29:21.000000 audiodiffusion-1.5.5/audiodiffusion/pipeline_audio_diffusion.py
--rw-rw-r--   0 teticio   (1000) teticio   (1000)    12150 2022-12-24 18:47:40.000000 audiodiffusion-1.5.5/audiodiffusion/utils.py
-drwxrwxr-x   0 teticio   (1000) teticio   (1000)        0 2023-05-23 13:40:14.820090 audiodiffusion-1.5.5/audiodiffusion.egg-info/
--rw-rw-r--   0 teticio   (1000) teticio   (1000)    13485 2023-05-23 13:40:14.000000 audiodiffusion-1.5.5/audiodiffusion.egg-info/PKG-INFO
--rw-rw-r--   0 teticio   (1000) teticio   (1000)      425 2023-05-23 13:40:14.000000 audiodiffusion-1.5.5/audiodiffusion.egg-info/SOURCES.txt
--rw-rw-r--   0 teticio   (1000) teticio   (1000)        1 2023-05-23 13:40:14.000000 audiodiffusion-1.5.5/audiodiffusion.egg-info/dependency_links.txt
--rw-rw-r--   0 teticio   (1000) teticio   (1000)        1 2022-12-02 17:31:12.000000 audiodiffusion-1.5.5/audiodiffusion.egg-info/not-zip-safe
--rw-rw-r--   0 teticio   (1000) teticio   (1000)       61 2023-05-23 13:40:14.000000 audiodiffusion-1.5.5/audiodiffusion.egg-info/requires.txt
--rw-rw-r--   0 teticio   (1000) teticio   (1000)       15 2023-05-23 13:40:14.000000 audiodiffusion-1.5.5/audiodiffusion.egg-info/top_level.txt
--rw-rw-r--   0 teticio   (1000) teticio   (1000)       57 2022-12-24 11:03:28.000000 audiodiffusion-1.5.5/pyproject.toml
--rw-rw-r--   0 teticio   (1000) teticio   (1000)      478 2023-05-23 13:40:14.824090 audiodiffusion-1.5.5/setup.cfg
--rw-rw-r--   0 teticio   (1000) teticio   (1000)       92 2022-08-28 13:28:51.000000 audiodiffusion-1.5.5/setup.py
+drwxrwxr-x   0 teticio   (1000) teticio   (1000)        0 2023-05-28 16:02:21.612927 audiodiffusion-1.5.6/
+-rw-rw-r--   0 teticio   (1000) teticio   (1000)    35149 2022-08-16 17:16:58.000000 audiodiffusion-1.5.6/LICENSE
+-rw-rw-r--   0 teticio   (1000) teticio   (1000)    13485 2023-05-28 16:02:21.612927 audiodiffusion-1.5.6/PKG-INFO
+-rw-rw-r--   0 teticio   (1000) teticio   (1000)    13229 2023-02-05 11:03:03.000000 audiodiffusion-1.5.6/README.md
+drwxrwxr-x   0 teticio   (1000) teticio   (1000)        0 2023-05-28 16:02:21.612927 audiodiffusion-1.5.6/audiodiffusion/
+-rw-rw-r--   0 teticio   (1000) teticio   (1000)     5296 2023-05-28 16:01:48.000000 audiodiffusion-1.5.6/audiodiffusion/__init__.py
+-rw-rw-r--   0 teticio   (1000) teticio   (1000)     3738 2023-05-23 13:33:43.000000 audiodiffusion-1.5.6/audiodiffusion/audio_encoder.py
+-rw-rw-r--   0 teticio   (1000) teticio   (1000)     5817 2023-05-28 16:01:32.000000 audiodiffusion-1.5.6/audiodiffusion/mel.py
+-rw-rw-r--   0 teticio   (1000) teticio   (1000)    10809 2023-04-22 08:29:21.000000 audiodiffusion-1.5.6/audiodiffusion/pipeline_audio_diffusion.py
+-rw-rw-r--   0 teticio   (1000) teticio   (1000)    12150 2022-12-24 18:47:40.000000 audiodiffusion-1.5.6/audiodiffusion/utils.py
+drwxrwxr-x   0 teticio   (1000) teticio   (1000)        0 2023-05-28 16:02:21.612927 audiodiffusion-1.5.6/audiodiffusion.egg-info/
+-rw-rw-r--   0 teticio   (1000) teticio   (1000)    13485 2023-05-28 16:02:21.000000 audiodiffusion-1.5.6/audiodiffusion.egg-info/PKG-INFO
+-rw-rw-r--   0 teticio   (1000) teticio   (1000)      425 2023-05-28 16:02:21.000000 audiodiffusion-1.5.6/audiodiffusion.egg-info/SOURCES.txt
+-rw-rw-r--   0 teticio   (1000) teticio   (1000)        1 2023-05-28 16:02:21.000000 audiodiffusion-1.5.6/audiodiffusion.egg-info/dependency_links.txt
+-rw-rw-r--   0 teticio   (1000) teticio   (1000)        1 2022-12-02 17:31:12.000000 audiodiffusion-1.5.6/audiodiffusion.egg-info/not-zip-safe
+-rw-rw-r--   0 teticio   (1000) teticio   (1000)       61 2023-05-28 16:02:21.000000 audiodiffusion-1.5.6/audiodiffusion.egg-info/requires.txt
+-rw-rw-r--   0 teticio   (1000) teticio   (1000)       15 2023-05-28 16:02:21.000000 audiodiffusion-1.5.6/audiodiffusion.egg-info/top_level.txt
+-rw-rw-r--   0 teticio   (1000) teticio   (1000)       57 2022-12-24 11:03:28.000000 audiodiffusion-1.5.6/pyproject.toml
+-rw-rw-r--   0 teticio   (1000) teticio   (1000)      478 2023-05-28 16:02:21.612927 audiodiffusion-1.5.6/setup.cfg
+-rw-rw-r--   0 teticio   (1000) teticio   (1000)       92 2022-08-28 13:28:51.000000 audiodiffusion-1.5.6/setup.py
```

### Comparing `audiodiffusion-1.5.5/LICENSE` & `audiodiffusion-1.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `audiodiffusion-1.5.5/PKG-INFO` & `audiodiffusion-1.5.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiodiffusion
-Version: 1.5.5
+Version: 1.5.6
 Summary: Generate Mel spectrogram dataset from directory of audio files.
 License: GPL3
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ---
```

### Comparing `audiodiffusion-1.5.5/README.md` & `audiodiffusion-1.5.6/README.md`

 * *Files identical despite different names*

### Comparing `audiodiffusion-1.5.5/audiodiffusion/__init__.py` & `audiodiffusion-1.5.6/audiodiffusion/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from librosa.beat import beat_track
 from PIL import Image
 from tqdm.auto import tqdm
 
 # from diffusers import AudioDiffusionPipeline
 from .pipeline_audio_diffusion import AudioDiffusionPipeline
 
-VERSION = "1.5.5"
+VERSION = "1.5.6"
 
 
 class AudioDiffusion:
     def __init__(
         self,
         model_id: str = "teticio/audio-diffusion-256",
         cuda: bool = torch.cuda.is_available(),
```

### Comparing `audiodiffusion-1.5.5/audiodiffusion/audio_encoder.py` & `audiodiffusion-1.5.6/audiodiffusion/audio_encoder.py`

 * *Files identical despite different names*

### Comparing `audiodiffusion-1.5.5/audiodiffusion/mel.py` & `audiodiffusion-1.5.6/audiodiffusion/mel.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
 import warnings
+from typing import Callable, Union
 
 from diffusers.configuration_utils import ConfigMixin, register_to_config
 from diffusers.schedulers.scheduling_utils import SchedulerMixin
 
 warnings.filterwarnings("ignore")
 
 import numpy as np  # noqa: E402
@@ -128,19 +129,20 @@
         """Get sample rate:
 
         Returns:
             `int`: sample rate of audio
         """
         return self.sr
 
-    def audio_slice_to_image(self, slice: int, ref=np.max) -> Image.Image:
+    def audio_slice_to_image(self, slice: int, ref: Union[float, Callable] = np.max) -> Image.Image:
         """Convert slice of audio to spectrogram.
 
         Args:
             slice (`int`): slice number of audio to convert (out of get_number_of_slices())
+            ref (`Union[float, Callable]`): reference value for spectrogram
 
         Returns:
             `PIL Image`: grayscale image of x_res x y_res
         """
         S = librosa.feature.melspectrogram(
             y=self.get_audio_slice(slice), sr=self.sr, n_fft=self.n_fft, hop_length=self.hop_length, n_mels=self.n_mels
         )
```

### Comparing `audiodiffusion-1.5.5/audiodiffusion/pipeline_audio_diffusion.py` & `audiodiffusion-1.5.6/audiodiffusion/pipeline_audio_diffusion.py`

 * *Files identical despite different names*

### Comparing `audiodiffusion-1.5.5/audiodiffusion/utils.py` & `audiodiffusion-1.5.6/audiodiffusion/utils.py`

 * *Files identical despite different names*

### Comparing `audiodiffusion-1.5.5/audiodiffusion.egg-info/PKG-INFO` & `audiodiffusion-1.5.6/audiodiffusion.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiodiffusion
-Version: 1.5.5
+Version: 1.5.6
 Summary: Generate Mel spectrogram dataset from directory of audio files.
 License: GPL3
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ---
```

