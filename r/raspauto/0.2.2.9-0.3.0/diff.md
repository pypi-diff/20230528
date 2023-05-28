# Comparing `tmp/raspauto-0.2.2.9.tar.gz` & `tmp/raspauto-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "raspauto-0.2.2.9.tar", last modified: Mon Sep 27 19:45:41 2021, max compression
+gzip compressed data, was "raspauto-0.3.0.tar", last modified: Sun May 28 18:49:39 2023, max compression
```

## Comparing `raspauto-0.2.2.9.tar` & `raspauto-0.3.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-27 19:45:41.586721 raspauto-0.2.2.9/
--rw-r--r--   0 runner    (1001) docker     (121)    34523 2021-09-27 19:45:28.000000 raspauto-0.2.2.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     5657 2021-09-27 19:45:41.586721 raspauto-0.2.2.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5231 2021-09-27 19:45:28.000000 raspauto-0.2.2.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-27 19:45:41.582721 raspauto-0.2.2.9/raspauto/
--rw-r--r--   0 runner    (1001) docker     (121)    16179 2021-09-27 19:45:28.000000 raspauto-0.2.2.9/raspauto/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-27 19:45:41.582721 raspauto-0.2.2.9/raspauto.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5657 2021-09-27 19:45:41.000000 raspauto-0.2.2.9/raspauto.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      206 2021-09-27 19:45:41.000000 raspauto-0.2.2.9/raspauto.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-09-27 19:45:41.000000 raspauto-0.2.2.9/raspauto.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       20 2021-09-27 19:45:41.000000 raspauto-0.2.2.9/raspauto.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2021-09-27 19:45:41.000000 raspauto-0.2.2.9/raspauto.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-09-27 19:45:41.586721 raspauto-0.2.2.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      772 2021-09-27 19:45:28.000000 raspauto-0.2.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:49:39.523830 raspauto-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    34524 2023-05-28 18:49:27.000000 raspauto-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5691 2023-05-28 18:49:39.523830 raspauto-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5287 2023-05-28 18:49:27.000000 raspauto-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:49:39.519830 raspauto-0.3.0/raspauto/
+-rw-r--r--   0 runner    (1001) docker     (123)    19113 2023-05-28 18:49:27.000000 raspauto-0.3.0/raspauto/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:49:39.519830 raspauto-0.3.0/raspauto.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5691 2023-05-28 18:49:39.000000 raspauto-0.3.0/raspauto.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-28 18:49:39.000000 raspauto-0.3.0/raspauto.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 18:49:39.000000 raspauto-0.3.0/raspauto.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-28 18:49:39.000000 raspauto-0.3.0/raspauto.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-28 18:49:39.000000 raspauto-0.3.0/raspauto.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-28 18:49:39.523830 raspauto-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-05-28 18:49:27.000000 raspauto-0.3.0/setup.py
```

### Comparing `raspauto-0.2.2.9/LICENSE` & `raspauto-0.3.0/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-                    GNU AFFERO GENERAL PUBLIC LICENSE
+""                   GNU AFFERO GENERAL PUBLIC LICENSE
                        Version 3, 19 November 2007
 
  Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
  Everyone is permitted to copy and distribute verbatim copies
  of this license document, but changing it is not allowed.
 
                             Preamble
```

### Comparing `raspauto-0.2.2.9/PKG-INFO` & `raspauto-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: raspauto
-Version: 0.2.2.9
+Version: 0.3.0
 Summary: Raspberry Automation Library and Voice Recognition
 Home-page: https://github.com/aattk/raspauto
+Download-URL: https://pypi.org/project/raspauto/
 Author: Alpaslan Tetik
 Author-email: 232arslan104@gmail.com
 License: GNU
-Download-URL: https://pypi.org/project/raspauto/
 Keywords: raspberry,automotion,control
-Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Raspauto
 ### Remote management for smart technologies
 
@@ -51,16 +50,16 @@
 ```
 sudo pip3 install raspauto
 ```
 
 Create a python file and write the code at the bottom
 
 ``` python
-import raspauto
-ra = raspauto.set("telegram_bot_token","bot_password")
+import raspauto as ra
+ra.set("telegram_bot_token","bot_password")
 ```
 **Bot Password** : You set the secret password for bot usage.
 
 **Remember**     : You must send the password you set for the first use in plain text.
 
 If there is an error in activating or deactivating the button, please give permission to write to the database with the help of the command at the bottom.
 
