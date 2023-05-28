# Comparing `tmp/s27a_jbq-1.0.2.tar.gz` & `tmp/s27a_jbq-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "s27a_jbq-1.0.2.tar", last modified: Thu May 25 12:45:15 2023, max compression
+gzip compressed data, was "s27a_jbq-1.0.3.tar", last modified: Sat May 27 11:09:22 2023, max compression
```

## Comparing `s27a_jbq-1.0.2.tar` & `s27a_jbq-1.0.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-05-25 12:45:15.573660 s27a_jbq-1.0.2/
--rw-rw-rw-   0        0        0     1064 2023-04-16 06:28:36.000000 s27a_jbq-1.0.2/LICENSE
--rw-rw-rw-   0        0        0    11851 2023-05-25 12:45:15.573660 s27a_jbq-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0    11334 2023-05-24 11:17:11.000000 s27a_jbq-1.0.2/README.md
--rw-rw-rw-   0        0        0      597 2023-05-23 12:26:37.000000 s27a_jbq-1.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-25 12:45:15.581166 s27a_jbq-1.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-25 12:45:15.526142 s27a_jbq-1.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-05-25 12:45:15.561578 s27a_jbq-1.0.2/src/s27a_jbq/
--rw-rw-rw-   0        0        0      177 2023-05-24 12:28:15.000000 s27a_jbq-1.0.2/src/s27a_jbq/__constants__.py
--rw-rw-rw-   0        0        0       87 2023-05-24 13:02:51.000000 s27a_jbq-1.0.2/src/s27a_jbq/__init__.py
--rw-rw-rw-   0        0        0     2188 2023-05-24 11:40:26.000000 s27a_jbq-1.0.2/src/s27a_jbq/__main__.py
--rw-rw-rw-   0        0        0     3970 2023-05-16 13:59:35.000000 s27a_jbq-1.0.2/src/s27a_jbq/extension.py
--rw-rw-rw-   0        0        0    10421 2023-05-22 12:26:11.000000 s27a_jbq-1.0.2/src/s27a_jbq/game.py
--rw-rw-rw-   0        0        0     6599 2023-05-24 12:00:48.000000 s27a_jbq-1.0.2/src/s27a_jbq/map.py
--rw-rw-rw-   0        0        0     6870 2023-05-24 12:24:33.000000 s27a_jbq-1.0.2/src/s27a_jbq/static.py
--rw-rw-rw-   0        0        0    16681 2023-05-24 13:03:58.000000 s27a_jbq-1.0.2/src/s27a_jbq/window.py
-drwxrwxrwx   0        0        0        0 2023-05-25 12:45:15.573660 s27a_jbq-1.0.2/src/s27a_jbq.egg-info/
--rw-rw-rw-   0        0        0    11851 2023-05-25 12:45:15.000000 s27a_jbq-1.0.2/src/s27a_jbq.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      369 2023-05-25 12:45:15.000000 s27a_jbq-1.0.2/src/s27a_jbq.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-25 12:45:15.000000 s27a_jbq-1.0.2/src/s27a_jbq.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-25 12:45:15.000000 s27a_jbq-1.0.2/src/s27a_jbq.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-27 11:09:22.333218 s27a_jbq-1.0.3/
+-rw-rw-rw-   0        0        0     1064 2023-04-16 06:28:36.000000 s27a_jbq-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0     4070 2023-05-27 11:09:22.333218 s27a_jbq-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3499 2023-05-27 10:35:28.000000 s27a_jbq-1.0.3/README.md
+-rw-rw-rw-   0        0        0      554 2023-05-27 11:09:02.000000 s27a_jbq-1.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-27 11:09:22.333218 s27a_jbq-1.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-27 11:09:22.308995 s27a_jbq-1.0.3/src/
+drwxrwxrwx   0        0        0        0 2023-05-27 11:09:22.331640 s27a_jbq-1.0.3/src/s27a_jbq/
+-rw-rw-rw-   0        0        0      177 2023-05-26 13:58:29.000000 s27a_jbq-1.0.3/src/s27a_jbq/__constants__.py
+-rw-rw-rw-   0        0        0       87 2023-05-24 13:02:51.000000 s27a_jbq-1.0.3/src/s27a_jbq/__init__.py
+-rw-rw-rw-   0        0        0     2188 2023-05-24 11:40:26.000000 s27a_jbq-1.0.3/src/s27a_jbq/__main__.py
+-rw-rw-rw-   0        0        0     4238 2023-05-27 01:42:31.000000 s27a_jbq-1.0.3/src/s27a_jbq/extension.py
+-rw-rw-rw-   0        0        0     9025 2023-05-27 10:58:01.000000 s27a_jbq-1.0.3/src/s27a_jbq/game.py
+-rw-rw-rw-   0        0        0     6765 2023-05-27 02:14:40.000000 s27a_jbq-1.0.3/src/s27a_jbq/map.py
+-rw-rw-rw-   0        0        0     6946 2023-05-27 10:36:44.000000 s27a_jbq-1.0.3/src/s27a_jbq/static.py
+-rw-rw-rw-   0        0        0    18929 2023-05-27 02:22:25.000000 s27a_jbq-1.0.3/src/s27a_jbq/window.py
+drwxrwxrwx   0        0        0        0 2023-05-27 11:09:22.333218 s27a_jbq-1.0.3/src/s27a_jbq.egg-info/
+-rw-rw-rw-   0        0        0     4070 2023-05-27 11:09:22.000000 s27a_jbq-1.0.3/src/s27a_jbq.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      369 2023-05-27 11:09:22.000000 s27a_jbq-1.0.3/src/s27a_jbq.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-27 11:09:22.000000 s27a_jbq-1.0.3/src/s27a_jbq.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-27 11:09:22.000000 s27a_jbq-1.0.3/src/s27a_jbq.egg-info/top_level.txt
```

### Comparing `s27a_jbq-1.0.2/LICENSE` & `s27a_jbq-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `s27a_jbq-1.0.2/src/s27a_jbq/__main__.py` & `s27a_jbq-1.0.3/src/s27a_jbq/__main__.py`

 * *Files identical despite different names*

