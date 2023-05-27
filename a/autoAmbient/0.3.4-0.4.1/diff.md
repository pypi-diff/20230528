# Comparing `tmp/autoAmbient-0.3.4.tar.gz` & `tmp/autoAmbient-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autoAmbient-0.3.4.tar", last modified: Sat May 27 21:54:42 2023, max compression
+gzip compressed data, was "autoAmbient-0.4.1.tar", last modified: Sat May 27 23:45:00 2023, max compression
```

## Comparing `autoAmbient-0.3.4.tar` & `autoAmbient-0.4.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 luis      (1000) luis      (1000)        0 2023-05-27 21:54:42.218104 autoAmbient-0.3.4/
--rw-rw-r--   0 luis      (1000) luis      (1000)     1087 2023-04-11 13:55:02.000000 autoAmbient-0.3.4/LICENSE
--rw-rw-r--   0 luis      (1000) luis      (1000)     3209 2023-05-27 21:54:42.218104 autoAmbient-0.3.4/PKG-INFO
--rw-rw-r--   0 luis      (1000) luis      (1000)     2324 2023-05-24 02:01:26.000000 autoAmbient-0.3.4/README.md
-drwxrwxr-x   0 luis      (1000) luis      (1000)        0 2023-05-27 21:54:42.214104 autoAmbient-0.3.4/ambient/
--rw-rw-r--   0 luis      (1000) luis      (1000)       73 2023-04-17 21:37:09.000000 autoAmbient-0.3.4/ambient/__init__.py
--rw-rw-r--   0 luis      (1000) luis      (1000)      897 2023-04-25 14:38:15.000000 autoAmbient-0.3.4/ambient/createAutoAmbient.py
--rw-rw-r--   0 luis      (1000) luis      (1000)      785 2023-04-25 15:08:35.000000 autoAmbient-0.3.4/ambient/createTagsFile.py
--rw-rw-r--   0 luis      (1000) luis      (1000)      721 2023-04-11 15:44:13.000000 autoAmbient-0.3.4/ambient/getFile.py
-drwxrwxr-x   0 luis      (1000) luis      (1000)        0 2023-05-27 21:54:42.214104 autoAmbient-0.3.4/ambient/models/
--rw-rw-r--   0 luis      (1000) luis      (1000)      165 2023-04-25 14:32:48.000000 autoAmbient-0.3.4/ambient/models/blocksModel.py
--rw-rw-r--   0 luis      (1000) luis      (1000)       47 2023-04-17 21:10:55.000000 autoAmbient-0.3.4/ambient/models/mainModel.py
--rw-rw-r--   0 luis      (1000) luis      (1000)      476 2023-04-25 14:56:13.000000 autoAmbient-0.3.4/ambient/models/runModel.py
-drwxrwxr-x   0 luis      (1000) luis      (1000)        0 2023-05-27 21:54:42.214104 autoAmbient-0.3.4/ambient/tolls/
--rw-rw-r--   0 luis      (1000) luis      (1000)     1892 2023-05-07 20:31:23.000000 autoAmbient-0.3.4/ambient/tolls/clicks.py
--rw-rw-r--   0 luis      (1000) luis      (1000)     4826 2023-04-17 22:02:18.000000 autoAmbient-0.3.4/ambient/tolls/gui.py
--rw-rw-r--   0 luis      (1000) luis      (1000)      822 2023-05-07 20:31:23.000000 autoAmbient-0.3.4/ambient/tolls/utils.py
-drwxrwxr-x   0 luis      (1000) luis      (1000)        0 2023-05-27 21:54:42.218104 autoAmbient-0.3.4/autoAmbient.egg-info/
--rw-rw-r--   0 luis      (1000) luis      (1000)     3209 2023-05-27 21:54:42.000000 autoAmbient-0.3.4/autoAmbient.egg-info/PKG-INFO
--rw-rw-r--   0 luis      (1000) luis      (1000)      510 2023-05-27 21:54:42.000000 autoAmbient-0.3.4/autoAmbient.egg-info/SOURCES.txt
--rw-rw-r--   0 luis      (1000) luis      (1000)        1 2023-05-27 21:54:42.000000 autoAmbient-0.3.4/autoAmbient.egg-info/dependency_links.txt
--rw-rw-r--   0 luis      (1000) luis      (1000)      142 2023-05-27 21:54:42.000000 autoAmbient-0.3.4/autoAmbient.egg-info/entry_points.txt
--rw-rw-r--   0 luis      (1000) luis      (1000)       94 2023-05-27 21:54:42.000000 autoAmbient-0.3.4/autoAmbient.egg-info/requires.txt
--rw-rw-r--   0 luis      (1000) luis      (1000)        8 2023-05-27 21:54:42.000000 autoAmbient-0.3.4/autoAmbient.egg-info/top_level.txt
--rw-rw-r--   0 luis      (1000) luis      (1000)        0 2023-04-11 14:47:07.000000 autoAmbient-0.3.4/pyproject.toml
--rw-rw-r--   0 luis      (1000) luis      (1000)      149 2023-05-27 21:54:42.218104 autoAmbient-0.3.4/setup.cfg
--rw-rw-r--   0 luis      (1000) luis      (1000)      921 2023-05-27 21:53:12.000000 autoAmbient-0.3.4/setup.py
+drwxrwxr-x   0 luis      (1000) luis      (1000)        0 2023-05-27 23:45:00.143622 autoAmbient-0.4.1/
+-rw-rw-r--   0 luis      (1000) luis      (1000)     1087 2023-04-11 13:55:02.000000 autoAmbient-0.4.1/LICENSE
+-rw-rw-r--   0 luis      (1000) luis      (1000)     4030 2023-05-27 23:45:00.143622 autoAmbient-0.4.1/PKG-INFO
+-rw-rw-r--   0 luis      (1000) luis      (1000)     3041 2023-05-27 23:23:13.000000 autoAmbient-0.4.1/README.md
+drwxrwxr-x   0 luis      (1000) luis      (1000)        0 2023-05-27 23:45:00.139622 autoAmbient-0.4.1/ambient/
+-rw-rw-r--   0 luis      (1000) luis      (1000)       73 2023-04-17 21:37:09.000000 autoAmbient-0.4.1/ambient/__init__.py
+-rw-rw-r--   0 luis      (1000) luis      (1000)      897 2023-04-25 14:38:15.000000 autoAmbient-0.4.1/ambient/createAutoAmbient.py
+-rw-rw-r--   0 luis      (1000) luis      (1000)      785 2023-04-25 15:08:35.000000 autoAmbient-0.4.1/ambient/createTagsFile.py
+-rw-rw-r--   0 luis      (1000) luis      (1000)      721 2023-04-11 15:44:13.000000 autoAmbient-0.4.1/ambient/getFile.py
+drwxrwxr-x   0 luis      (1000) luis      (1000)        0 2023-05-27 23:45:00.143622 autoAmbient-0.4.1/ambient/models/
+-rw-rw-r--   0 luis      (1000) luis      (1000)      146 2023-05-27 22:37:25.000000 autoAmbient-0.4.1/ambient/models/blocksModel.py
+-rw-rw-r--   0 luis      (1000) luis      (1000)       47 2023-04-17 21:10:55.000000 autoAmbient-0.4.1/ambient/models/mainModel.py
+-rw-rw-r--   0 luis      (1000) luis      (1000)      312 2023-05-27 23:17:15.000000 autoAmbient-0.4.1/ambient/models/runModel.py
+drwxrwxr-x   0 luis      (1000) luis      (1000)        0 2023-05-27 23:45:00.143622 autoAmbient-0.4.1/ambient/tolls/
+-rw-rw-r--   0 luis      (1000) luis      (1000)     2117 2023-05-27 22:11:56.000000 autoAmbient-0.4.1/ambient/tolls/clicks.py
+-rw-rw-r--   0 luis      (1000) luis      (1000)     4826 2023-04-17 22:02:18.000000 autoAmbient-0.4.1/ambient/tolls/gui.py
+-rw-rw-r--   0 luis      (1000) luis      (1000)     1113 2023-05-27 22:29:18.000000 autoAmbient-0.4.1/ambient/tolls/utils.py
+drwxrwxr-x   0 luis      (1000) luis      (1000)        0 2023-05-27 23:45:00.143622 autoAmbient-0.4.1/autoAmbient.egg-info/
+-rw-rw-r--   0 luis      (1000) luis      (1000)     4030 2023-05-27 23:45:00.000000 autoAmbient-0.4.1/autoAmbient.egg-info/PKG-INFO
+-rw-rw-r--   0 luis      (1000) luis      (1000)      510 2023-05-27 23:45:00.000000 autoAmbient-0.4.1/autoAmbient.egg-info/SOURCES.txt
+-rw-rw-r--   0 luis      (1000) luis      (1000)        1 2023-05-27 23:45:00.000000 autoAmbient-0.4.1/autoAmbient.egg-info/dependency_links.txt
+-rw-rw-r--   0 luis      (1000) luis      (1000)      142 2023-05-27 23:45:00.000000 autoAmbient-0.4.1/autoAmbient.egg-info/entry_points.txt
+-rw-rw-r--   0 luis      (1000) luis      (1000)       94 2023-05-27 23:45:00.000000 autoAmbient-0.4.1/autoAmbient.egg-info/requires.txt
+-rw-rw-r--   0 luis      (1000) luis      (1000)        8 2023-05-27 23:45:00.000000 autoAmbient-0.4.1/autoAmbient.egg-info/top_level.txt
+-rw-rw-r--   0 luis      (1000) luis      (1000)        0 2023-04-11 14:47:07.000000 autoAmbient-0.4.1/pyproject.toml
+-rw-rw-r--   0 luis      (1000) luis      (1000)      149 2023-05-27 23:45:00.143622 autoAmbient-0.4.1/setup.cfg
+-rw-rw-r--   0 luis      (1000) luis      (1000)      921 2023-05-27 23:43:29.000000 autoAmbient-0.4.1/setup.py
```

### Comparing `autoAmbient-0.3.4/LICENSE` & `autoAmbient-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `autoAmbient-0.3.4/README.md` & `autoAmbient-0.4.1/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -24,39 +24,52 @@
 ```bash
 createTagsFile
 ```
 
 Após a criação da referencia à imagem no arquivo de tags você deve escrever o seu fluxo em run.py como no exemplo a seguir:
 
 ```python
