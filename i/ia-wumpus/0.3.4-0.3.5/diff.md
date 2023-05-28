# Comparing `tmp/ia_wumpus-0.3.4.tar.gz` & `tmp/ia_wumpus-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ia_wumpus-0.3.4.tar", max compression
+gzip compressed data, was "ia_wumpus-0.3.5.tar", max compression
```

## Comparing `ia_wumpus-0.3.4.tar` & `ia_wumpus-0.3.5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1071 2023-05-06 13:51:13.656383 ia_wumpus-0.3.4/LICENSE
--rw-r--r--   0        0        0     3921 2023-05-18 15:05:34.982478 ia_wumpus-0.3.4/README.md
--rw-r--r--   0        0        0      636 2023-05-28 14:43:13.018218 ia_wumpus-0.3.4/ia_wumpus/__init__.py
--rw-r--r--   0        0        0     8202 2023-05-28 18:03:34.486720 ia_wumpus-0.3.4/ia_wumpus/agente_reativo_v1.py
--rw-r--r--   0        0        0     8973 2023-05-28 18:40:13.592967 ia_wumpus-0.3.4/ia_wumpus/ambiente.py
--rw-r--r--   0        0        0     1355 2023-05-27 02:48:23.434838 ia_wumpus-0.3.4/ia_wumpus/dinamica_agente_ambiente.py
--rw-r--r--   0        0        0      511 2023-05-28 18:43:53.012821 ia_wumpus-0.3.4/pyproject.toml
--rw-r--r--   0        0        0     4575 1970-01-01 00:00:00.000000 ia_wumpus-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-05-06 13:51:13.656383 ia_wumpus-0.3.5/LICENSE
+-rw-r--r--   0        0        0     3921 2023-05-18 15:05:34.982478 ia_wumpus-0.3.5/README.md
+-rw-r--r--   0        0        0      636 2023-05-28 14:43:13.018218 ia_wumpus-0.3.5/ia_wumpus/__init__.py
+-rw-r--r--   0        0        0     8519 2023-05-28 19:13:54.450734 ia_wumpus-0.3.5/ia_wumpus/agente_reativo_v1.py
+-rw-r--r--   0        0        0     8960 2023-05-28 19:01:53.341149 ia_wumpus-0.3.5/ia_wumpus/ambiente.py
+-rw-r--r--   0        0        0     1355 2023-05-27 02:48:23.434838 ia_wumpus-0.3.5/ia_wumpus/dinamica_agente_ambiente.py
+-rw-r--r--   0        0        0      511 2023-05-28 19:16:32.303392 ia_wumpus-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0     4575 1970-01-01 00:00:00.000000 ia_wumpus-0.3.5/PKG-INFO
```

### Comparing `ia_wumpus-0.3.4/LICENSE` & `ia_wumpus-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ia_wumpus-0.3.4/README.md` & `ia_wumpus-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `ia_wumpus-0.3.4/ia_wumpus/__init__.py` & `ia_wumpus-0.3.5/ia_wumpus/__init__.py`

 * *Files identical despite different names*

### Comparing `ia_wumpus-0.3.4/ia_wumpus/agente_reativo_v1.py` & `ia_wumpus-0.3.5/ia_wumpus/agente_reativo_v1.py`

 * *Files 3% similar despite different names*

```diff
@@ -44,14 +44,15 @@
     def get_opcoes_mov(self) -> List:
         """
         Método responsável por obter as possíveis obções de movimentação
         do agente no ambiente.
         """
         pos_agente = self.amb.get_pos_objetos()["agente"][0]
         self.__opcoes_mov_agente(pos_agente=pos_agente)
+        print(self.__list_opc_mov_ag)
         return self.__list_opc_mov_ag
 
     def __opcoes_mov_agente(self, pos_agente: Tuple) -> None:
         """
             Verifica as possíveis opções de movimentação do agente
             para a posição atual.
         """
@@ -186,27 +187,34 @@
 
     def mostrar_opcoes_mov(self) -> None:
         print(self.__list_opc_mov_ag)
 
 
 if __name__ == "__main__":
     rodadas = 0
+    passos = 0
     while True:
-        amb = Ambiente()
+        passos = 0
+        amb = Ambiente(dimensao_ambiente=5, t_pausa=0.0)
         amb.mostrar_ambiente()
         agente = AgenteReativoV1(amb)
         while True:
             agente.verificar_atirar_wumpus()
             pos_mov = agente.sortear_pos(agente.get_opcoes_mov())
             amb.atualiza_pos_agente(pos_mov)
             amb.mostrar_ambiente()
             agente.pegar_outro()
             agente.status_agente_ouro()
             agente.verificar_morte_agente_wumpus()
             agente.verificar_morte_agente_poco()
             if agente.verificar_vitorio():
+                passos += 1
+                rodadas += 1
                 agente.ganhou_jogo()
-                print(f"Quantidade de rodadas: {rodadas}")
+                print(f"Quantidade de passos no Ambiente: {passos}")
+                print(f"Quantidade de rodadas: {rodadas}\n")
                 os._exit(0)
             elif agente.morreu:
                 break
+            passos += 1
+        print(f"Quantidade de passos no Ambiente: {passos}")
         rodadas += 1
```

### Comparing `ia_wumpus-0.3.4/ia_wumpus/ambiente.py` & `ia_wumpus-0.3.5/ia_wumpus/ambiente.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,18 +20,18 @@
 from typing import Tuple, Dict
 from rich.console import Console
 from rich.theme import Theme
 from os import system, name
 from time import sleep
 
 custom_theme = Theme({
-    "info": "purple",
+    "info1": "dim cyan bold",
     "color_mundo": "blue bold",
     "color_menus": "blue bold",
-    "info_bold": "purple bold",
+    "info2": "purple bold",
     "warning": "magenta",
     "green": "green",
     "danger": "red"
 })
 console = Console(theme=custom_theme)
 
 