@@ -95,14 +94,15 @@
 sudo reboot
 ```
 
 ## Telegram Bot Commands
 |Command|Function|Usage|
 |-|-|-|
 |Every key press|It sends the defined pin lists as a button.|-|
+|/login|Allows the user to log in.|``/login your_password``|
 |/start|It sends the defined pin lists as a button.|``/start``|
 |/pinadd|Adds pin information to the system|``/pinadd pin_name pin_number``|
 |/pinlist|It shows the pin information attached to the system.|``/pinlist``|
 |/userlist|It shows the user information attached to the system.|``/userlist``|
 |/pindelete|Starts the Pin Delete process.|``/pindelete``|
 |/userdelete|Starts the User Delete process.|``/userdelete``|
 |/rename|Used to name the user.|``/rename name``|
@@ -144,9 +144,7 @@
 - Telegram Button Usage Added.
 - Adding users via Telegram 
 - User delete via Telegram 
 - Added adding pin via Telegram
 - Added delete pin via Telegram
 #### version 0.1.6.5
 - Firebase support has been replaced by Telegram.
-
-
```

### Comparing `raspauto-0.2.2.9/README.md` & `raspauto-0.3.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -36,16 +36,16 @@
 ```
 sudo pip3 install raspauto
 ```
 
 Create a python file and write the code at the bottom
 
 ``` python
-import raspauto
-ra = raspauto.set("telegram_bot_token","bot_password")
+import raspauto as ra
+ra.set("telegram_bot_token","bot_password")
 ```
 **Bot Password** : You set the secret password for bot usage.
 
 **Remember**     : You must send the password you set for the first use in plain text.
 
 If there is an error in activating or deactivating the button, please give permission to write to the database with the help of the command at the bottom.
 
@@ -80,14 +80,15 @@
 sudo reboot
 ```
 
 ## Telegram Bot Commands
 |Command|Function|Usage|
 |-|-|-|
 |Every key press|It sends the defined pin lists as a button.|-|
+|/login|Allows the user to log in.|``/login your_password``|
 |/start|It sends the defined pin lists as a button.|``/start``|
 |/pinadd|Adds pin information to the system|``/pinadd pin_name pin_number``|
 |/pinlist|It shows the pin information attached to the system.|``/pinlist``|
 |/userlist|It shows the user information attached to the system.|``/userlist``|
 |/pindelete|Starts the Pin Delete process.|``/pindelete``|
 |/userdelete|Starts the User Delete process.|``/userdelete``|
 |/rename|Used to name the user.|``/rename name``|
```

### Comparing `raspauto-0.2.2.9/raspauto/__init__.py` & `raspauto-0.3.0/raspauto/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,174 +1,187 @@
 # -*- coding: utf-8 -*-
-import time
 import os
+import sqlite3 as sql
 import subprocess
+import time
 from threading import Thread
-import telegram
-import sqlite3 as sql
+
+import speech_recognition as sr
+from gtts import gTTS
 
 try:
-    import RPi.GPIO as GPIO
     import picamera
+    import RPi.GPIO as GPIO
 except Exception as e:
     print("GPIO Library not found.")
 
-from telegram import InlineKeyboardButton, InlineKeyboardMarkup
-from telegram.ext import Updater, CommandHandler, CallbackQueryHandler, MessageHandler, Filters
 
+from telegram import InlineKeyboardButton, InlineKeyboardMarkup, Update
+from telegram.ext import Application, CallbackQueryHandler, CommandHandler, ContextTypes, filters, MessageHandler, Updater
 
-# try:
-#     HOGCV = cv2.HOGDescriptor()
-#     HOGCV.setSVMDetector(cv2.HOGDescriptor_getDefaultPeopleDetector())
-# except Exception as e:
-#     print("OpenCV Library not found.")
 
 class set:
     def __init__(self, telegram_id, password):
         self.tid = telegram_id
         self.password = password
         self.pins = []
         self.awatch = False
+        self.asistan_state = True
         self.aupdate = []
         self.acontext = []
+        self.loginErrortext = "You are not logged in. Please login with /login <password> command."
         self.dbinit()
         self.pinKeyboardUpdate(1)
         self.updateInit()
-        
+        self.asistan()
 
     def updateInit(self):
