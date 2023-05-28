# Comparing `tmp/nlp-models-2.0.1.tar.gz` & `tmp/nlp-models-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nlp-models-2.0.1.tar", last modified: Fri May 26 14:52:52 2023, max compression
+gzip compressed data, was "nlp-models-2.1.0.tar", last modified: Sun May 28 20:27:34 2023, max compression
```

## Comparing `nlp-models-2.0.1.tar` & `nlp-models-2.1.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:52:52.185801 nlp-models-2.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-05-26 14:52:40.000000 nlp-models-2.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-05-26 14:52:52.185801 nlp-models-2.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-05-26 14:52:40.000000 nlp-models-2.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-26 14:52:40.000000 nlp-models-2.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-05-26 14:52:52.185801 nlp-models-2.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-26 14:52:40.000000 nlp-models-2.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:52:52.181801 nlp-models-2.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:52:52.185801 nlp-models-2.0.1/src/bert_classifier/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 14:52:40.000000 nlp-models-2.0.1/src/bert_classifier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-05-26 14:52:40.000000 nlp-models-2.0.1/src/bert_classifier/bert.py
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-05-26 14:52:40.000000 nlp-models-2.0.1/src/bert_classifier/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-05-26 14:52:40.000000 nlp-models-2.0.1/src/bert_classifier/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-05-26 14:52:40.000000 nlp-models-2.0.1/src/bert_classifier/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-05-26 14:52:40.000000 nlp-models-2.0.1/src/bert_classifier/predict.py
--rw-r--r--   0 runner    (1001) docker     (123)     3624 2023-05-26 14:52:40.000000 nlp-models-2.0.1/src/bert_classifier/train.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:52:52.185801 nlp-models-2.0.1/src/multi_task_model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 14:52:40.000000 nlp-models-2.0.1/src/multi_task_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-05-26 14:52:40.000000 nlp-models-2.0.1/src/multi_task_model/layers.py
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-26 14:52:40.000000 nlp-models-2.0.1/src/multi_task_model/loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-05-26 14:52:40.000000 nlp-models-2.0.1/src/multi_task_model/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-05-26 14:52:40.000000 nlp-models-2.0.1/src/multi_task_model/mtl.py
--rw-r--r--   0 runner    (1001) docker     (123)     9092 2023-05-26 14:52:40.000000 nlp-models-2.0.1/src/multi_task_model/trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-05-26 14:52:40.000000 nlp-models-2.0.1/src/multi_task_model/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:52:52.185801 nlp-models-2.0.1/src/nlp_models.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-05-26 14:52:52.000000 nlp-models-2.0.1/src/nlp_models.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-05-26 14:52:52.000000 nlp-models-2.0.1/src/nlp_models.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 14:52:52.000000 nlp-models-2.0.1/src/nlp_models.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-26 14:52:52.000000 nlp-models-2.0.1/src/nlp_models.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-26 14:52:52.000000 nlp-models-2.0.1/src/nlp_models.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 20:27:34.219632 nlp-models-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-05-28 20:27:19.000000 nlp-models-2.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-05-28 20:27:34.219632 nlp-models-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-05-28 20:27:19.000000 nlp-models-2.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-28 20:27:19.000000 nlp-models-2.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-05-28 20:27:34.219632 nlp-models-2.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-28 20:27:19.000000 nlp-models-2.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 20:27:34.215632 nlp-models-2.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 20:27:34.215632 nlp-models-2.1.0/src/bert_classifier/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 20:27:19.000000 nlp-models-2.1.0/src/bert_classifier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-05-28 20:27:19.000000 nlp-models-2.1.0/src/bert_classifier/bert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-05-28 20:27:19.000000 nlp-models-2.1.0/src/bert_classifier/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-05-28 20:27:20.000000 nlp-models-2.1.0/src/bert_classifier/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-05-28 20:27:20.000000 nlp-models-2.1.0/src/bert_classifier/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-05-28 20:27:20.000000 nlp-models-2.1.0/src/bert_classifier/predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3624 2023-05-28 20:27:20.000000 nlp-models-2.1.0/src/bert_classifier/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 20:27:34.219632 nlp-models-2.1.0/src/multi_task_model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 20:27:20.000000 nlp-models-2.1.0/src/multi_task_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-05-28 20:27:20.000000 nlp-models-2.1.0/src/multi_task_model/layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-28 20:27:20.000000 nlp-models-2.1.0/src/multi_task_model/loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-05-28 20:27:20.000000 nlp-models-2.1.0/src/multi_task_model/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-05-28 20:27:20.000000 nlp-models-2.1.0/src/multi_task_model/mtl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9589 2023-05-28 20:27:20.000000 nlp-models-2.1.0/src/multi_task_model/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-05-28 20:27:20.000000 nlp-models-2.1.0/src/multi_task_model/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 20:27:34.219632 nlp-models-2.1.0/src/nlp_models.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-05-28 20:27:34.000000 nlp-models-2.1.0/src/nlp_models.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-05-28 20:27:34.000000 nlp-models-2.1.0/src/nlp_models.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 20:27:34.000000 nlp-models-2.1.0/src/nlp_models.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-28 20:27:34.000000 nlp-models-2.1.0/src/nlp_models.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-28 20:27:34.000000 nlp-models-2.1.0/src/nlp_models.egg-info/top_level.txt
```

### Comparing `nlp-models-2.0.1/LICENSE` & `nlp-models-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nlp-models-2.0.1/PKG-INFO` & `nlp-models-2.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlp-models
-Version: 2.0.1
+Version: 2.1.0
 Summary: Transformers based NLP models
 Home-page: https://github.com/minggnim/nlp-models
 Author: Ming Gao
 Author-email: ming_gao@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `nlp-models-2.0.1/README.md` & `nlp-models-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `nlp-models-2.0.1/setup.cfg` & `nlp-models-2.1.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = nlp-models
