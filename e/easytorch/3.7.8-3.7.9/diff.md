# Comparing `tmp/easytorch-3.7.8.tar.gz` & `tmp/easytorch-3.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easytorch-3.7.8.tar", last modified: Wed May 24 23:19:59 2023, max compression
+gzip compressed data, was "easytorch-3.7.9.tar", last modified: Sun May 28 01:34:24 2023, max compression
```

## Comparing `easytorch-3.7.8.tar` & `easytorch-3.7.9.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:19:59.446579 easytorch-3.7.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-24 23:19:48.000000 easytorch-3.7.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8267 2023-05-24 23:19:59.446579 easytorch-3.7.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7879 2023-05-24 23:19:48.000000 easytorch-3.7.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:19:59.442579 easytorch-3.7.8/easytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-24 23:19:48.000000 easytorch-3.7.8/easytorch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:19:59.442579 easytorch-3.7.8/easytorch/config/
--rw-r--r--   0 runner    (1001) docker     (123)     4424 2023-05-24 23:19:48.000000 easytorch-3.7.8/easytorch/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-05-24 23:19:48.000000 easytorch-3.7.8/easytorch/config/state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:19:59.446579 easytorch-3.7.8/easytorch/data/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-24 23:19:48.000000 easytorch-3.7.8/easytorch/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12992 2023-05-24 23:19:48.000000 easytorch-3.7.8/easytorch/data/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-05-24 23:19:48.000000 easytorch-3.7.8/easytorch/data/datautils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-05-24 23:19:48.000000 easytorch-3.7.8/easytorch/data/multiproc.py
--rw-r--r--   0 runner    (1001) docker     (123)    12745 2023-05-24 23:19:48.000000 easytorch-3.7.8/easytorch/easytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:19:59.446579 easytorch-3.7.8/easytorch/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-24 23:19:48.000000 easytorch-3.7.8/easytorch/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-05-24 23:19:48.000000 easytorch-3.7.8/easytorch/metrics/loss.py
--rw-r--r--   0 runner    (1001) docker     (123)    13674 2023-05-24 23:19:48.000000 easytorch-3.7.8/easytorch/metrics/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    19267 2023-05-24 23:19:48.000000 easytorch-3.7.8/easytorch/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:19:59.446579 easytorch-3.7.8/easytorch/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-05-24 23:19:48.000000 easytorch-3.7.8/easytorch/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-05-24 23:19:48.000000 easytorch-3.7.8/easytorch/utils/ddp_check.py
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-05-24 23:19:48.000000 easytorch-3.7.8/easytorch/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-05-24 23:19:48.000000 easytorch-3.7.8/easytorch/utils/tensorutils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:19:59.446579 easytorch-3.7.8/easytorch/vision/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-24 23:19:48.000000 easytorch-3.7.8/easytorch/vision/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9116 2023-05-24 23:19:48.000000 easytorch-3.7.8/easytorch/vision/imageutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-05-24 23:19:48.000000 easytorch-3.7.8/easytorch/vision/plotter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-05-24 23:19:48.000000 easytorch-3.7.8/easytorch/vision/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:19:59.442579 easytorch-3.7.8/easytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8267 2023-05-24 23:19:59.000000 easytorch-3.7.8/easytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-05-24 23:19:59.000000 easytorch-3.7.8/easytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 23:19:59.000000 easytorch-3.7.8/easytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-24 23:19:59.000000 easytorch-3.7.8/easytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-24 23:19:59.000000 easytorch-3.7.8/easytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 23:19:59.446579 easytorch-3.7.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-05-24 23:19:48.000000 easytorch-3.7.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 01:34:24.450652 easytorch-3.7.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-28 01:34:11.000000 easytorch-3.7.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8267 2023-05-28 01:34:24.450652 easytorch-3.7.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7879 2023-05-28 01:34:11.000000 easytorch-3.7.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 01:34:24.446653 easytorch-3.7.9/easytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-28 01:34:11.000000 easytorch-3.7.9/easytorch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 01:34:24.450652 easytorch-3.7.9/easytorch/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     4424 2023-05-28 01:34:11.000000 easytorch-3.7.9/easytorch/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-05-28 01:34:11.000000 easytorch-3.7.9/easytorch/config/state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 01:34:24.450652 easytorch-3.7.9/easytorch/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-28 01:34:11.000000 easytorch-3.7.9/easytorch/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12992 2023-05-28 01:34:11.000000 easytorch-3.7.9/easytorch/data/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-05-28 01:34:11.000000 easytorch-3.7.9/easytorch/data/datautils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-05-28 01:34:11.000000 easytorch-3.7.9/easytorch/data/multiproc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13268 2023-05-28 01:34:11.000000 easytorch-3.7.9/easytorch/easytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 01:34:24.450652 easytorch-3.7.9/easytorch/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-28 01:34:11.000000 easytorch-3.7.9/easytorch/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-05-28 01:34:11.000000 easytorch-3.7.9/easytorch/metrics/loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13674 2023-05-28 01:34:11.000000 easytorch-3.7.9/easytorch/metrics/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19093 2023-05-28 01:34:11.000000 easytorch-3.7.9/easytorch/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 01:34:24.450652 easytorch-3.7.9/easytorch/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-05-28 01:34:11.000000 easytorch-3.7.9/easytorch/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-05-28 01:34:11.000000 easytorch-3.7.9/easytorch/utils/ddp_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-05-28 01:34:11.000000 easytorch-3.7.9/easytorch/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-05-28 01:34:11.000000 easytorch-3.7.9/easytorch/utils/tensorutils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 01:34:24.450652 easytorch-3.7.9/easytorch/vision/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-28 01:34:11.000000 easytorch-3.7.9/easytorch/vision/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9116 2023-05-28 01:34:11.000000 easytorch-3.7.9/easytorch/vision/imageutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-05-28 01:34:11.000000 easytorch-3.7.9/easytorch/vision/plotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-05-28 01:34:11.000000 easytorch-3.7.9/easytorch/vision/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 01:34:24.446653 easytorch-3.7.9/easytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8267 2023-05-28 01:34:24.000000 easytorch-3.7.9/easytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-05-28 01:34:24.000000 easytorch-3.7.9/easytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 01:34:24.000000 easytorch-3.7.9/easytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-28 01:34:24.000000 easytorch-3.7.9/easytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-28 01:34:24.000000 easytorch-3.7.9/easytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-28 01:34:24.450652 easytorch-3.7.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-05-28 01:34:11.000000 easytorch-3.7.9/setup.py
```

### Comparing `easytorch-3.7.8/LICENSE` & `easytorch-3.7.9/LICENSE`

 * *Files identical despite different names*

### Comparing `easytorch-3.7.8/PKG-INFO` & `easytorch-3.7.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easytorch
-Version: 3.7.8
+Version: 3.7.9
 Summary: Easy Neural Network Experiments with pytorch
 Home-page: https://github.com/sraashis/easytorch
 Author: Aashis Khana1
 Author-email: sraashis@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `easytorch-3.7.8/README.md` & `easytorch-3.7.9/README.md`

 * *Files identical despite different names*