### Comparing `s27a_jbq-1.0.2/src/s27a_jbq/extension.py` & `s27a_jbq-1.0.3/src/s27a_jbq/extension.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,14 +22,20 @@
 
     def get_chess_by_arr(self,arr:ARR):
         return self.app.map_data.chessboard[arr[0]][arr[1]]
 
     def get_chess_arr_by_id(self,id:int):
         return self.app.map_data.get_chess_arr_by_id(id)
 
+    def can_eat(self,chess1,chess2):
+        return self.app.map_data.can_eat(chess1,chess2)
+
+    def add_chess(self,id:int,arr:ARR):
+        self.app.map_data.chessboard[arr[0]][arr[1]] = self.app.chess(id,*self.app.map_data.chesses[id - 1],self.app.map_data)
+
     def move(self,arr1:ARR,arr2:ARR):
         return self.app.map_data.move(arr1,arr2,self.turn)
 
 class Extension:
     def __init__(self,methods:dict[str]):
         self.name = methods["EX_NAME"]
         self.version = methods["EX_VERSION"]
```

### Comparing `s27a_jbq-1.0.2/src/s27a_jbq/game.py` & `s27a_jbq-1.0.3/src/s27a_jbq/game.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,19 @@
-import sys
-
-if sys.platform != "win32":
-    sys.stdout("程序必须在Windows系统中运行")
-    sys.exit()
-
-from tkinter.messagebox import showinfo,showwarning,showerror
+from tkinter.messagebox import showinfo,showerror
 
 from .static import ARR,MapViewer,static_data,save_record
 from .map import Chess,Map,HistoryRecorder
 from .window import MainWindow,GameWindow,SettingWindow
 from .extension import ExtAPI,ExtensionManager
 
 class App:
-    RUNNING = False
+    chess = Chess # 扩展调用
+    running = False
     def __init__(self):