-from ambient.tolls.utils import take_click_types
-import tags as tg  # tags é um arquivo que contém referências a todas as imagens
-import ambient.tolls.clicks as cl
-from ambient.tolls.utils import remove_self_necessity
+from botcity.core import DesktopBot
+import tags as tg  # noqa: E261, F401
+import blocks as bls
+from ambient.tolls.utils import Nf
 
 
 def run():
     class Bot(DesktopBot):
         def action(self, execution=None):
-            nf = take_click_types(
-                tuple([remove_self_necessity(self, f) for f in cl.click_functions])
-            )
-            find, click, clickIfPossible = nf
-
+            nf = Nf(self)
             click(tg.btn_name) #o lugar que você que clicar
 
     Bot.main()
+
 ```
 
 Depois disso é só executar o main.py e ver a mágica acontecer
 
-O auto-enviroment conta com diversas maneiras de corrigir erros como as GUIs para quando a respectiva imagem não for encontrada
+## Funções
+
+As quatro funções disponíveis no arquivo `automations-enviroment/src/run.py` que são fornecidas pela classe `Nf` do módulo `ambient.tolls.utils` têm as seguintes funcionalidades:
+
+- `click(imgName, waiting_time)`: essa função faz um clique esquerdo do mouse na imagem com o nome fornecido.
+
+- `clickIfPossible(imgName, waiting_time)`: realiza a mesma operação do click, mas apenas se for possível, caso contrário, ele será ignorado e não emitira mensagem de erro.
+
+- `awaitItGoOut(imgName, waiting_time)`: essa função aguarda até que a imagem passada como parâmetro desapareça da tela.
+
+- `find(imgName, waiting_time, afterAction, notFoundAction)`: essa função busca pela imagem passada como parâmetro ,caso seja encontrado, executa o afterAction e, caso não, o notFoundAction.
+
+## Mensagens de erro
+
+O auto-enviroment conta com diversas maneiras de corrigir erros como as GUIs para quando a respectiva imagem não for encontrada.
 
 ![Captura de tela de 2023-05-23 22-57-20](https://github.com/luisArthurRodriguesDaSilva/auto-enviroment/assets/66787949/76c89f66-bcfa-432e-83c6-85bb2e56d766)
 
+Mais algumas dessas interfaces podem ser usadas importando `from ambient.tolls.gui import gui` como no exemplo a seguir.
+
 ## Contribuindo
 
 Se você quiser contribuir com a biblioteca AutoAmbient, você deve seguir as seguintes etapas:
 
 1. Fork o repositório
 2. Crie sua branch de features (`git checkout -b feature/fooBar`)
 3. Realize o commit de suas alterações (`git commit -am 'Add some fooBar'`)
```