### Comparing `easytorch-3.7.8/easytorch/config/__init__.py` & `easytorch-3.7.9/easytorch/config/__init__.py`

 * *Files identical despite different names*

### Comparing `easytorch-3.7.8/easytorch/config/state.py` & `easytorch-3.7.9/easytorch/config/state.py`

 * *Files identical despite different names*

### Comparing `easytorch-3.7.8/easytorch/data/data.py` & `easytorch-3.7.9/easytorch/data/data.py`

 * *Files identical despite different names*

### Comparing `easytorch-3.7.8/easytorch/data/datautils.py` & `easytorch-3.7.9/easytorch/data/datautils.py`

 * *Files identical despite different names*

### Comparing `easytorch-3.7.8/easytorch/data/multiproc.py` & `easytorch-3.7.9/easytorch/data/multiproc.py`

 * *Files identical despite different names*

### Comparing `easytorch-3.7.8/easytorch/easytorch.py` & `easytorch-3.7.9/easytorch/easytorch.py`

 * *Files 5% similar despite different names*

```diff
@@ -84,19 +84,20 @@
 
         self.dataloader_args = dataloader_args
         assert (self.conf.get('phase') in self._MODES_), self._MODE_ERR_
 
         self._device_check()
         self._ddp_setup()
         self._make_reproducible()
-        self.conf.update(is_master=self.conf.get('is_master', True), world_rank=0)
-        self.conf['RUN-ID'] = _dtime.now().strftime("ET-%Y%m%d-%H%M%S-") + _uuid.uuid4().hex[:4].upper()
+        self.conf.update(is_master=self.conf.get('is_master', True))
+        self.conf['RUN-ID'] = _dtime.now().strftime("ET-%Y-%m-%d-%H%M%S-") + _uuid.uuid4().hex[:8].upper()
 
-        self.conf['save_dir'] = self.conf['output_base_dir'] + _sep + self.conf['phase'].upper() + _sep + self.conf[
-            "name"]
+        self.conf['save_dir'] = self.conf['output_base_dir'] + _sep + (
+                self.conf['phase'].upper() + _sep + self.conf["name"]
+        )
 
         """ No multi Loading in other than train mode """
         self.conf['multi_load'] = self.conf['multi_load'] and self.conf['phase'] == Phase.TRAIN
 
     def _device_check(self):
         self.conf['gpus'] = self.conf['gpus'] if self.conf.get('gpus') else []
         if self.conf['verbose'] and len(self.conf['gpus']) > NUM_GPUS:
@@ -184,15 +185,15 @@
         engine.init_nn()
 
     def _run_training_and_eval(self, data_split, engine, dataset_cls):
 
         train_loader = engine.data_handle.get_data_loader(
             handle_key='train',
             shuffle=True,
-            datset=engine.data_handle.get_dataset(Phase.TRAIN, data_split, dataset_cls),
+            dataset=engine.data_handle.get_dataset(Phase.TRAIN, data_split, dataset_cls),
             distributed=self.conf['use_ddp'])
 
         val_dataset = engine.data_handle.get_dataset(Phase.VALIDATION, data_split, dataset_cls)
         if val_dataset:
             val_loader = engine.data_handle.get_data_loader(
                 handle_key='validation',
                 shuffle=False,
@@ -226,34 +227,46 @@
 
         best_exists = _os.path.exists(engine.conf['save_dir'] + _sep + engine.cache['best_checkpoint'])
         if best_exists and (self.conf['phase'] == Phase.TRAIN or self.conf['pretrained_path'] is None):
             engine.load_checkpoint(engine.conf['save_dir'] + _sep + engine.cache['best_checkpoint'],
                                    map_location=engine.device['gpu'], load_optimizer_state=False)
 
         """ Run and save experiment test scores """
-        test_out = engine.evaluation(dataloader=dataloader, mode=Phase.TEST, save_predictions=True)
-        test_meter = engine.reduce_scores([test_out], distributed=False)
-        engine.cache[LogKey.TEST_METRICS] = [test_meter.get()]
+        engine.cache[
+            'output_csv_TEST'
+        ] = f"{engine.conf['save_dir']}{_sep}TEST_results_{engine.conf['RUN-ID']}.csv"
+        with open(engine.cache[f'output_csv_TEST'], 'w') as rw:
+            test_out = engine.evaluation(dataloader=dataloader, mode=Phase.TEST,
+                                         save_predictions=True, results_writer=rw)
+
+            test_meter = engine.reduce_scores([test_out], distributed=False)
+            engine.cache[LogKey.TEST_METRICS] = [test_meter.get()]
         _utils.save_scores(self.conf['save_dir'], engine.cache, name=engine.conf['name'],
                            file_keys=[LogKey.TEST_METRICS])
 
         if not engine.cache.get('_saved'):
             _utils.save_cache(self.conf, engine.cache, name=f"{engine.conf['name']}_test")
         return test_out
 
     def _inference(self, data_split, engine, dataset_cls):
         infer_dataset = engine.data_handle.get_dataset(Phase.INFERENCE, data_split, dataset_cls)
+
         dataloader = engine.data_handle.get_data_loader(
             handle_key=Phase.INFERENCE,
             shuffle=False,
             dataset=infer_dataset,
             distributed=self.conf['use_ddp'] and self.conf.get('distributed_inference'),
             use_unpadded_sampler=True,
         )
-        engine.inference(dataloader=dataloader)
+
+        engine.cache[
+            'output_csv_INFERENCE'
+        ] = f"{engine.conf['save_dir']}{_sep}INFERENCE_results_{engine.conf['RUN-ID']}.csv"
+        with open(engine.cache[f'output_csv_INFERENCE'], 'w') as rw:
+            engine.inference(dataloader=dataloader, results_writer=rw)
         _utils.save_cache(self.conf, engine.cache, name=f"{engine.conf['name']}_inference")
 
     def run(self, runner_cls: typing.Type[ETRunner],
             dataset_cls: typing.Type[ETDataset] = ETDataset,
             data_handle_cls: typing.Type[ETDataHandle] = ETDataHandle):
 
         if self.conf['is_master']:
```