-        if App.RUNNING:
+        if App.running:
             raise RuntimeError("App只能有一个实例")
         App.RUNNING = True
         self.map_data = None
         self.map_path = None
         self.open_setting = False
 
     def run(self,debug:bool = False):
@@ -44,19 +39,19 @@
         if self.debug:
             self.map_data = Map(*MapViewer.view(filename))
         else:
             try:
                 self.map_data = Map(*MapViewer.view(filename))
             except FileNotFoundError:
                 if error_prompt:
-                    showwarning("提示","未找到地图文件")
+                    showerror("错误","未找到地图文件")
                 return
             except:
                 if error_prompt:
-                    showwarning("提示","地图文件格式错误")
+                    showerror("错误","地图文件格式错误")
                 return
         if success_prompt:
             showinfo("提示","地图文件加载成功")
         self.map_path = filename
         self.window.set_map(self.map_path)
 
     def start_game(self):
@@ -93,25 +88,26 @@
         window.destroy()
 
 # 游戏类
 # 每场创建一个新的Game对象
 class Game:
     def __init__(self,map_data:Map,debug:bool):
         self.map_data = map_data
-        self.debug = debug
         self.map_data.init_chessboard(self.win)
         self.history_recorder = HistoryRecorder(self.map_data)
         game_api = {
             "click":self.click,
-            "info":self.get_info,
+            "get_chess":lambda arr:self.map_data.chessboard[arr[0]][arr[1]],
+            "get_can_go":self.get_can_go,
+            "chosen_turn":lambda:self.turn if self.chosen else None,
             "back":self.back,
             "stop":self.stop
         }
-        self.red_window = GameWindow(1,self.map_data,game_api)
-        self.blue_window = GameWindow(2,self.map_data,game_api)
+        self.red_window = GameWindow(1,self.map_data,game_api,debug)
+        self.blue_window = GameWindow(2,self.map_data,game_api,debug)
         ExtAPI.win = self.win
         ExtAPI.stalemate = self.stalemate
 
     def start(self):
         self.running = True
         self.turn = 1
         self.chosen = None
@@ -159,15 +155,15 @@
                         break
                 self.red_window.set_text("mess",self.turn if mess else 0)
                 self.blue_window.set_text("mess",self.turn if mess else 0)
                 self.turn = 1 if self.turn == 2 else 2
                 self.history_recorder.add_history(self.map_data,self.turn)
                 self.refresh()
             else:
-                window.choose(self.chosen[1],remove = True)
+                window.choose(*self.chosen,remove = True)
             self.chosen = None
         else: # 选择棋子
             chess = self.map_data.chessboard[arr[0]][arr[1]]
             if not chess:
                 return
             if chess.belong != belong and chess.belong != 3:
                 return
@@ -175,77 +171,49 @@
                 if self.turn == 1 and self.map_data.red_move_ne == 2:
                     return
                 elif self.turn == 2 and self.map_data.blue_move_ne == 2:
                     return
             can_go = self.get_can_go(chess,arr)
             if can_go:
                 self.chosen = [arr,can_go]
-                window.choose(can_go)
+                window.choose(*self.chosen)
 
     # 返回当前棋子可以行走的格子
     def get_can_go(self,chess:Chess,arr:ARR):
         can_go = list[list[ARR]]()
         for i in chess.now_move[0]: # 行走一格
             d_arr = self.map_data.get_arr_by_rd(arr,i,1)
             if not d_arr:
                 continue
             mp = self.map_data.chessboard[d_arr[0]][d_arr[1]]
-            if (not mp) or (chess.belong != 3 and mp.belong != 3 and mp.belong != self.turn):
+            if (not mp) or self.map_data.can_eat(chess,mp):
                 can_go.append([d_arr])
         for i in chess.now_move[1]:
             can_go.append([])
             k = 1
             while True:
                 d_arr = self.map_data.get_arr_by_rd(arr,i,k)
                 if not d_arr:
                     break
                 mp = self.map_data.chessboard[d_arr[0]][d_arr[1]]
                 if not mp: # 空格，继续向远处搜索
                     can_go.append(can_go[-1] + [d_arr])