-        updater = Updater(self.tid, use_context=True)
-        updater.dispatcher.add_handler(CommandHandler('start', self.start))
-        updater.dispatcher.add_handler(CommandHandler('pinadd', self.pinadd))
-        updater.dispatcher.add_handler(CommandHandler('pinlist', self.pin_list))
-        updater.dispatcher.add_handler(CommandHandler('pindelete', self.pinDelete))
-        updater.dispatcher.add_handler(CommandHandler('userdelete', self.user_delete))
-        updater.dispatcher.add_handler(CommandHandler('userlist', self.userList))
-        updater.dispatcher.add_handler(CommandHandler('rename', self.rename))
-        # updater.dispatcher.add_handler(CommandHandler('pinset', pinset))
-        updater.dispatcher.add_handler(CommandHandler('restart', self.restart))
-        updater.dispatcher.add_handler(CommandHandler('photo', self.photo))
-        updater.dispatcher.add_handler(CommandHandler('alarmstart', self.alarmstart))
-        updater.dispatcher.add_handler(CommandHandler('alarmstop', self.alarmstop))
-        updater.dispatcher.add_handler(CommandHandler('temp',self.temp))
-        updater.dispatcher.add_handler(CommandHandler('code', self.code))
-        updater.dispatcher.add_handler(CommandHandler('commands', self.commands))
-        updater.dispatcher.add_handler(CommandHandler('libupdate', self.libupdate))
-        updater.dispatcher.add_handler(CommandHandler('alwayswatch', self.alwayswatch))
-        updater.dispatcher.add_handler(CallbackQueryHandler(self.button))
-        updater.dispatcher.add_handler(CommandHandler('help',self.help_command))
-        updater.dispatcher.add_handler(MessageHandler(Filters.text & ~Filters.command, self.emsg))
-        updater.start_polling()
-        updater.idle()
+        """Run the bot."""
+        # Create the Application and pass it your bot's token.
+        application = Application.builder().token(self.tid).build()
+
+        application.add_handler(CommandHandler("start", self.start))
+        application.add_handler(CommandHandler("pinadd", self.pinadd))
+        application.add_handler(CommandHandler("pinlist", self.pin_list))
+        application.add_handler(CommandHandler("pindelete", self.pinDelete))
+        application.add_handler(CommandHandler("userdelete", self.user_delete))
+        application.add_handler(CommandHandler("userlist", self.userList))
+        application.add_handler(CommandHandler("rename", self.rename))
+        application.add_handler(CommandHandler("restart", self.restart))
+        application.add_handler(CommandHandler("photo", self.photo))
+        application.add_handler(CommandHandler("alarmstart", self.alarmstart))
+        application.add_handler(CommandHandler("alarmstop", self.alarmstop))
+        application.add_handler(CommandHandler("temp", self.temp))
+        application.add_handler(CommandHandler("code", self.code))
+        application.add_handler(CommandHandler("commands", self.commands))
+        application.add_handler(CommandHandler("libupdate", self.libupdate))
+        application.add_handler(CommandHandler("asistan", self.asistan))
+        application.add_handler(CommandHandler("login", self.login))
+        application.add_handler(CommandHandler(
+            "asistan_stop", self.asistan_stop))
+        application.add_handler(CommandHandler(
+            "alwayswatch", self.alwayswatch))
+        application.add_handler(CommandHandler("help", self.help_command))
+        application.add_handler(MessageHandler(
+            filters.TEXT & ~filters.COMMAND, self.emsg))
+
+        # Run the bot until the user presses Ctrl-C
+        application.run_polling()
 
     def dbinit(self):
         if(not os.path.isfile("ra.sqlite")):
             db = sql.connect('ra.sqlite')
             im = db.cursor()
             im.execute("CREATE TABLE users (id, name)")
             im.execute("CREATE TABLE pins (id,name,state)")
             im.execute("CREATE TABLE alarm (id,state)")
             im.execute("CREATE TABLE language (lcode,data)")
 
-    def saveUser(self,id,name):
+    def saveUser(self, id, name):
         db = sql.connect('ra.sqlite')
         im = db.cursor()
         im.execute("INSERT INTO users VALUES ('"+str(id)+"', '"+name+"')")
         db.commit()
         db.close()
 
     def readUsers(self):
         db = sql.connect('ra.sqlite')
         im = db.cursor()
         im.execute("SELECT * FROM users")
         data = im.fetchall()
         db.close()
         return data
 
-    def renameUser(self,id,name):
+    def renameUser(self, id, name):
         db = sql.connect('ra.sqlite')
         im = db.cursor()
         im.execute("UPDATE users SET name = '"+name+"' WHERE id='"+str(id)+"'")
         db.commit()
         db.close()
 
-    def isLogin(self,id):
+    def isLogin(self, id):
         db = sql.connect('ra.sqlite')
         im = db.cursor()
         im.execute("SELECT * FROM users where id = '"+str(id)+"'")
         data = im.fetchall()
         db.close()
         if len(data) > 0:
             return True
         else:
             return False
-    
-    def savePin(self,data):
+
+    def savePin(self, data):
         data = data.split(" ")
         if len(data) > 1:
             db = sql.connect('ra.sqlite')
             im = db.cursor()
-            im.execute("INSERT INTO pins VALUES ('"+str(data[2])+"', '"+str(data[1])+"','F')")
+            im.execute("INSERT INTO pins VALUES ('" +
+                       str(data[2])+"', '"+str(data[1])+"','F')")
             db.commit()
             db.close()
             return True