### Comparing `autoAmbient-0.3.4/ambient/createAutoAmbient.py` & `autoAmbient-0.4.1/ambient/createAutoAmbient.py`

 * *Files identical despite different names*

### Comparing `autoAmbient-0.3.4/ambient/createTagsFile.py` & `autoAmbient-0.4.1/ambient/createTagsFile.py`

 * *Files identical despite different names*

### Comparing `autoAmbient-0.3.4/ambient/getFile.py` & `autoAmbient-0.4.1/ambient/getFile.py`

 * *Files identical despite different names*

### Comparing `autoAmbient-0.3.4/ambient/tolls/clicks.py` & `autoAmbient-0.4.1/ambient/tolls/clicks.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from . import gui
 import pyautogui
+import time
 from typing import Callable
 
 gui = gui.gui
 
 
 def alertImageNotFound(imgName):
     raise Exception(f"{imgName} não foi encontrado")
@@ -65,8 +66,16 @@
         btn,
         waiting_time=1000,
         afterAction=lambda: click(self, btn),
         notFoundAction=lambda imgName: print(imgName, "não achado mas segue o fluxo"),
     )
 
 
-click_functions = find, click, clickIfPossible
+def awaitItGoOut(self, imgName):
+    while 1:
+        print(f"esperando {imgName} sumir")
+        time.sleep(1)
+        if not self.find(imgName, matching=0.93, waiting_time=50):
+            break
+
+
+click_functions = find, click, clickIfPossible, awaitItGoOut
```

### Comparing `autoAmbient-0.3.4/ambient/tolls/gui.py` & `autoAmbient-0.4.1/ambient/tolls/gui.py`

 * *Files identical despite different names*

### Comparing `autoAmbient-0.3.4/setup.py` & `autoAmbient-0.4.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="autoAmbient",
-    version="0.3.4",
+    version="0.4.1",
     author="Luis Arthur Rodrigues da Silva",
     author_email="luisarthurlards03@gmail.com",
     packages=["ambient", "ambient.tolls", "ambient.models"],
     url="https://github.com/luisArthurRodriguesDaSilva/automations-enviroment",
     long_description=long_description,
     long_description_content_type="text/markdown",
     python_requires=">=3.8",
```