### Comparing `easytorch-3.7.8/easytorch/metrics/loss.py` & `easytorch-3.7.9/easytorch/metrics/loss.py`

 * *Files identical despite different names*

### Comparing `easytorch-3.7.8/easytorch/metrics/metrics.py` & `easytorch-3.7.9/easytorch/metrics/metrics.py`

 * *Files identical despite different names*

### Comparing `easytorch-3.7.8/easytorch/runner.py` & `easytorch-3.7.9/easytorch/runner.py`

 * *Files 1% similar despite different names*

```diff
@@ -213,15 +213,16 @@
         return None
 
     @_torch.no_grad()
     def evaluation(self,
                    epoch=1,
                    mode='validation',
                    dataloader=None,
-                   save_predictions=False) -> _metrics.ETMeter:
+                   save_predictions=False,
+                   results_writer=None) -> _metrics.ETMeter:
         self.mode = mode
         for k in self.nn:
             self.nn[k].eval()
 
         eval_meter = self.new_meter()
         info(f'{mode} ...', self.conf['verbose'])
 
@@ -235,15 +236,15 @@
             try:
                 meter = self.new_meter()
                 for i, batch in enumerate(dataloader, 1):
                     self.batch_index = i
                     it = self.iteration(batch)
 
                     if save_predictions:
-                        _update_scores(self.save_predictions(dataloader.dataset, it), it, meter)
+                        _update_scores(self.save_predictions(dataloader.dataset, it, results_writer), it, meter)
                     else:
                         _update_scores(None, it, meter)
 
                     if self.conf['verbose'] and lazy_debug(i, add=epoch):
                         info(f"  Itr:{i}/{len(dataloader)}, {it['meter']}")
 
                 if self.conf['verbose']:
@@ -373,30 +374,26 @@
 
             if not self.conf['use_ddp']:
                 """Plot only in non-ddp mode to maintain consistency"""
                 self.cache[LogKey.TRAIN_LOG].append(running_meter.get())
 
             running_meter.reset()
 
-    def _inference_output_name():
-        return f"{self.conf['save_dir']}{_sep}INFERENCE_{self.conf['RUN-ID']}.csv"
     @_torch.no_grad()
-    def inference(self, dataloader):
+    def inference(self, dataloader, results_writer):
         self.mode = Phase.INFERENCE
 
         first_model = list(self.nn.keys())[0]
         self.nn[first_model].eval()
 
-        self.cache['output_csv'] = self._inference_output_name()
-        with open(self.cache['output_csv'], 'w') as fw:
-            for i, batch in enumerate(dataloader, 1):
-                self.batch_index = i
-                it = self.iteration(batch)
-                self.save_predictions(dataloader.dataset, it, writer=fw)
-                info(f"{self.conf['name']}, batch {i}/{len(dataloader)} done", self.conf['verbose'])
+        for i, batch in enumerate(dataloader, 1):
+            self.batch_index = i
+            it = self.iteration(batch)
+            self.save_predictions(dataloader.dataset, it, writer=results_writer)
+            info(f"{self.conf['name']}, batch {i}/{len(dataloader)} done", self.conf['verbose'])
 
         success(f"{self.conf['name']}, Inference results saved in:"
                 f"\n\t{self.cache['output_csv']}", self.conf['verbose'])
 
     def train(self, train_loader, validation_loader) -> None:
         ep = 0
         for ep in range(1, self.conf['epochs'] + 1):
```