-                elif chess.belong != 3 and mp.belong != 3 and mp.belong != self.turn:
+                elif self.map_data.can_eat(chess,mp):
                     can_go.append(can_go[-1] + [d_arr])
                     break
                 else:
                     break
                 k += 1
         can_go = ExtensionManager.Ext.check_can_go([i for i in can_go if i],chess,arr) # 载入扩展修改can_go
         can_go_set = set[ARR]() # 集合去重
         for i in can_go:
             for j in i:
                 can_go_set.add(j)
         return list(can_go_set)
 
-    # 显示棋子基本信息
-    def get_info(self,arr:ARR):
-        chess = self.map_data.chessboard[arr[0]][arr[1]]
-        if chess:
-            belong = "红方" if chess.belong == 1 else "蓝方" if chess.belong == 2 else "中立"
-            is_captain = "是" if chess.is_captain else "否"
-            is_tran = ("是" if chess.is_tran else "否") if chess.tran_con else "无法升变"
-            info = f"名称：{chess.name}\n编号：{chess.id}\n归属：{belong}\n首领棋子：{is_captain}\n是否升变：{is_tran}"
-            if self.debug:
-                if chess.attr:
-                    attr = "\n    ".join([f"{i}：{j}" for i,j in zip(chess.attr.keys(),chess.attr.values())])
-                    info += f"\n其他参数：\n    {attr}"
-                move = chess.tran_move if chess.is_tran else chess.move
-                show_move = ""
-                for i in range(len(move)):
-                    show_move += f"\n    第{i + 1}项："
-                    if not move[i]:
-                        show_move += "无"
-                        continue
-                    for j in move[i]:
-                        show_move += f"\n        方向{j[0]}："
-                        if j[1:]:
-                            show_move += f"{j[1:]}"
-                        else:
-                            show_move += "任意"
-                info += f"\n目前可行走函数：{show_move}"
-            showinfo("棋子信息",info)
-
     # 悔棋及撤销
     def back(self,steps:int):
         data = self.history_recorder.rollback(steps)
         if data:
             self.map_data.chessboard,self.turn = data
             self.refresh()
 
@@ -256,9 +224,12 @@
     # 和棋
     # 只能由扩展触发
     def stalemate(self):
         showinfo("提示","双方和棋")
         self.stop()
 
     def stop(self):
-        save_record(self.history_recorder.history) # 记录棋局
+        try:
+            save_record(self.history_recorder.history) # 记录棋局
+        except PermissionError:
+            showerror("错误","棋局记录文件被占用")
         self.running = False
```

### Comparing `s27a_jbq-1.0.2/src/s27a_jbq/map.py` & `s27a_jbq-1.0.3/src/s27a_jbq/map.py`

 * *Files 6% similar despite different names*

```diff
@@ -39,16 +39,15 @@
         self.map = map
         self.rules = rules
         self.rl = len(self.map) # 地图行数
         self.cl = len(self.map[0]) # 地图列数
         self.red_move_ne = 0 # 红方移动中立棋子次数
         self.blue_move_ne = 0
 
-    # 初始化棋盘
-    # 每局初始化一次
+    # 初始化棋盘，每局初始化一次
     def init_chessboard(self,win_func):
         self.win = win_func
         self.chessboard = list[list[Chess]]()
         for i in self.map:
             self.chessboard.append([])
             for j in i:
                 if j:
@@ -110,14 +109,18 @@
                         return True
             for j in ExtensionManager.Ext.loc_rules: # 扩展中的函数
                 if command == j:
                     if ExtensionManager.Ext.loc_rules[j](i[1:],arr):
                         return True
         return False
 