@@ -91,17 +91,15 @@
             _ = system('cls')
         else:
             _ = system('clear')
 
     def atualiza_pos_agente(self, pos_agente: Tuple[int, int]) -> None:
         """Atualiza a posição do Agente no Ambiente."""
         self.__mundo[self.__pos_objetos["agente"][-1]] = 0
-        # print("antes ", self.__pos_objetos["agente"][-1])
         self.__pos_objetos["agente"] = [pos_agente]
-        # print("depois ", self.__pos_objetos["agente"][-1])
         self.__mundo[self.__pos_objetos["agente"][-1]] = 4
 
     def get_pos_objetos(self) -> Dict:
         """Obtem as posições dos Objetos no Ambiente."""
         return self.__pos_objetos
 
     def set_pos_ouro(self) -> None:
@@ -156,31 +154,28 @@
 
     def __add_pos_wumpus(self) -> None:
         """Posicionando os Wumpo(s) no Ambiente."""
         for i in range(self.wumpus):
             pos_wumpus = self.__add_pos_obj_map(1)
             self.__salvar_pos_objetos(objeto="wumpus", pos_objeto=pos_wumpus)
             self.__add_percepcoes_obj(objeto="fedor", pos=pos_wumpus)
-            # print(f"am Wumpus pos: {pos_wumpus}")
 
     def __add_pos_pocos(self) -> None:
         """Posicionando os Poços no Ambiente."""
         for i in range(self.pocos):
             pos_poco = self.__add_pos_obj_map(2)
             self.__salvar_pos_objetos(objeto="pocos", pos_objeto=pos_poco)
             self.__add_percepcoes_obj(objeto="brisa", pos=pos_poco)
-            # print(f"Poço pos: {pos_poco}")
 
     def __add_pos_ouro(self) -> None:
         """Posicionando o(s) Ouro(s) no Ambiente."""
         for i in range(self.ouro):
             pos_ouro = self.__add_pos_obj_map(3)
             self.__salvar_pos_objetos(objeto="ouro", pos_objeto=pos_ouro)
             self.__pos_percepcoes["brilho"].append((pos_ouro[1], pos_ouro[0]))
-            # print(f"Ouro pos: {pos_ouro}")
 
     def __add_pos_agente(self) -> None:
         """Posicionando o(s) Agente(s) no Ambiente."""
         self.__mundo[(0, 0)] = 4
         self.__salvar_pos_objetos(objeto="agente", pos_objeto=(0, 0))
 
     @staticmethod
@@ -205,33 +200,40 @@
     def mostrar_ambiente(self) -> None:
         """Exibe o Mundo do Wumpus com os objetos em suas posições."""
         console.print(f"\n[gray]Mundo do Wumpus:\n{self.__mundo}",
                       style="color_mundo")
         self.tempo_pausa()
 
     def mostrar_percepcoes(self):
+        style = "info2"
         """Exibe o dicionário com as posições das percepções."""
-        print("\n======== Posições das Percepções - Mundo do Wumpus ========")
-        print(f"Posição Fedor  :\n\t{self.__pos_percepcoes['fedor']}")
-        print(f"Posições Brisa :\n\t{self.__pos_percepcoes['brisa']}")
-        print(f"Posição Brilho :\n\t{self.__pos_percepcoes['brilho']}")
-        print("============================================================\n")
+        console.print("\n================ Posições das Percepções =========",
+                      style=style)
+        console.print(f"Posição Fedor  :\n\t{self.__pos_percepcoes['fedor']}",
+                      style=style)
+        console.print(f"Posições Brisa :\n\t{self.__pos_percepcoes['brisa']}",
+                      style=style)
+        console.print(f"Posição Brilho :\n\t{self.__pos_percepcoes['brilho']}",
+                      style=style)
+        console.print("==================================================\n",
+                      style=style)
 
 
 if __name__ == "__main__":
     amb = Ambiente(dimensao_ambiente=5)
     # amb.infos_ambiente()
     amb.mostrar_ambiente()
-    # amb.mostrar_percepcoes()
+    amb.mostrar_percepcoes()
     amb.atualiza_pos_agente((0, 1))
     amb.mostrar_ambiente()
     amb.atualiza_pos_agente((0, 2))
     amb.mostrar_ambiente()
     amb.atualiza_pos_agente((0, 3))
     amb.mostrar_ambiente()
 
     amb.atualiza_pos_agente((0, 4))
     amb.mostrar_ambiente()
     amb.atualiza_pos_agente((1, 4))
     amb.mostrar_ambiente()
     amb.atualiza_pos_agente((2, 4))
     amb.mostrar_ambiente()
+    amb.mostrar_percepcoes()
```

### Comparing `ia_wumpus-0.3.4/ia_wumpus/dinamica_agente_ambiente.py` & `ia_wumpus-0.3.5/ia_wumpus/dinamica_agente_ambiente.py`

 * *Files identical despite different names*

### Comparing `ia_wumpus-0.3.4/PKG-INFO` & `ia_wumpus-0.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ia-wumpus
-Version: 0.3.4
+Version: 0.3.5
 Summary: Projeto O Mundo do Wumpus - Anbiente para estudo da disciplina de Inteligencia Computacional.
 Author: Oseiasdfarias
 Author-email: oseias.dfarias@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