-version = 2.0.1
+version = 2.1.0
 author = Ming Gao
 author_email = ming_gao@outlook.com
 url = https://github.com/minggnim/nlp-models
 description = Transformers based NLP models
 long_description = file: README.md
 long_description_content_type = text/markdown
 classifiers =
```

### Comparing `nlp-models-2.0.1/src/bert_classifier/bert.py` & `nlp-models-2.1.0/src/bert_classifier/bert.py`

 * *Files identical despite different names*

### Comparing `nlp-models-2.0.1/src/bert_classifier/data.py` & `nlp-models-2.1.0/src/bert_classifier/data.py`

 * *Files identical despite different names*

### Comparing `nlp-models-2.0.1/src/bert_classifier/io.py` & `nlp-models-2.1.0/src/bert_classifier/io.py`

 * *Files identical despite different names*

### Comparing `nlp-models-2.0.1/src/bert_classifier/metrics.py` & `nlp-models-2.1.0/src/bert_classifier/metrics.py`

 * *Files identical despite different names*

### Comparing `nlp-models-2.0.1/src/bert_classifier/predict.py` & `nlp-models-2.1.0/src/bert_classifier/predict.py`

 * *Files identical despite different names*

### Comparing `nlp-models-2.0.1/src/bert_classifier/train.py` & `nlp-models-2.1.0/src/bert_classifier/train.py`

 * *Files identical despite different names*

### Comparing `nlp-models-2.0.1/src/multi_task_model/layers.py` & `nlp-models-2.1.0/src/multi_task_model/layers.py`

 * *Files identical despite different names*

### Comparing `nlp-models-2.0.1/src/multi_task_model/metrics.py` & `nlp-models-2.1.0/src/multi_task_model/metrics.py`

 * *Files identical despite different names*

### Comparing `nlp-models-2.0.1/src/multi_task_model/mtl.py` & `nlp-models-2.1.0/src/multi_task_model/mtl.py`

 * *Files identical despite different names*

### Comparing `nlp-models-2.0.1/src/multi_task_model/trainer.py` & `nlp-models-2.1.0/src/multi_task_model/trainer.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,19 +37,22 @@
         self.model = model
         self.train_dataloader = train_dataloader
         self.test_dataloader = test_dataloader
         self.configs = configs
         self.metrics = metrics
         self.device = device
         self.chkpt_dir = chkpt_dir