-        else: 
+        else:
             return False
 
-    def deletePin(self,id,query):
+    def deletePin(self, id, query):
         db = sql.connect('ra.sqlite')
         im = db.cursor()
         im.execute("SELECT * FROM pins where id = '"+str(id)+"'")
         data = im.fetchone()
         im.execute("DELETE FROM pins WHERE id = '"+str(id)+"'")
-        query.edit_message_text(text= data[1] + " deleted.".format(query.data))
+        query.edit_message_text(text=data[1] + " deleted.".format(query.data))
         db.commit()
         db.close()
 
-    def deleteUser(self,id,query):
+    def deleteUser(self, id, query):
         db = sql.connect('ra.sqlite')
         im = db.cursor()
         im.execute("SELECT * FROM users where id = '"+str(id)+"'")
         data = im.fetchone()
         im.execute("DELETE FROM users WHERE id = '"+str(id)+"'")
-        query.edit_message_text(text= data[1] + " deleted.".format(query.data))
+        query.edit_message_text(text=data[1] + " deleted.".format(query.data))
         db.commit()
         db.close()
 
-    def updatePinState(self,id,query):
+    def updatePinState(self, id, query):
         db = sql.connect('ra.sqlite')
         im = db.cursor()
         im.execute("SELECT * FROM pins where id = '"+str(id)+"'")
         data = im.fetchone()
         stt = ""
         if (data[2] == 'F'):
             stt = "T"
             try:
                 GPIO.output(int(data[0]), GPIO.HIGH)
-                query.edit_message_text(text=data[1] + " opened.".format(query.data))
+                query.edit_message_text(
+                    text=data[1] + " opened.".format(query.data))
             except Exception as e:
                 print("GPIO Set Error")
-                query.edit_message_text("Something went wrong.".format(query.data))
+                query.edit_message_text(
+                    "Something went wrong.".format(query.data))
         elif (data[2] == 'T'):
             stt = "F"
             try:
                 GPIO.output(int(data[0]), GPIO.LOW)
-                query.edit_message_text(text=data[1] + " closed.".format(query.data))
-                im.execute("UPDATE pins SET state = '"+stt+"' WHERE id='"+str(id)+"'")
+                query.edit_message_text(
+                    text=data[1] + " closed.".format(query.data))
+                im.execute("UPDATE pins SET state = '" +
+                           stt+"' WHERE id='"+str(id)+"'")
             except Exception as e:
                 print("GPIO Set Error")
-                query.edit_message_text("Something went wrong.".format(query.data))
+                query.edit_message_text(
+                    "Something went wrong.".format(query.data))
         try:
-            im.execute("UPDATE pins SET state = '"+stt+"' WHERE id='"+str(id)+"'")
+            im.execute("UPDATE pins SET state = '" +
+                       stt+"' WHERE id='"+str(id)+"'")
         except Exception as e:
             print("Save Database Error ! ")
         db.commit()
         db.close()
-            
-    
+
     def readPins(self):
         db = sql.connect('ra.sqlite')
         im = db.cursor()
         im.execute("SELECT * FROM pins")
         data = im.fetchall()
         db.close()
         try:
@@ -177,239 +190,285 @@
             GPIO.setmode(GPIO.BOARD)
             for i in data:
                 GPIO.setup(int(i[0]), GPIO.OUT)
                 if (i[2] == 'T'):
                     GPIO.output(int(i[0]), GPIO.HIGH)
                 else:
                     GPIO.output(int(i[0]), GPIO.LOW)
-        except Exception  as e:
+        except Exception as e:
             print(e)
         return data
 
-    def pinKeyboardUpdate(self,id):
+    def pinKeyboardUpdate(self, id):
         i_counter = 0
         pin_temp = []
         self.pins = []
-        dpin  = self.readPins()
+        dpin = self.readPins()
         for pin in dpin:
-            pin_temp = pin_temp + [InlineKeyboardButton(pin[1], callback_data= str(id) +"#"+pin[0])]
+            pin_temp = pin_temp + \
+                [InlineKeyboardButton(
+                    pin[1], callback_data=str(id) + "#"+pin[0])]
             i_counter += 1
             if i_counter == 3:
                 self.pins = self.pins + [pin_temp]
                 pin_temp = []
                 i_counter = 0
             elif pin == dpin[-1]:
                 self.pins = self.pins + [pin_temp]
                 pin_temp = []
                 i_counter = 0
-    
-    def userKeyboardUpdate(self,id):
+
+    def userKeyboardUpdate(self, id):
         i_counter = 0
         pin_temp = []
         self.users = []
-        dpin  = self.readUsers()
+        dpin = self.readUsers()
         for pin in dpin:
-            pin_temp = pin_temp + [InlineKeyboardButton(pin[1] +" / "+ pin[0], callback_data= str(id) +"#"+pin[0])]
+            pin_temp = pin_temp + \
+                [InlineKeyboardButton(
+                    pin[1] + " / " + pin[0], callback_data=str(id) + "#"+pin[0])]
             i_counter += 1
             if i_counter == 2:
                 self.users = self.users + [pin_temp]
                 pin_temp = []
                 i_counter = 0
             elif pin == dpin[-1]:
                 self.users = self.users + [pin_temp]
                 pin_temp = []
                 i_counter = 0
 
-    # def detect(self,frame):
-    #     bounding_box_cordinates, weights =  HOGCV.detectMultiScale(frame, winStride = (4, 4), padding = (8, 8), scale = 1.03)
-        
-    #     person = 1
-    #     for x,y,w,h in bounding_box_cordinates:
-    #         cv2.rectangle(frame, (x,y), (x+w,y+h), (0,255,0), 2)
-    #         cv2.putText(frame, f'person {person}', (x,y), cv2.FONT_HERSHEY_SIMPLEX, 0.5, (0,0,255), 1)
-    #         person += 1
-    #     self.alarmpeople.message.reply_text('Please choose:')
-    #     cv2.putText(frame, 'Status : Detecting ', (40,40), cv2.FONT_HERSHEY_DUPLEX, 0.8, (255,0,0), 2)
-    #     cv2.putText(frame, f'Total Persons : {person-1}', (40,70), cv2.FONT_HERSHEY_DUPLEX, 0.8, (255,0,0), 2)
-    #     cv2.imshow('output', frame)
-    #     return frame
-
-    # def peopleTracer(self):
-    #     video = cv2.VideoCapture(0)
-    #     while self.alarm:
-    #         try:
-    #             print('Detecting people...')
-    #             check, frame = video.read()
-    #             frame = detect(frame)
-    #             cv2.imshow("Frame",frame)
-    #             key = cv2.waitKey(1)
-    #             if key == ord('q'):
-    #                 break
-            
-    #         except Exception as e:
-    #             pass
-    #     video.release()
-    #     cv2.destroyAllWindows()
-
-    def start(self,update, context):
-        if self.login(update, context):
+    async def start(self, update: Update, context: ContextTypes.DEFAULT_TYPE) -> None:
+        if self.isLogin(update.effective_chat.id):
             self.pinKeyboardUpdate(1)
             keyboard = self.pins
             reply_markup = InlineKeyboardMarkup(keyboard)