+    # 是否可以吃子
+    def can_eat(self,chess1:Chess,chess2:Chess):
+        return chess1.belong != 3 and chess2.belong != 3 and chess1.belong != chess2.belong
+
     # 移动棋子
     def move(self,arr1:ARR,arr2:ARR,turn:int):
         if self.rules["restrict_move_ne"] and self.chessboard[arr1[0]][arr1[1]] and self.chessboard[arr1[0]][arr1[1]].belong == 3:
             if turn == 1:
                 self.red_move_ne += 1
             else:
                 self.blue_move_ne += 1
```

### Comparing `s27a_jbq-1.0.2/src/s27a_jbq/static.py` & `s27a_jbq-1.0.3/src/s27a_jbq/static.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import os
-import sys
 import csv
 import json
 
 from openpyxl import load_workbook
 
-RELEASE_DATE = "2023-05-25"
+RELEASE_DATE = "2023-05-28"
 COLOR_STYLES = {
     "normal":{
         "name":"标准",
         "colors":{
             "chessboard":"khaki",
             "red-label":"pink",
             "blue-label":"skyblue",
             "chess-bg":"lightyellow",
+            "selected-chess-bg":"yellow",
             "blank-feasible-bg":"lightgreen",
             "occupied-feasible-bg":"pink",
             "red-chess-fg":"lightcoral",
             "red-tran-chess-fg":"red",
             "blue-chess-fg":"cornflowerblue",
             "blue-tran-chess-fg":"blue",
             "neutral-chess-fg":"green"
@@ -26,14 +26,15 @@
     "dark":{
         "name":"暗色",
         "colors":{
             "chessboard":"grey",
             "red-label":"pink",
             "blue-label":"skyblue",
             "chess-bg":"darkslategrey",
+            "selected-chess-bg":"darkgrey",
             "blank-feasible-bg":"green",
             "occupied-feasible-bg":"firebrick",
             "red-chess-fg":"pink",
             "red-tran-chess-fg":"lightcoral",
             "blue-chess-fg":"deepskyblue",
             "blue-tran-chess-fg":"dodgerblue",
             "neutral-chess-fg":"lightgreen"
```

### Comparing `s27a_jbq-1.0.2/src/s27a_jbq/window.py` & `s27a_jbq-1.0.3/src/s27a_jbq/window.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,15 @@
-import tkinter as tk
+import sys
+if sys.platform != "win32":
+    sys.stdout("程序必须在Windows系统中运行")
+    sys.exit()
+
 import webbrowser
 
+import tkinter as tk
 from tkinter.messagebox import showinfo
 from tkinter.filedialog import askopenfilename,asksaveasfilename
 
 from .__constants__ import __version__
 from .static import ARR,RELEASE_DATE,static_data,refresh_extension,refresh_color,set_record_path
 from .map import Chess,Map
 from .extension import Extension,ExtensionManager
@@ -12,14 +17,19 @@
 class MainWindow(tk.Tk):
     def __init__(self,app_api:dict,debug:bool):
         super().__init__()
         self.app_api = app_api
         self.title(f"精班棋 {__version__}{' [debug mode]' if debug else ''}")
         self.minsize(480,360)
         self.resizable(width = False,height = False)
+        self.init_window()
+        self.refresh_extension()
+        self.init_menu()
+
+    def init_window(self):
         self.start_btn = tk.Button(self,text = "开始游戏",width = 60,height = 3,**static_data["shape-style"]["btn-style"],command = self.app_api["start_game"])
         self.start_btn.pack(pady = 5)
         self.map_label = tk.Label(self,text = "未选择地图",width = 60,height = 3,**static_data["shape-style"]["label-style"])
         self.map_label.pack(pady = 5)
         self.map_btn_frame = tk.Frame(self)
         self.map_btn_frame.pack(pady = 5)
         self.get_map_btn = tk.Button(self.map_btn_frame,text = "选择地图",width = 15,height = 2,**static_data["shape-style"]["btn-style"],command = self.app_api["get_map"])
@@ -27,18 +37,14 @@
         self.refresh_map_btn = tk.Button(self.map_btn_frame,text = "刷新地图",width = 15,height = 2,**static_data["shape-style"]["btn-style"],command = self.app_api["refresh_map"])
         self.refresh_map_btn.pack(side = "right",padx = 5)
         self.extension_label = tk.Label(self,width = 60,**static_data["shape-style"]["label-style"])
         self.extension_label.pack(pady = 5)
         self.set_extension_btn = tk.Button(self,text = "设置扩展",width = 15,height = 2,**static_data["shape-style"]["btn-style"],command = self.app_api["setting"])
         self.set_extension_btn.pack(pady = 5)
 
-        self.refresh_extension()
-        self.init_menu()
-
-    # 初始化菜单栏
     def init_menu(self):
         self.menu = tk.Menu(self)
         self.config(menu = self.menu)
         # 文件菜单
         self.file_menu = tk.Menu(self.menu,tearoff = False)
         self.menu.add_cascade(label = "文件(F)",underline = 3,menu = self.file_menu)
         self.file_menu.add_command(label = "选择地图",command = self.app_api["get_map"])
@@ -51,16 +57,15 @@
         self.game_menu = tk.Menu(self.menu,tearoff = False)
         self.menu.add_cascade(label = "游戏(G)",underline = 3,menu = self.game_menu)
         self.game_menu.add_command(label = "开始游戏",command = self.app_api["start_game"])
         # 帮助菜单
         self.help_menu = tk.Menu(self.menu,tearoff = False)
         self.menu.add_cascade(label = "帮助(H)",underline = 3,menu = self.help_menu)
         self.help_menu.add_command(label = "精班棋文档",command = self.open_url("https://github.com/amf14151/s27a_jbq/blob/main/README.md"))
-        self.help_menu.add_command(label = "获取地图",command = self.open_url("https://github.com/amf14151/s27a_jbq/tree/main/map"))
-        self.help_menu.add_command(label = "获取扩展",command = self.open_url("https://github.com/amf14151/s27a_jbq/tree/main/extensions"))
+        self.help_menu.add_command(label = "获取地图/扩展",command = self.open_url("https://amf14151.github.io/JBQ/"))
         self.help_menu.add_separator()
         self.help_menu.add_command(label = "反馈",command = self.open_url("https://github.com/amf14151/s27a_jbq/issues"))
         self.help_menu.add_separator()
         self.help_menu.add_command(label = "关于精班棋",command = self.show_about)
 
     def choose_map_file(self):
         filename = askopenfilename(filetypes = [("Excel Files","*.xlsx"),("All Files","*.*")],title = "选择地图文件")
@@ -81,20 +86,21 @@
     def open_url(self,url:str):
         return lambda:webbrowser.open(url)
 
     def show_about(self):
         showinfo("关于精班棋",f"版本: {__version__}\n发布日期: {RELEASE_DATE}")
 
 class GameWindow(tk.Tk):
-    def __init__(self,belong:int,map_data:Map,game_api:dict):
+    def __init__(self,belong:int,map_data:Map,game_api:dict,debug:bool):
         super().__init__()
         self.belong = belong
         self.map_data = map_data
         self.game_api = game_api
-        self.can_go_prompt_list = ["·","*","o","x","%"]
+        self.debug = debug
+        self.can_go_prompt_list = ["·","*","o","x","$","%"]
         self.show_can_go_prompt = True
         self.title("红方" if self.belong == 1 else "蓝方")
         self.resizable(width = False,height = False)
         self.protocol("WM_DELETE_WINDOW",self.game_api["stop"])
         self.init_menu()
         self.init_chessboard()
         self.refresh_map()
@@ -165,38 +171,83 @@
         self.chess_frame = tk.Frame(self,bg = static_data["colors"]["chessboard"])
         self.chess_btn = list[list[tk.Button]]()
         for i in range(self.map_data.rl):
             self.chess_btn.append([])
             for j in range(self.map_data.cl):
                 self.chess_btn[-1].append(tk.Button(self.chess_frame,height = 3,width = 8,relief = "flat",bd = 0,command = self.click(i,j,1)))
                 self.chess_btn[-1][-1].bind("<Button 3>",self.click(i,j,3))
+                self.chess_btn[-1][-1].bind("<Enter>",self.click(i,j,4))
+                self.chess_btn[-1][-1].bind("<Leave>",self.click(i,j,5))
                 self.chess_btn[-1][-1].grid(row = i,column = j,padx = 1,pady = 1)
         self.chess_frame.pack()
         self.mess_label = tk.Label(self,height = 3,width = 24)
         self.mess_label.pack()
         if len(self.chess_btn) > 8 or len(self.chess_btn[0]) > 12:
             self.change_chess_height()
             self.change_show_prompt()
 
     # 点击棋子回调中转函数
     def click(self,x:int,y:int,key:int):
+        x = self.getx(x)
+        y = self.gety(y)
         def wrapper(event = None):
-            if key == 1:
-                self.game_api["click"]((self.getx(x),self.gety(y)),self.belong)
+            if key == 1: # 左键
+                self.game_api["click"]((x,y),self.belong)
+                return
+            else:
+                chess = self.game_api["get_chess"]((x,y))
+                if not chess:
+                    return
+            if key == 3: # 右键
+                self.get_info(chess)
+                return
             else:
-                self.game_api["info"]((self.getx(x),self.gety(y)))
+                if self.game_api["chosen_turn"]() == self.belong:
+                    return
+            if key == 4: # 进入
+                self.choose(None,self.game_api["get_can_go"](chess,(x,y)))
+            elif key == 5: # 离开
+                self.choose(None,self.game_api["get_can_go"](chess,(x,y)),remove = True)
         return wrapper
 
+    # 显示棋子基本信息
+    def get_info(self,chess:Chess):
+        belong = "红方" if chess.belong == 1 else "蓝方" if chess.belong == 2 else "中立"
+        is_captain = "是" if chess.is_captain else "否"
+        is_tran = ("是" if chess.is_tran else "否") if chess.tran_con else "无法升变"
+        info = f"名称：{chess.name}\n编号：{chess.id}\n归属：{belong}\n首领棋子：{is_captain}\n是否升变：{is_tran}"
+        if self.debug:
+            if chess.attr:
+                attr = "\n    ".join([f"{i}：{j}" for i,j in zip(chess.attr.keys(),chess.attr.values())])
+                info += f"\n其他参数：\n    {attr}"
+            move = chess.tran_move if chess.is_tran else chess.move
+            show_move = ""
+            for i in range(len(move)):
+                if not move[i]:
+                    continue
+                show_move += f"\n    第{i + 1}项（{self.can_go_prompt_list[i]}）："
+                for j in move[i]:
+                    show_move += f"\n        方向{j[0]}："
+                    if j[1:]:
+                        show_move += f"{j[1:]}"
+                    else:
+                        show_move += "任意"
+            info += f"\n目前可行走函数：{show_move}"
+        showinfo("棋子信息",info)
+
     def set_text(self,type:str,fro:int,turn:tuple = None):
         if type == "turn": # 设置回合
             self.turn_label["text"] = f"{'己方' if fro == self.belong else '对方'}回合\n回合数：{turn[0]}/{turn[1]}"
         elif type == "mess": # 设置将军
             self.mess_label["text"] = f"{'红方' if fro == 1 else '蓝方'}将军！" if fro else ""
 
-    def choose(self,can_go:list[ARR],remove:bool = False):
+    def choose(self,arr:ARR,can_go:list[ARR],remove:bool = False):
+        if arr:
+            bg = "chess-bg" if remove else "selected-chess-bg"
+            self.chess_btn[self.getx(arr[0])][self.gety(arr[1])]["bg"] = static_data["colors"][bg]
         for i in can_go:
             bg = "chess-bg" if remove else ("occupied-feasible-bg" if self.map_data.chessboard[i[0]][i[1]] else "blank-feasible-bg")
             self.chess_btn[self.getx(i[0])][self.gety(i[1])]["bg"] = static_data["colors"][bg]
 
     def refresh_map(self):
         for i in range(self.map_data.rl):
             for j in range(self.map_data.cl):
```

