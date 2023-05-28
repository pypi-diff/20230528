# Comparing `tmp/ia_wumpus-0.3.tar.gz` & `tmp/ia_wumpus-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ia_wumpus-0.3.tar", max compression
+gzip compressed data, was "ia_wumpus-0.3.2.tar", max compression
```

## Comparing `ia_wumpus-0.3.tar` & `ia_wumpus-0.3.2.tar`

### file list

```diff
@@ -1,6 +1,8 @@
--rw-r--r--   0        0        0     1071 2023-05-06 13:51:13.656383 ia_wumpus-0.3/LICENSE
--rw-r--r--   0        0        0     3921 2023-05-18 15:05:34.982478 ia_wumpus-0.3/README.md
--rw-r--r--   0        0        0      556 2023-05-18 16:12:01.534500 ia_wumpus-0.3/ia_wumpus/__init__.py
--rw-r--r--   0        0        0     7172 2023-05-18 16:11:42.806216 ia_wumpus-0.3/ia_wumpus/ambiente.py
--rw-r--r--   0        0        0      474 2023-05-18 16:12:36.364693 ia_wumpus-0.3/pyproject.toml
--rw-r--r--   0        0        0     4495 1970-01-01 00:00:00.000000 ia_wumpus-0.3/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-05-06 13:51:13.656383 ia_wumpus-0.3.2/LICENSE
+-rw-r--r--   0        0        0     3921 2023-05-18 15:05:34.982478 ia_wumpus-0.3.2/README.md
+-rw-r--r--   0        0        0      636 2023-05-27 22:33:07.393251 ia_wumpus-0.3.2/ia_wumpus/__init__.py
+-rw-r--r--   0        0        0     6276 2023-05-27 19:32:15.239720 ia_wumpus-0.3.2/ia_wumpus/agente_reativo_v1.py
+-rw-r--r--   0        0        0     7406 2023-05-27 17:56:52.970762 ia_wumpus-0.3.2/ia_wumpus/ambiente.py
+-rw-r--r--   0        0        0     1355 2023-05-27 02:48:23.434838 ia_wumpus-0.3.2/ia_wumpus/dinamica_agente_ambiente.py
+-rw-r--r--   0        0        0      476 2023-05-27 22:33:13.597239 ia_wumpus-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     4497 1970-01-01 00:00:00.000000 ia_wumpus-0.3.2/PKG-INFO
```

### Comparing `ia_wumpus-0.3/LICENSE` & `ia_wumpus-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ia_wumpus-0.3/README.md` & `ia_wumpus-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `ia_wumpus-0.3/ia_wumpus/ambiente.py` & `ia_wumpus-0.3.2/ia_wumpus/ambiente.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,141 +13,145 @@
 #            Oséias Farias
 #
 # Data: Maio - 2023
 #  ----------------------------------------------------
 
 import numpy as np
 from random import randint
-import numpy.typing as npt
 from typing import Tuple, Dict
 
 
 class Ambiente:
     """
         Classe que implementa o Ambiente e as percepções
         do Mundo do Wumpus.
     """
     def __init__(self, dimensao_ambiente: int = 3,
                  wumpus: int = 1, ouro: int = 1) -> None:
-        self.pocos = dimensao_ambiente
+        if dimensao_ambiente < 3:
+            self.dimensao_ambiente = 3
+        else:
+            self.dimensao_ambiente = dimensao_ambiente
+        self.pocos = self.dimensao_ambiente
         self.wumpus = wumpus
         self.ouro = ouro
-        self.dimensoes = (dimensao_ambiente, dimensao_ambiente)
+        self.dimensoes = (self.dimensao_ambiente,
+                          self.dimensao_ambiente)
 
         self.__mundo = np.zeros(self.dimensoes, dtype=int)
         self.__mundo[:] = 0
 
         # Percepções dos Objetos no Ambiente.
-        self.percepcoes: dict = {"pocos":  [],
-                                 "wumpus": [],
-                                 "ouro":   []}
+        self.__pos_percepcoes: dict = {"brisa":  [],
+                                       "fedor":  [],
+                                       "brilho": []}
         # Posições dos Objetos no Ambiente.
-        self.pos_objetos: dict = {"pocos":  [],
-                                  "wumpus": [],
-                                  "ouro":   [],
-                                  "agente": []}
+        self.__pos_objetos: dict = {"pocos":  [],
+                                    "wumpus": [],
+                                    "ouro":   [],
+                                    "agente": []}
 
         # Posicionando o Agente no ambiente.
         self.__add_pos_agente()
         # Posicionando o(s) Wumpu(s) no ambiente.
         self.__add_pos_wumpus()
         # Posicionando o(s) Poço(s) no ambiente.
         self.__add_pos_pocos()
         # Posicionando o(s) Ouro(s) no ambiente.
         self.__add_pos_ouro()
         # Menu
         self.__menu()
 
     def atualiza_pos_agente(self, pos_agente: Tuple[int, int]) -> None:
         """Atualiza a posição do Agente no Ambiente."""
-        self.__mundo[self.pos_objetos["agente"][-1]] = 0
-        print("antes ", self.pos_objetos["agente"][-1])
-        self.pos_objetos["agente"] = [pos_agente]
-        print("depois ", self.pos_objetos["agente"][-1])
-        self.__mundo[self.pos_objetos["agente"][-1]] = 4
+        self.__mundo[self.__pos_objetos["agente"][-1]] = 0
+        # print("antes ", self.__pos_objetos["agente"][-1])
+        self.__pos_objetos["agente"] = [pos_agente]
+        # print("depois ", self.__pos_objetos["agente"][-1])
+        self.__mundo[self.__pos_objetos["agente"][-1]] = 4
 
     def get_pos_objetos(self) -> Dict:
         """Obtem as posições dos Objetos no Ambiente."""
-        return self.pos_objetos
+        return self.__pos_objetos
 
     def get_percepcoes(self) -> Dict:
         """Obtem as percepções dos Objetos no Ambiente."""
-        return self.percepcoes
+        return self.__pos_percepcoes
 
-    def add_pos_obj_map(self, obj: int) -> npt.NDArray:
+    def __add_pos_obj_map(self, obj: int) -> Tuple:
         """Posiciona os Objetos no Ambiente."""
         self.pos_sort = self.__sortear_pos()
         if self.__mundo[self.pos_sort[0], self.pos_sort[1]] == 0:
             self.__mundo[self.pos_sort[0], self.pos_sort[1]] = obj
             return self.pos_sort
         elif ((self.pos_sort[0] == 0) and (self.pos_sort[1] == 0)):
-            self.add_pos_obj_map(obj)
+            self.__add_pos_obj_map(obj)
         else:
-            self.add_pos_obj_map(obj)
+            self.__add_pos_obj_map(obj)
         return self.pos_sort
 
-    def salvar_pos_objetos(self, objeto: str, pos_objeto) -> None:
+    def __salvar_pos_objetos(self, objeto: str, pos_objeto) -> None:
         """Armazena as posições dos Objetos em um dicionário Python."""
-        self.pos_objetos[objeto].append(pos_objeto)
+        self.__pos_objetos[objeto].append(pos_objeto)
 
-    def __sortear_pos(self) -> npt.NDArray:
+    def __sortear_pos(self) -> Tuple:
         """Sortea as posições dos Objetos no Ambiente."""
         x = randint(0, self.dimensoes[0]-1)
         y = randint(0, self.dimensoes[0]-1)
-        return np.array([x, y])
+        return (x, y)
 
-    def __add_percepcoes_obj(self, objeto: str, pos: npt.NDArray) -> None:
+    def __add_percepcoes_obj(self, objeto: str, pos: Tuple) -> None:
         """Posiciona as percepções no Ambiente."""
         if pos[0] == 0:
-            self.percepcoes[objeto].append((pos[1], pos[0] + 1))
+            self.__pos_percepcoes[objeto].append((pos[1], pos[0] + 1))
         elif pos[0] == (self.dimensoes[0] - 1):
-            self.percepcoes[objeto].append((pos[1], pos[0] - 1))
+            self.__pos_percepcoes[objeto].append((pos[1], pos[0] - 1))
         elif (pos[0] > 0) and (pos[0] < (self.dimensoes[0] - 1)):
-            self.percepcoes[objeto].append((pos[1], pos[0] + 1))
-            self.percepcoes[objeto].append((pos[1], pos[0] - 1))
+            self.__pos_percepcoes[objeto].append((pos[1], pos[0] + 1))
+            self.__pos_percepcoes[objeto].append((pos[1], pos[0] - 1))
 
         if pos[1] == 0:
-            self.percepcoes[objeto].append((pos[1] + 1, pos[0]))
+            self.__pos_percepcoes[objeto].append((pos[1] + 1, pos[0]))
         elif pos[1] == (self.dimensoes[0] - 1):
-            self.percepcoes[objeto].append((pos[1] - 1, pos[0]))
+            self.__pos_percepcoes[objeto].append((pos[1] - 1, pos[0]))
         elif (pos[1] > 0) and (pos[1] < (self.dimensoes[0] - 1)):
-            self.percepcoes[objeto].append((pos[1] + 1, pos[0]))
-            self.percepcoes[objeto].append((pos[1] - 1, pos[0]))
+            self.__pos_percepcoes[objeto].append((pos[1] + 1, pos[0]))
+            self.__pos_percepcoes[objeto].append((pos[1] - 1, pos[0]))
 
     def __add_pos_wumpus(self) -> None:
         """Posicionando os Wumpo(s) no Ambiente."""
         for i in range(self.wumpus):
-            pos_wumpus = self.add_pos_obj_map(1)
-            self.salvar_pos_objetos(objeto="wumpus", pos_objeto=pos_wumpus)
-            self.__add_percepcoes_obj(objeto="wumpus", pos=pos_wumpus)
-            # print(f"Wumpus pos: {pos_wumpus}")
+            pos_wumpus = self.__add_pos_obj_map(1)
+            self.__salvar_pos_objetos(objeto="wumpus", pos_objeto=pos_wumpus)
+            self.__add_percepcoes_obj(objeto="fedor", pos=pos_wumpus)
+            # print(f"am Wumpus pos: {pos_wumpus}")
 
     def __add_pos_pocos(self) -> None:
         """Posicionando os Poços no Ambiente."""
         for i in range(self.pocos):
-            pos_poco = self.add_pos_obj_map(2)
-            self.salvar_pos_objetos(objeto="pocos", pos_objeto=pos_poco)
-            self.__add_percepcoes_obj(objeto="pocos", pos=pos_poco)
+            pos_poco = self.__add_pos_obj_map(2)
+            self.__salvar_pos_objetos(objeto="pocos", pos_objeto=pos_poco)
+            self.__add_percepcoes_obj(objeto="brisa", pos=pos_poco)
             # print(f"Poço pos: {pos_poco}")
 
     def __add_pos_ouro(self) -> None:
         """Posicionando o(s) Ouro(s) no Ambiente."""
         for i in range(self.ouro):
-            pos_ouro = self.add_pos_obj_map(3)
-            self.salvar_pos_objetos(objeto="ouro", pos_objeto=pos_ouro)
-            self.percepcoes["ouro"].append((pos_ouro[1], pos_ouro[0]))
+            pos_ouro = self.__add_pos_obj_map(3)
+            self.__salvar_pos_objetos(objeto="ouro", pos_objeto=pos_ouro)
+            self.__pos_percepcoes["brilho"].append((pos_ouro[1], pos_ouro[0]))
             # print(f"Ouro pos: {pos_ouro}")
 
     def __add_pos_agente(self) -> None:
         """Posicionando o(s) Agente(s) no Ambiente."""
         self.__mundo[(0, 0)] = 4
-        self.salvar_pos_objetos(objeto="agente", pos_objeto=((0, 0)))
+        self.__salvar_pos_objetos(objeto="agente", pos_objeto=(0, 0))
 
-    @classmethod
-    def __menu(self) -> None:
+    @staticmethod
+    def __menu() -> None:
         """Menu com a descrições dos Objetos."""
         print("\n====== Menu - Mundo do Wumpus ======")
         print("\t+ 1 - Wumpus")
         print("\t+ 2 - Poços")
         print("\t+ 3 - Ouro")
         print("\t+ 4 - Agente")
         print("====================================")
@@ -159,17 +163,17 @@
     def mostrar_ambiente(self) -> None:
         """Exibe o Mundo do Wumpus com os objetos em suas posições."""
         print(f"\nMundo do Wumpus:\n{self.__mundo}")
 
     def mostrar_percepcoes(self):
         """Exibe o dicionário com as posições das percepções."""
         print("\n======== Posições das Percepções - Mundo do Wumpus ========")
-        print(f"\tPos - Percepção do Wumpus:\n\t{self.percepcoes['wumpus']}\n")
-        print(f"\tPos - Percepção do Poços:\n\t{self.percepcoes['pocos']}\n")
-        print(f"\tPos - Percepção do Ouro:\n\t{self.percepcoes['ouro']}")
+        print(f"Posição Fedor  :\n\t{self.__pos_percepcoes['fedor']}")
+        print(f"Posições Brisa :\n\t{self.__pos_percepcoes['brisa']}")
+        print(f"Posição Brilho :\n\t{self.__pos_percepcoes['brilho']}")
         print("============================================================\n")
 
 
 if __name__ == "__main__":
     amb = Ambiente(dimensao_ambiente=5)
     # amb.infos_ambiente()
     amb.mostrar_ambiente()
```

### Comparing `ia_wumpus-0.3/PKG-INFO` & `ia_wumpus-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ia-wumpus
-Version: 0.3
+Version: 0.3.2
 Summary: Projeto O Mundo do Wumpus - Anbiente para estudo da disciplina de Inteligencia Computacional.
 Author: Oseiasdfarias
 Author-email: oseias.dfarias@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