-        self.set_optimizer()
+        self.set_params()
         self.train_logs = []
         self.val_logs = []
     
-    def set_optimizer(self):
+    def set_params(self):
+        '''
+        set parameters to optimize and schedule
+        '''
         if not self.configs.tune_base_model:
             for param in self.model.base_model.parameters():
                 param.requires_grad = False
 
         self.optimizer = self.get_optimizer(
             list(self.model.named_parameters()), 
             self.configs.optimizer_class, 
@@ -57,81 +60,38 @@
             self.configs.weight_decay)
         
         self.scheduler = self.get_scheduler(
             self.optimizer, 
             self.configs.scheduler, 
             self.configs.warmup_steps, 
             len(self.train_dataloader)*self.configs.epochs)
-
-    def logger(self, epoch, metrics, loss, mode):
-        log = {
-            f'epoch_{epoch-1}': {
-                'loss': loss,
-                'accuracy': metrics
-            }
-        }
-        if mode == 'train':
-            self.train_logs.append(log)
-        else:
-            self.val_logs.append(log)
-
-    def print_per_epoch(self, epoch):
-        print(f"\n\n{'-'*30}EPOCH {epoch}/{self.configs.epochs}{'-'*30}")
-        epoch -= 1 
-        train_loss = self.train_logs[epoch][f'epoch_{epoch}']['loss']
-        train_acc = self.train_logs[epoch][f'epoch_{epoch}']['accuracy']
-        val_loss = self.val_logs[epoch][f'epoch_{epoch}']['loss']
-        val_acc = self.val_logs[epoch][f'epoch_{epoch}']['accuracy']
-        print(f"Train -> LOSS: {train_loss} | ACCURACY: {train_acc}")
-        print(f"Validation -> LOSS: {val_loss} | ACCURACY: {val_acc}\n\n\n")
-
-    def save_checkpoint(self, epoch):
-        if not self.chkpt_dir.exists():
-            self.chkpt_dir.mkdir(parents=True)
-        epoch -= 1
-        chkpt_path = self.chkpt_dir / ('chkpt' + str(epoch) + '.pt')
-        torch.save({
-            'epoch': epoch,
-            'model_state_dict': self.model.state_dict(),
-            'optimizer_state_dict': self.optimizer.state_dict(),
-            'train_loss': self.train_logs[epoch][f'epoch_{epoch}']['loss'],
-            'val_loss': self.val_logs[epoch][f'epoch_{epoch}']['loss'],
-            'train_acc': self.train_logs[epoch][f'epoch_{epoch}']['accuracy'],
-            'val_acc': self.val_logs[epoch][f'epoch_{epoch}']['accuracy'],
-        }, chkpt_path)
-
-    def load_checkpoint(self, chkpt_dir):
-        chkpt = torch.load(chkpt_dir)
-        self.model.load_state_dict(chkpt['model_state_dict'])
-        self.optimizer.load_state_dict(chkpt['optimizer_state_dict'])
-        self.scheduler = self.get_scheduler(
-            self.optimizer, 
-            self.configs.scheduler, 
-            0, 
-            len(self.train_dataloader)*self.configs.epochs)
-
-    def clear(self):
-        gc.collect()
-        torch.cuda.empty_cache()
     
-    def fit(self):
+    def train(self):
         epochs = tqdm(range(1, self.configs.epochs+1), leave = True, desc="Training...")
         for epoch in epochs:
             self.model.train()
             epochs.set_description(f"EPOCH {epoch} / {self.configs.epochs} | training...")
             self.train_one_epoch(epoch)
             self.clear()
             
             self.model.eval()
             epochs.set_description(f"EPOCH {epoch} / {self.configs.epochs} | validating...")
             self.validate_one_epoch(epoch)
             self.clear()
                 
             self.print_per_epoch(epoch)
             self.save_checkpoint(epoch)
+            
+    def continue_training(self, chkpt_file):
+        '''
+        continue training from checkpoint
+        '''
+        self.model, self.optimizer, _ = self.load_checkpoint(chkpt_file, self.model, self.optimizer)
+        self.schedule_cold_start()
+        self.train()
 
     def train_one_epoch(self, epoch):
         batches = tqdm(self.train_dataloader, total=len(self.train_dataloader))
         total_train_loss = total_train_acc = 0
         for features, labels in batches:
             labels = labels.to(self.device)
             features = batch_to_device(features, self.device)