### Comparing `easytorch-3.7.8/easytorch/utils/__init__.py` & `easytorch-3.7.9/easytorch/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `easytorch-3.7.8/easytorch/utils/ddp_check.py` & `easytorch-3.7.9/easytorch/utils/ddp_check.py`

 * *Files identical despite different names*

### Comparing `easytorch-3.7.8/easytorch/utils/tensorutils.py` & `easytorch-3.7.9/easytorch/utils/tensorutils.py`

 * *Files identical despite different names*

### Comparing `easytorch-3.7.8/easytorch/vision/imageutils.py` & `easytorch-3.7.9/easytorch/vision/imageutils.py`

 * *Files identical despite different names*

### Comparing `easytorch-3.7.8/easytorch/vision/plotter.py` & `easytorch-3.7.9/easytorch/vision/plotter.py`

 * *Files identical despite different names*

### Comparing `easytorch-3.7.8/easytorch/vision/transforms.py` & `easytorch-3.7.9/easytorch/vision/transforms.py`

 * *Files identical despite different names*

### Comparing `easytorch-3.7.8/easytorch.egg-info/PKG-INFO` & `easytorch-3.7.9/easytorch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easytorch
-Version: 3.7.8
+Version: 3.7.9
 Summary: Easy Neural Network Experiments with pytorch
 Home-page: https://github.com/sraashis/easytorch
 Author: Aashis Khana1
 Author-email: sraashis@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `easytorch-3.7.8/easytorch.egg-info/SOURCES.txt` & `easytorch-3.7.9/easytorch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `easytorch-3.7.8/setup.py` & `easytorch-3.7.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     import cv2
 except:
     _requires.append('opencv-contrib-python-headless')
 
 # This call to setup() does all the work
 setup(
     name="easytorch",
-    version="3.7.8",
+    version="3.7.9",
     description="Easy Neural Network Experiments with pytorch",
     long_description=_README,
     long_description_content_type="text/markdown",
     url="https://github.com/sraashis/easytorch",
     author="Aashis Khana1",
     author_email="sraashis@gmail.com",
     license="MIT",
```