-            update.message.reply_text(
+            await update.message.reply_text(
                 'Please choose:', reply_markup=reply_markup)
+        else:
+            await update.message.reply_text(self.loginErrortext)
 
-    def emsg(self,update, context):
-        if self.login(update, context):
+    async def emsg(self, update: Update, context: ContextTypes.DEFAULT_TYPE) -> None:
+        if self.isLogin(update.effective_chat.id):
             msg = update.message.text
             if len(msg) == 1:
                 self.pinKeyboardUpdate(1)
                 keyboard = self.pins
                 reply_markup = InlineKeyboardMarkup(keyboard)
-                update.message.reply_text(
+                await update.message.reply_text(
                     'Please choose:', reply_markup=reply_markup)
+        else:
+            await update.message.reply_text(self.loginErrortext)
 
-    def login(self,update, context):
+    async def login(self, update: Update, context: ContextTypes.DEFAULT_TYPE) -> None:
         if self.isLogin(update.effective_chat.id):
             return True
-        elif self.password == update.message.text:
-            self.saveUser(update.effective_chat.id,"-")
-            update.message.reply_text("Login Succesfully")
+        elif self.password == update.message.text.split(" ")[1]:
+            self.saveUser(update.effective_chat.id, "-")
+            await update.message.reply_text("Login Succesfully")
             return True
         else:
-            update.message.reply_text("Wrong Password")
-            update.message.reply_text("Try Again")
+            await update.message.reply_text("Wrong Password")
+            await update.message.reply_text("Try Again")
             return False
 
-    def button(self,update, context):
-        if self.login(update, context):
+    async def button(self, update: Update, context: ContextTypes.DEFAULT_TYPE) -> None:
+        if self.isLogin(update.effective_chat.id):
             query = update.callback_query
-            query.answer() # str(query.data)
+            query.answer()  # str(query.data)
             aa = query.data.split("#")
             if (aa[0] == "1"):
-                self.updatePinState(aa[1],query)
+                self.updatePinState(aa[1], query)
             elif (aa[0] == "2"):
-                self.deletePin(aa[1],query)
+                self.deletePin(aa[1], query)
             elif (aa[0] == "3"):
-                self.deleteUser(aa[1],query)
+                self.deleteUser(aa[1], query)
 
-    def help_command(self,update, context):
-        update.message.reply_text("Creator: Alpaslan Tetik\nhttps://t.me/raspauto")
+    async def help_command(self, update: Update, context: ContextTypes.DEFAULT_TYPE) -> None:
+        await update.message.reply_text(
+            "Creator: Alpaslan Tetik\nhttps://t.me/raspauto")
 
-    def commands(self,update, context):
-        update.message.reply_text("https://github.com/aattk/raspauto#telegram-bot-commands")
+    async def commands(self, update: Update, context: ContextTypes.DEFAULT_TYPE) -> None:
+        await update.message.reply_text(
+            "https://github.com/aattk/raspauto#telegram-bot-commands")
 
-    def restart(self,update, context):
-        if self.login(update, context):
+    async def restart(self, update: Update, context: ContextTypes.DEFAULT_TYPE) -> None:
+        if self.isLogin(update.effective_chat.id):
             try:
                 GPIO.cleanup()
-                update.message.reply_text("Reboot Now")
+                await update.message.reply_text("Reboot Now")
                 os.system("reboot")
             except Exception as e:
                 print("All Pins Cleaned.")
 
-    def temp(self,update, context):
-        if self.login(update, context):
+    async def temp(self, update: Update, context: ContextTypes.DEFAULT_TYPE) -> None:
+        if self.isLogin(update.effective_chat.id):
             try:
-                data = subprocess.check_output('/opt/vc/bin/vcgencmd measure_temp', shell=True)
-                update.message.reply_text(str(data)[2:13])
+                data = subprocess.check_output(
+                    '/opt/vc/bin/vcgencmd measure_temp', shell=True)
+                await update.message.reply_text(str(data)[2:13])
             except Exception as e:
                 print("Error temp Function")
-                update.message.reply_text("Temp Error")
+                await update.message.reply_text("Temp Error")
+        else:
+            await update.message.reply_text(self.loginErrortext)
 
-    def libupdate(self,update, context):
-        if self.login(update, context):
+    async def libupdate(self, update: Update, context: ContextTypes.DEFAULT_TYPE) -> None:
+        if self.isLogin(update.effective_chat.id):
             try:
-                direct_output = subprocess.check_output('pip3 install raspauto --upgrade', shell=True)
-                update.message.reply_text(direct_output.decode('utf-8'))
-                update.message.reply_text("Please Reboot /restart")
+                direct_output = subprocess.check_output(
+                    'pip3 install raspauto --upgrade', shell=True)
+                await update.message.reply_text(direct_output.decode('utf-8'))
+                await update.message.reply_text("Please Reboot /restart")
             except Exception as e:
                 print("Error Update Function")
-                update.message.reply_text("Something went wrong.")
+                await update.message.reply_text("Something went wrong.")
+        else:
+            await update.message.reply_text(self.loginErrortext)
 
-    def pinadd(self,update, context):
-        if self.login(update, context):
+    async def pinadd(self, update: Update, context: ContextTypes.DEFAULT_TYPE) -> None:
+        if self.isLogin(update.effective_chat.id):
             if self.savePin(update.message.text):
-                update.message.reply_text("Successfully added")
+                await update.message.reply_text("Successfully added")
             else:
-                update.message.reply_text("Something went wrong.")
-                update.message.reply_text("Example Usage:")
-                update.message.reply_text("/pinadd kitchen 12")
+                await update.message.reply_text("Something went wrong.")
+                await update.message.reply_text("Example Usage:")
+                await update.message.reply_text("/pinadd kitchen 12")
+        else:
+            await update.message.reply_text(self.loginErrortext)
 
-    def code(self,update, context):
-        if self.login(update, context):
+    async def code(self, update: Update, context: ContextTypes.DEFAULT_TYPE) -> None:
+        if self.isLogin(update.effective_chat.id):
             cd = update.message.text
             cd = cd[6:]
             try:
                 data = subprocess.check_output(str(cd), shell=True)
                 update.message.reply_text(data.decode('utf-8'))
             except Exception as e:
                 print("Code Run Error")
-                update.message.reply_text("Code Run Error")
+                await update.message.reply_text("Code Run Error")
+        else:
+            await update.message.reply_text(self.loginErrortext)
 
-    def pin_list(self,update, context):
-        if self.login(update, context):
+    async def pin_list(self, update: Update, context: ContextTypes.DEFAULT_TYPE) -> None:
+        if self.isLogin(update.effective_chat.id):
             data = ""
             for i in self.readPins():
-                data = data +"Name           : " + i[1] + "\nPin Number : "+ i[0] + "\n-----------------------------------------\n" 
-            update.message.reply_text("# Defined Pin List\n-----------------------------------------\n"+data)
-    
-    def userList(self,update, context):
-        if self.login(update, context):
+                data = data + "Name           : " + \
+                    i[1] + "\nPin Number : " + i[0] + \
+                    "\n-----------------------------------------\n"
+            await update.message.reply_text("# Defined Pin List\n-----------------------------------------\n"+data)
+        else:
+            await update.message.reply_text(self.loginErrortext)
+
+    async def userList(self, update: Update, context: ContextTypes.DEFAULT_TYPE) -> None:
+        if self.isLogin(update.effective_chat.id):
             data = ""
             for i in self.readUsers():
-                data = data +"Name             : " + i[1] + "\nUser Number : "+ i[0] + "\n-----------------------------------------\n" 
-            update.message.reply_text("# User List\n-----------------------------------------\n"+data)
+                data = data + "Name             : " + \
+                    i[1] + "\nUser Number : " + i[0] + \
+                    "\n-----------------------------------------\n"
+            await update.message.reply_text(
+                "# User List\n-----------------------------------------\n"+data)
+        else:
+            await update.message.reply_text(self.loginErrortext)
 
-    def pinDelete(self,update, context):
-        if self.login(update, context):
+    async def pinDelete(self, update: Update, context: ContextTypes.DEFAULT_TYPE) -> None:
+        if self.isLogin(update.effective_chat.id):
             self.pinKeyboardUpdate(2)
             keyboard = self.pins
             reply_markup = InlineKeyboardMarkup(keyboard)
-            update.message.reply_text('Please choose:', reply_markup=reply_markup)
-            update.message.reply_text("Select the pin to do the deletion.")
+            await update.message.reply_text(
+                'Please choose:', reply_markup=reply_markup)
+            await update.message.reply_text("Select the pin to do the deletion.")
+        else:
+            await update.message.reply_text(self.loginErrortext)
 
-    def user_delete(self,update, context):
-        if self.login(update, context):
+    async def user_delete(self, update: Update, context: ContextTypes.DEFAULT_TYPE) -> None:
+        if self.isLogin(update.effective_chat.id):
             self.userKeyboardUpdate(3)
             keyboard = self.users
             reply_markup = InlineKeyboardMarkup(keyboard)
-            update.message.reply_text('Please choose:', reply_markup=reply_markup)
-            update.message.reply_text("Select the user to do the deletion.")
-    
-    def rename(self,update, context):
-        if self.login(update,context):
-            self.renameUser(update.effective_chat.id,update.message.text.split(" ")[1])
-            update.message.reply_text("Renaming is successful.")
+            await update.message.reply_text(
+                'Please choose:', reply_markup=reply_markup)
+            await update.message.reply_text("Select the user to do the deletion.")
+        else:
+            await update.message.reply_text(self.loginErrortext)
+
+    async def rename(self, update: Update, context: ContextTypes.DEFAULT_TYPE) -> None:
+        if self.isLogin(update.effective_chat.id):
+            self.renameUser(update.effective_chat.id,
+                            update.message.text.split(" ")[1])
+            await update.message.reply_text("Renaming is successful.")
+        else:
+            await update.message.reply_text(self.loginErrortext)
 
-    def photo(self,update, context):
-        if self.login(update, context):
+    async def photo(self, update: Update, context: ContextTypes.DEFAULT_TYPE) -> None:
+        if self.isLogin(update.effective_chat.id):
             with picamera.PiCamera() as camera:
                 camera.start_preview()
                 time.sleep(4)
                 camera.capture('raspauto.jpg')
                 camera.stop_preview()
             time.sleep(2)
-            update.message.reply_photo(photo=open('raspauto.jpg', 'rb'), timeout=240)
-    
-    def alarmstart(self,update,context):
+            await update.message.reply_photo(photo=open(
+                'raspauto.jpg', 'rb'), timeout=240)
+        else:
+            await update.message.reply_text(self.loginErrortext)
+
+    async def alarmstart(self, update: Update, context: ContextTypes.DEFAULT_TYPE) -> None:
         self.alarm = True
         self.alarmpeople = update
-        Thread(target = self.peopleTracer).start()
+        Thread(target=self.peopleTracer).start()
 
-    def alarmstop(self,update,context):
+    async def alarmstop(self, update: Update, context: ContextTypes.DEFAULT_TYPE) -> None:
         self.alarm = False
 
-    def alwayswatch(self,update,context):
+    async def alwayswatch(self, update: Update, context: ContextTypes.DEFAULT_TYPE) -> None:
         self.awatch = ~self.awatch
-        self.aupdate = update;
-        self.acontext = context;        
-        self.alwaysphoto(self.aupdate,self.acontext)
-        update.message.reply_text(f"Always Watch {self.awatch}")
+        self.aupdate = update
+        self.acontext = context
+        self.alwaysphoto(self.aupdate, self.acontext)
+        await update.message.reply_text(f"Always Watch {self.awatch}")
 
-    def alwaysphoto(self,update,context):
+    async def alwaysphoto(self, update: Update, context: ContextTypes.DEFAULT_TYPE) -> None:
         try:
-            while self.awatch:  
-                self.photo(self.aupdate,self.acontext)
+            while self.awatch:
+                self.photo(self.aupdate, self.acontext)
                 print("Fotograf Gonderildi.")
         except Exception as e:
-            print(f"Bir hata olsutu. {e}")
+            print(f"Bir hata olsutu. {e}")
+
+    def speak(self, message):
+        tts = gTTS(text=message, lang='tr')
+        tts.save("audio.mp3")
+        os.system("audio.mp3")
+
+    def recordAudio(self):
+        r = sr.Recognizer()
+        with sr.Microphone() as source:
+            print("Say something!")
+            audio = r.listen(source)
+        data = ""
+        try:
+            data = r.recognize_google(audio, language='tr-tr')
+            data = data.lower()
+        except sr.UnknownValueError:
+            print("Google Speech Recognition could not understand audio")
+        return data
+
+    async def asistan(self, update: Update, context: ContextTypes.DEFAULT_TYPE) -> None:
+        while(self.asistan_state):
+            data = self.recordAudio()
+            self.komut_olustur(data)
+        self.asistan_state = True
+
+    async def asistan_stop(self, update: Update, context: ContextTypes.DEFAULT_TYPE) -> None:
+        self.asistan_state = False
+        await update.message.reply_text(f"Assistant turned off.")
+
+    def komut_olustur(self, data):
+        for i in self.readPins():
+            if i[1].lower() in data:
+                if "aç" in data:
+                    self.speak(f"{i[1]} açıldı.")
+                elif "kapat" in data:
+                    self.speak(f"{i[1]} kapatıldı.")
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `raspauto-0.2.2.9/raspauto.egg-info/PKG-INFO` & `raspauto-0.3.0/raspauto.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: raspauto
-Version: 0.2.2.9
+Version: 0.3.0
 Summary: Raspberry Automation Library and Voice Recognition
 Home-page: https://github.com/aattk/raspauto
+Download-URL: https://pypi.org/project/raspauto/
 Author: Alpaslan Tetik
 Author-email: 232arslan104@gmail.com
 License: GNU
-Download-URL: https://pypi.org/project/raspauto/
 Keywords: raspberry,automotion,control
-Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Raspauto
 ### Remote management for smart technologies
 
@@ -51,16 +50,16 @@
 ```
 sudo pip3 install raspauto
 ```
 
 Create a python file and write the code at the bottom
 
 ``` python
-import raspauto
-ra = raspauto.set("telegram_bot_token","bot_password")
+import raspauto as ra
+ra.set("telegram_bot_token","bot_password")
 ```
 **Bot Password** : You set the secret password for bot usage.
 
 **Remember**     : You must send the password you set for the first use in plain text.
 
 If there is an error in activating or deactivating the button, please give permission to write to the database with the help of the command at the bottom.
 
@@ -95,14 +94,15 @@
 sudo reboot
 ```
 
 ## Telegram Bot Commands
 |Command|Function|Usage|
 |-|-|-|
 |Every key press|It sends the defined pin lists as a button.|-|
+|/login|Allows the user to log in.|``/login your_password``|
 |/start|It sends the defined pin lists as a button.|``/start``|
 |/pinadd|Adds pin information to the system|``/pinadd pin_name pin_number``|
 |/pinlist|It shows the pin information attached to the system.|``/pinlist``|
 |/userlist|It shows the user information attached to the system.|``/userlist``|
 |/pindelete|Starts the Pin Delete process.|``/pindelete``|
 |/userdelete|Starts the User Delete process.|``/userdelete``|
 |/rename|Used to name the user.|``/rename name``|
@@ -144,9 +144,7 @@
 - Telegram Button Usage Added.
 - Adding users via Telegram 
 - User delete via Telegram 
 - Added adding pin via Telegram
 - Added delete pin via Telegram
 #### version 0.1.6.5
 - Firebase support has been replaced by Telegram.
-
-
```

### Comparing `raspauto-0.2.2.9/setup.py` & `raspauto-0.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open('README.md') as readme_file:
     README = readme_file.read()
 
 
 setup_args = dict(
     name='raspauto',
-    version='0.2.2.9',
+    version='0.3.0',
     description='Raspberry Automation Library and Voice Recognition',
     long_description_content_type="text/markdown",
     long_description=README,
     license='GNU',
     packages=find_packages(),
     author='Alpaslan Tetik',
     author_email='232arslan104@gmail.com',
```