@@ -221,7 +181,63 @@
             return transformers.get_cosine_schedule_with_warmup(
                 optimizer, num_warmup_steps=warmup_steps, num_training_steps=t_total)
         elif scheduler == 'warmupcosinewithhardrestarts':
             return transformers.get_cosine_with_hard_restarts_schedule_with_warmup(
                 optimizer, num_warmup_steps=warmup_steps, num_training_steps=t_total)
         else:
             raise ValueError(f'Unkown scheduler {scheduler}')
+
+    @staticmethod
+    def load_checkpoint(chkpt_dir, model, optimizer: Optional=None):
+        chkpt = torch.load(chkpt_dir)
+        model.load_state_dict(chkpt['model_state_dict'])
+        if optimizer:
+            optimizer.load_state_dict(chkpt['optimizer_state_dict'])
+        return model, optimizer, chkpt
+    
+    def save_checkpoint(self, epoch):
+        if not self.chkpt_dir.exists():
+            self.chkpt_dir.mkdir(parents=True)
+        epoch -= 1
+        chkpt_path = self.chkpt_dir / ('chkpt' + str(epoch) + '.pt')
+        torch.save({
+            'epoch': epoch,
+            'model_state_dict': self.model.state_dict(),
+            'optimizer_state_dict': self.optimizer.state_dict(),
+            'train_loss': self.train_logs[epoch][f'epoch_{epoch}']['loss'],
+            'val_loss': self.val_logs[epoch][f'epoch_{epoch}']['loss'],
+            'train_acc': self.train_logs[epoch][f'epoch_{epoch}']['accuracy'],
+            'val_acc': self.val_logs[epoch][f'epoch_{epoch}']['accuracy'],
+        }, chkpt_path)
+        
+    def schedule_cold_start(self):
+        self.scheduler = self.get_scheduler(
+            self.optimizer, 
+            self.configs.scheduler, 
+            0, 
+            len(self.train_dataloader)*self.configs.epochs)
+
+    def print_per_epoch(self, epoch):
+        print(f"\n\n{'-'*30}EPOCH {epoch}/{self.configs.epochs}{'-'*30}")
+        epoch -= 1 
+        train_loss = self.train_logs[epoch][f'epoch_{epoch}']['loss']
+        train_acc = self.train_logs[epoch][f'epoch_{epoch}']['accuracy']
+        val_loss = self.val_logs[epoch][f'epoch_{epoch}']['loss']
+        val_acc = self.val_logs[epoch][f'epoch_{epoch}']['accuracy']
+        print(f"Train -> LOSS: {train_loss} | ACCURACY: {train_acc}")
+        print(f"Validation -> LOSS: {val_loss} | ACCURACY: {val_acc}\n\n\n")
+
+    def logger(self, epoch, metrics, loss, mode):
+        log = {
+            f'epoch_{epoch-1}': {
+                'loss': loss,
+                'accuracy': metrics
+            }
+        }
+        if mode == 'train':
+            self.train_logs.append(log)
+        else:
+            self.val_logs.append(log)
+
+    def clear(self):
+        gc.collect()
+        torch.cuda.empty_cache()
```

### Comparing `nlp-models-2.0.1/src/multi_task_model/utils.py` & `nlp-models-2.1.0/src/multi_task_model/utils.py`

 * *Files identical despite different names*

### Comparing `nlp-models-2.0.1/src/nlp_models.egg-info/PKG-INFO` & `nlp-models-2.1.0/src/nlp_models.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlp-models
-Version: 2.0.1
+Version: 2.1.0
 Summary: Transformers based NLP models
 Home-page: https://github.com/minggnim/nlp-models
 Author: Ming Gao
 Author-email: ming_gao@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `nlp-models-2.0.1/src/nlp_models.egg-info/SOURCES.txt` & `nlp-models-2.1.0/src/nlp_models.egg-info/SOURCES.txt`

 * *Files identical despite different names*

