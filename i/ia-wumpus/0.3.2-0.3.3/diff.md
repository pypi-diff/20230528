# Comparing `tmp/ia_wumpus-0.3.2.tar.gz` & `tmp/ia_wumpus-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ia_wumpus-0.3.2.tar", max compression
+gzip compressed data, was "ia_wumpus-0.3.3.tar", max compression
```

## Comparing `ia_wumpus-0.3.2.tar` & `ia_wumpus-0.3.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1071 2023-05-06 13:51:13.656383 ia_wumpus-0.3.2/LICENSE
--rw-r--r--   0        0        0     3921 2023-05-18 15:05:34.982478 ia_wumpus-0.3.2/README.md
--rw-r--r--   0        0        0      636 2023-05-27 22:33:07.393251 ia_wumpus-0.3.2/ia_wumpus/__init__.py
--rw-r--r--   0        0        0     6276 2023-05-27 19:32:15.239720 ia_wumpus-0.3.2/ia_wumpus/agente_reativo_v1.py
--rw-r--r--   0        0        0     7406 2023-05-27 17:56:52.970762 ia_wumpus-0.3.2/ia_wumpus/ambiente.py
--rw-r--r--   0        0        0     1355 2023-05-27 02:48:23.434838 ia_wumpus-0.3.2/ia_wumpus/dinamica_agente_ambiente.py
--rw-r--r--   0        0        0      476 2023-05-27 22:33:13.597239 ia_wumpus-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     4497 1970-01-01 00:00:00.000000 ia_wumpus-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-05-06 13:51:13.656383 ia_wumpus-0.3.3/LICENSE
+-rw-r--r--   0        0        0     3921 2023-05-18 15:05:34.982478 ia_wumpus-0.3.3/README.md
+-rw-r--r--   0        0        0      636 2023-05-28 14:43:13.018218 ia_wumpus-0.3.3/ia_wumpus/__init__.py
+-rw-r--r--   0        0        0     6333 2023-05-28 14:25:17.908004 ia_wumpus-0.3.3/ia_wumpus/agente_reativo_v1.py
+-rw-r--r--   0        0        0     7596 2023-05-28 14:15:51.000747 ia_wumpus-0.3.3/ia_wumpus/ambiente.py
+-rw-r--r--   0        0        0     1355 2023-05-27 02:48:23.434838 ia_wumpus-0.3.3/ia_wumpus/dinamica_agente_ambiente.py
+-rw-r--r--   0        0        0      476 2023-05-28 14:43:06.446101 ia_wumpus-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0     4497 1970-01-01 00:00:00.000000 ia_wumpus-0.3.3/PKG-INFO
```

### Comparing `ia_wumpus-0.3.2/LICENSE` & `ia_wumpus-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ia_wumpus-0.3.2/README.md` & `ia_wumpus-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `ia_wumpus-0.3.2/ia_wumpus/__init__.py` & `ia_wumpus-0.3.3/ia_wumpus/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -15,8 +15,8 @@
 # Data: Maio - 2023
 #  ----------------------------------------------------
 
 from .ambiente import Ambiente                   # noqa: F401
 from .agente_reativo_v1 import AgenteReativoV1   # noqa: F401
 
 
-__version__ = "0.3.2"
+__version__ = "0.3.3"
```

### Comparing `ia_wumpus-0.3.2/ia_wumpus/agente_reativo_v1.py` & `ia_wumpus-0.3.3/ia_wumpus/agente_reativo_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,38 +28,39 @@
         self.pegou_ouro: bool = False
         self.vitoria: bool = False
         self.morreu: bool = False
 
     def get_opcoes_mov(self) -> List:
         pos_agente = self.amb.get_pos_objetos()["agente"][0]
         self.__opcoes_mov_agente(pos_agente=pos_agente)
+        print("Opçoes andar: ", self.__list_opc_mov_ag)
         return self.__list_opc_mov_ag
 
     def __opcoes_mov_agente(self, pos_agente: Tuple) -> None:
         """
             Verifica as possíveis opções de movimentação do agente
             para a posição atual.
         """
         self.__list_opc_mov_ag = []
         dimensao_amb = self.amb.dimensoes[0]
         if pos_agente[0] == 0:
-            self.__list_opc_mov_ag.append((pos_agente[1], pos_agente[0] + 1))
+            self.__list_opc_mov_ag.append((pos_agente[0] + 1, pos_agente[1]))
         elif pos_agente[0] == (dimensao_amb - 1):
-            self.__list_opc_mov_ag.append((pos_agente[1], pos_agente[0] - 1))
+            self.__list_opc_mov_ag.append((pos_agente[0] - 1, pos_agente[1]))
         elif (pos_agente[0] > 0) and (pos_agente[0] < (dimensao_amb - 1)):
-            self.__list_opc_mov_ag.append((pos_agente[1], pos_agente[0] + 1))
-            self.__list_opc_mov_ag.append((pos_agente[1], pos_agente[0] - 1))
+            self.__list_opc_mov_ag.append((pos_agente[0] + 1, pos_agente[1]))
+            self.__list_opc_mov_ag.append((pos_agente[0] - 1, pos_agente[1]))
 
         if pos_agente[1] == 0:
-            self.__list_opc_mov_ag.append((pos_agente[1] + 1, pos_agente[0]))
+            self.__list_opc_mov_ag.append((pos_agente[0], pos_agente[1] + 1))
         elif pos_agente[1] == (dimensao_amb - 1):
-            self.__list_opc_mov_ag.append((pos_agente[1] - 1, pos_agente[0]))
+            self.__list_opc_mov_ag.append((pos_agente[0], pos_agente[1] - 1))
         elif (pos_agente[1] > 0) and (pos_agente[1] < (dimensao_amb - 1)):
-            self.__list_opc_mov_ag.append((pos_agente[1] + 1, pos_agente[0]))
-            self.__list_opc_mov_ag.append((pos_agente[1] - 1, pos_agente[0]))
+            self.__list_opc_mov_ag.append((pos_agente[0], pos_agente[1] + 1))
+            self.__list_opc_mov_ag.append((pos_agente[0], pos_agente[1] - 1))
 
     def verificar_morte_agente_wumpus(self) -> None:
         pos_wumpus = self.amb.get_pos_objetos()["wumpus"]
         pos_agente = self.amb.get_pos_objetos()["agente"]
         for i in pos_wumpus:
             for j in pos_agente:
                 if i == j:
```

### Comparing `ia_wumpus-0.3.2/ia_wumpus/ambiente.py` & `ia_wumpus-0.3.3/ia_wumpus/ambiente.py`

 * *Files 5% similar despite different names*

```diff
@@ -174,13 +174,20 @@
 
 
 if __name__ == "__main__":
     amb = Ambiente(dimensao_ambiente=5)
     # amb.infos_ambiente()
     amb.mostrar_ambiente()
     # amb.mostrar_percepcoes()
-    amb.atualiza_pos_agente((1, 1))
+    amb.atualiza_pos_agente((0, 1))
     amb.mostrar_ambiente()
-    amb.atualiza_pos_agente((2, 2))
+    amb.atualiza_pos_agente((0, 2))
     amb.mostrar_ambiente()
-    amb.atualiza_pos_agente((3, 3))
+    amb.atualiza_pos_agente((0, 3))
+    amb.mostrar_ambiente()
+
+    amb.atualiza_pos_agente((0, 4))
+    amb.mostrar_ambiente()
+    amb.atualiza_pos_agente((1, 4))
+    amb.mostrar_ambiente()
+    amb.atualiza_pos_agente((2, 4))
     amb.mostrar_ambiente()
```

### Comparing `ia_wumpus-0.3.2/ia_wumpus/dinamica_agente_ambiente.py` & `ia_wumpus-0.3.3/ia_wumpus/dinamica_agente_ambiente.py`

 * *Files identical despite different names*

### Comparing `ia_wumpus-0.3.2/PKG-INFO` & `ia_wumpus-0.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ia-wumpus
-Version: 0.3.2
+Version: 0.3.3
 Summary: Projeto O Mundo do Wumpus - Anbiente para estudo da disciplina de Inteligencia Computacional.
 Author: Oseiasdfarias
 Author-email: oseias.dfarias@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

