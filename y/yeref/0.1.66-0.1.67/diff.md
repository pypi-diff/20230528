# Comparing `tmp/yeref-0.1.66.tar.gz` & `tmp/yeref-0.1.67.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yeref-0.1.66.tar", last modified: Fri May 26 17:59:17 2023, max compression
+gzip compressed data, was "yeref-0.1.67.tar", last modified: Sun May 28 15:01:58 2023, max compression
```

## Comparing `yeref-0.1.66.tar` & `yeref-0.1.67.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-05-26 17:59:17.559635 yeref-0.1.66/
--rw-r--r--   0 mark       (501) staff       (20)       85 2023-05-26 17:59:17.559863 yeref-0.1.66/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)       38 2023-05-26 17:59:17.562327 yeref-0.1.66/setup.cfg
--rw-r--r--   0 mark       (501) staff       (20)     1351 2023-05-26 17:59:04.000000 yeref-0.1.66/setup.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-05-26 17:59:17.552749 yeref-0.1.66/yeref/
--rw-r--r--   0 mark       (501) staff       (20)       39 2023-04-21 17:52:00.000000 yeref-0.1.66/yeref/__init__.py
--rw-r--r--   0 mark       (501) staff       (20)   489150 2023-05-26 17:58:09.000000 yeref-0.1.66/yeref/l_.py
--rw-r--r--   0 mark       (501) staff       (20)   204673 2023-05-25 18:35:58.000000 yeref-0.1.66/yeref/yeref.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-05-26 17:59:17.559029 yeref-0.1.66/yeref.egg-info/
--rw-r--r--   0 mark       (501) staff       (20)       85 2023-05-26 17:59:17.000000 yeref-0.1.66/yeref.egg-info/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)      179 2023-05-26 17:59:17.000000 yeref-0.1.66/yeref.egg-info/SOURCES.txt
--rw-r--r--   0 mark       (501) staff       (20)        1 2023-05-26 17:59:17.000000 yeref-0.1.66/yeref.egg-info/dependency_links.txt
--rw-r--r--   0 mark       (501) staff       (20)        6 2023-05-26 17:59:17.000000 yeref-0.1.66/yeref.egg-info/top_level.txt
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-05-28 15:01:58.185911 yeref-0.1.67/
+-rw-r--r--   0 mark       (501) staff       (20)       85 2023-05-28 15:01:58.186205 yeref-0.1.67/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)       38 2023-05-28 15:01:58.187826 yeref-0.1.67/setup.cfg
+-rw-r--r--   0 mark       (501) staff       (20)     1351 2023-05-28 15:01:46.000000 yeref-0.1.67/setup.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-05-28 15:01:58.176803 yeref-0.1.67/yeref/
+-rw-r--r--   0 mark       (501) staff       (20)       39 2023-04-21 17:52:00.000000 yeref-0.1.67/yeref/__init__.py
+-rw-r--r--   0 mark       (501) staff       (20)   489139 2023-05-27 17:27:42.000000 yeref-0.1.67/yeref/l_.py
+-rw-r--r--   0 mark       (501) staff       (20)   204736 2023-05-27 15:53:48.000000 yeref-0.1.67/yeref/yeref.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-05-28 15:01:58.185030 yeref-0.1.67/yeref.egg-info/
+-rw-r--r--   0 mark       (501) staff       (20)       85 2023-05-28 15:01:58.000000 yeref-0.1.67/yeref.egg-info/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)      179 2023-05-28 15:01:58.000000 yeref-0.1.67/yeref.egg-info/SOURCES.txt
+-rw-r--r--   0 mark       (501) staff       (20)        1 2023-05-28 15:01:58.000000 yeref-0.1.67/yeref.egg-info/dependency_links.txt
+-rw-r--r--   0 mark       (501) staff       (20)        6 2023-05-28 15:01:58.000000 yeref-0.1.67/yeref.egg-info/top_level.txt
```

### Comparing `yeref-0.1.66/setup.py` & `yeref-0.1.67/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
       name='yeref',
-      version='0.1.66',
+      version='0.1.67',
       description='desc-f',
       author='john smith',
       packages=['yeref'],
       # install_requires=[
       #       "httplib2>=0.20.4",
       #       "moviepy>=1.0.3",
       #       "Pillow>=9.2.0",
@@ -39,15 +39,15 @@
 # python setup.py bdist_wheel
 # endregion
 
 # python -m build
 
 # twine upload dist/*
 
-# python3 -m pip install --force-reinstall /Users/mark/PycharmProjects/AUTOBOT/yeref/dist/yeref-0.1.65-py3-none-any.whl
+# python3 -m pip install --force-reinstall /Users/mark/PycharmProjects/AUTOBOT/yeref/dist/yeref-0.1.66-py3-none-any.whl
 
 # python3 -m pip install --upgrade yeref
 
 # pip install --force-reinstall -v "yeref==0.1.30"
 # pip install https://github.com/aiogram/aiogram/archive/refs/heads/dev-3.x.zip
 # pip show aiogram
 # ARCHFLAGS="-arch x86_64" pip install pycurl
```

### Comparing `yeref-0.1.66/yeref/l_.py` & `yeref-0.1.67/yeref/l_.py`

 * *Files 0% similar despite different names*

```diff
@@ -2468,15 +2468,15 @@
     'en': "🔎 Unload the database by keywords <i>{0}</i> ..\n\n#duration 1 min",
     'es': "🔎 Descarga la base de datos por palabras clave <i>{0}</i> ..\n\n#duración 1 min",
     'fr': "🔎 Décharger la base de données par mots clés <i>{0}</i> ..\n\n#durée 1 min",
     'zh': "🔎 通过关键字<i>{0}</i>卸载数据库 ..\n\n#duration 1 分钟",
     'ar': "🔎 تفريغ قاعدة البيانات بالكلمات الأساسية <i>{0}</i> ..\n\n# المدة 1 دقيقة",
 }
 l_find_category_keywords = {
-    'ru': "📰 Введи ключевые слова для поиска через пробелы или разделители",
+    'ru': "📰 <b>Введи</b> ключевые слова для поиска через пробелы или разделители",
     'en': "📰 Enter keywords to search through spaces or delimiters",
     'es': "📰 Ingrese palabras clave para buscar a través de espacios o delimitadores",
     'fr': "📰 Entrez des mots-clés pour rechercher dans des espaces ou des délimiteurs",
     'zh': "📰 输入关键字以通过空格或分隔符进行搜索",
     'ar': "📰 أدخل كلمات أساسية للبحث من خلال المسافات أو المحددات",
 }
 l_find_reached = {
@@ -3415,23 +3415,23 @@
     'ar': "🔘️☐ تعطيل مكافحة الغارة",
 }
 # endregion
 
 
 # region cban_
 l_cban_add = {
-    'ru': "🕵🏽 Введи <code>id</code> или <code>@username</code> пользователей  через пробельные символы или разделители, чтобы добавить их в /ban-список (*даже тех, кого нет <u>{0}</u>-файле)\n\n👩🏽‍💻 Текущее число пользователей /ban-списка: <u>{1}</u>",
+    'ru': "🕵🏽 <b>Введи</b> <code>id</code> или <code>@username</code> пользователей  через пробельные символы или разделители, чтобы добавить их в /ban-список (*даже тех, кого нет <u>{0}</u>-файле)\n\n👩🏽‍💻 Текущее число пользователей /ban-списка: <u>{1}</u>",
     'en': "🗣 Push the ✅/☑️ to <b>On/Off</b> auto-transcribe (speach to text) for <i><b>income</b>/<b>outgoing</b> messages</i>",
     'es': "🗣 Presiona ✅/☑️ para <b>Encender/Apagar</b> <i>sistema</i> mensajes\n\n👩🏽‍💻 Por ejemplo, <i>Usuario se unió al grupo</i>",
     'fr': "🗣 Appuyez sur ✅/☑️ pour <b>Activer/Désactiver</b> les messages <i>système</i>\n\n👩🏽‍💻 Par exemple, <i>L'utilisateur a rejoint le bote</i>",
     'zh': "🗣 將 ✅/☑️ 推送到 <b>On/Off</b> <i>system</i> 消息\n\n👩🏽‍💻 例如，<i>用戶加入群組</i>",
     'ar': "👣 اضغط على ✅ / ☑️ ، إلى رسائل <b> تشغيل / إيقاف </b> <i> النظام </i>\n\n👩🏽‍💻 على سبيل المثال ، <i> انضم المستخدم إلى المجموعة </i>",
 }
 l_cban_remove = {
-    'ru': "🕵🏽 Введи <code>id</code> или <code>@username</code> пользователей из <u>{0}</u>-файла через пробельные символы или разделители, чтобы удалить их из /ban-списка\n\n👩🏽‍💻 Текущее число пользователей /ban-списка: <u>{1}</u>",
+    'ru': "🕵🏽 <b>Введи</b> <code>id</code> или <code>@username</code> пользователей из <u>{0}</u>-файла через пробельные символы или разделители, чтобы удалить их из /ban-списка\n\n👩🏽‍💻 Текущее число пользователей /ban-списка: <u>{1}</u>",
     'en': "🗣 Push the ✅/☑️ to <b>On/Off</b> auto-transcribe (speach to text) for <i><b>income</b>/<b>outgoing</b> messages</i>",
     'es': "🗣 Presiona ✅/☑️ para <b>Encender/Apagar</b> <i>sistema</i> mensajes\n\n👩🏽‍💻 Por ejemplo, <i>Usuario se unió al grupo</i>",
     'fr': "🗣 Appuyez sur ✅/☑️ pour <b>Activer/Désactiver</b> les messages <i>système</i>\n\n👩🏽‍💻 Par exemple, <i>L'utilisateur a rejoint le bote</i>",
     'zh': "🗣 將 ✅/☑️ 推送到 <b>On/Off</b> <i>system</i> 消息\n\n👩🏽‍💻 例如，<i>用戶加入群組</i>",
     'ar': "👣 اضغط على ✅ / ☑️ ، إلى رسائل <b> تشغيل / إيقاف </b> <i> النظام </i>\n\n👩🏽‍💻 على سبيل المثال ، <i> انضم المستخدم إلى المجموعة </i>",
 }
 l_cban_added = {
@@ -3607,15 +3607,15 @@
     'en': "\n\nIn the Settings [Administrators] for @{0} enable:\n[✅ Delete Msgs]\n[✅ Ban Users]\n[✅ Invite Users]\n🕚Wait for 1min",
     'es': "\n\nEn la Configuración [Administradores] para @{0} active:\n[✅ Eliminar mensajes]\n[✅ Prohibir usuarios]\n[✅ Invitar usuarios]\n🕚Espere 1 minuto",
     'fr': "\n\nDans les paramètres [Administrateurs] pour @{0}, activez :\n[✅ Supprimer les messages]\n[✅ Bannir les utilisateurs]\n[✅ Inviter des utilisateurs]\n🕚Attendez 1 minute",
     'zh': "\n\n在@{0}的設置[管理員]中打開：\n[✅刪除消息]\n[✅禁止用戶]\n[✅邀請用戶]\n🕚等待1分鐘",
     'ar': "\n\n في الإعدادات [Administrators] لـ @{0} شغّل:\n [✅ حذف الرسائل] \n على [✅ حظر المستخدمين] \n [✅ دعوة المستخدمين] \n وانتظر لمدة دقيقة واحدة",
 }
 l_creact_correct = {
-    'ru': "👍🏽 Введи корректное <b>число</b> креативных авто-реакций на последний пост канала\n\n👩🏽‍💻 Используй команду <code>/react {0}</code>, чтобы задать количество авто-реакций (<b>текущее</b> количество: <u>{0}</u>)",
+    'ru': "👍🏽 <b>Введи</b> корректное <b>число</b> креативных авто-реакций на последний пост канала\n\n👩🏽‍💻 Используй команду <code>/react {0}</code>, чтобы задать количество авто-реакций (<b>текущее</b> количество: <u>{0}</u>)",
     'en': "👍🏽 Ready! Current primary delay for <u>new</u> users (before writing their <u>1</u>st message) is <u>{0}</u> min",
     'es': "👍🏽 Listo! El retraso principal actual para los <u>nuevos</u> usuarios (antes de escribir su <u>1</u>er mensaje) es <u>{0}</u> min",
     'fr': "👍🏽 Prêt! Le délai principal actuel pour les <u>nouveaux</u> utilisateurs (avant d'écrire leur <u>1</u>er message) est de <u>{0}</u> min",
     'zh': "👍🏽 準備好了！<u>新</u>用戶的當前主要延遲（在寫他們的<u>1</u>st消息之前）是<u>{0}</u>分鐘",
     'ar': "👥 جاهز! التأخير الأساسي الحالي لمستخدمي <u> الجدد </u> (قبل كتابة رسالتهم <u> 1 </u> st) هو <u>{0}</u> min",
 }
 l_creact_on = {
@@ -3651,15 +3651,15 @@
     'en': "\n\nIn the Settings [Administrators] for @{0} enable:\n[✅ Delete Msgs]\n[✅ Ban Users]\n[✅ Invite Users]\n🕚Wait for 1min",
     'es': "\n\nEn la Configuración [Administradores] para @{0} active:\n[✅ Eliminar mensajes]\n[✅ Prohibir usuarios]\n[✅ Invitar usuarios]\n🕚Espere 1 minuto",
     'fr': "\n\nDans les paramètres [Administrateurs] pour @{0}, activez :\n[✅ Supprimer les messages]\n[✅ Bannir les utilisateurs]\n[✅ Inviter des utilisateurs]\n🕚Attendez 1 minute",
     'zh': "\n\n在@{0}的設置[管理員]中打開：\n[✅刪除消息]\n[✅禁止用戶]\n[✅邀請用戶]\n🕚等待1分鐘",
     'ar': "\n\n في الإعدادات [Administrators] لـ @{0} شغّل:\n [✅ حذف الرسائل] \n على [✅ حظر المستخدمين] \n [✅ دعوة المستخدمين] \n وانتظر لمدة دقيقة واحدة",
 }
 l_cview_correct = {
-    'ru': "👁️‍🗨️ Введи корректное <b>число</b> авто-просмотров последнего поста канала\n\n👩🏽‍💻 Используй команду <code>/view {0}</code>, чтобы задать количество авто-просмотров (<b>текущее</b> количество: <u>{0}</u>)",
+    'ru': "👁️‍🗨️ <b>Введи</b> корректное <b>число</b> авто-просмотров последнего поста канала\n\n👩🏽‍💻 Используй команду <code>/view {0}</code>, чтобы задать количество авто-просмотров (<b>текущее</b> количество: <u>{0}</u>)",
     'en': "👁️‍🗨️ Ready! Current primary delay for <u>new</u> users (before writing their <u>1</u>st message) is <u>{0}</u> min",
     'es': "👁️‍🗨️ Listo! El retraso principal actual para los <u>nuevos</u> usuarios (antes de escribir su <u>1</u>er mensaje) es <u>{0}</u> min",
     'fr': "👁️‍🗨️ Prêt! Le délai principal actuel pour les <u>nouveaux</u> utilisateurs (avant d'écrire leur <u>1</u>er message) est de <u>{0}</u> min",
     'zh': "👁️‍🗨️ 準備好了！<u>新</u>用戶的當前主要延遲（在寫他們的<u>1</u>st消息之前）是<u>{0}</u>分鐘",
     'ar': "👥 جاهز! التأخير الأساسي الحالي لمستخدمي <u> الجدد </u> (قبل كتابة رسالتهم <u> 1 </u> st) هو <u>{0}</u> min",
 }
 l_cview_on = {
@@ -3703,15 +3703,15 @@
     'en': "🪄 In the Settings [Administrators] enable:\n[✅ Pin Messages] for @{0}",
     'es': "🪄 En la Configuración [Administradores] habilite:\n[✅ Pinear mensajes] para @{0}",
     'fr': "🪄 Dans les paramètres [Administrateurs], activez :\n[✅ Épingler les messages] pour @{0}",
     'zh': "🪄 在設置 [Administrators] 中啟用：\n[✅ Pin Messages] for @{0}",
     'ar': "🔔 في الإعدادات ، فعّل [المسؤولون]: \n [✅ تثبيت الرسائل] لـ @{0}",
 }
 l_cdecor_footer_config = {
-    'ru': "🪄 Введи краткий <b>текст</b>, который будет добавляться в окончание к постам канала (например, часто используемые #хэштеги)",
+    'ru': "🪄 <b>Введи</b> краткий <b>текст</b>, который будет добавляться в окончание к постам канала (например, часто используемые #хэштеги)",
     'en': "🪄 There are no greetings you need to ⚙️Configure",
     'es': "🪄 No hay saludos que necesites ⚙️Configurar",
     'fr': "🪄 Vous n'avez pas besoin de salutations ⚙️Configurer",
     'zh': "🪄 無需問候⚙️配置",
     'ar': "🔔لا توجد تحيات تحتاج إلى تكوين",
 }
 l_cdecor_footer_done = {
@@ -4339,15 +4339,15 @@
     'en': "👮🏽 Ready! Current <b>button name</b> in <i>Enter control</i> is: {0}",
     'es': "👮🏽 Lista! El <b>nombre del botón</b> actual en <i>Control de entrada</i> es: {0}",
     'fr': "👮🏽 Prêt! Le <b>nom du bouton</b> actuel dans <i>Saisir le contrôle</i> est : {0}",
     'zh': "👮🏽 準備好! <i>輸入控件</i>中的當前<b>按鈕名稱</b>是：{0}",
     'ar': "👮🏽 جاهز! <b> اسم الزر </b> الحالي في <i> إدخال التحكم </i> هو: {0}",
 }
 l_button_correct = {
-    'ru': "👮🏽 Введи корректное название <i>для имени кнопки</i> Входного контроля\n\n👉🏼 Например, <code>/button {0}</code>",
+    'ru': "👮🏽 <b>Введи</b> корректное название <i>для имени кнопки</i> Входного контроля\n\n👉🏼 Например, <code>/button {0}</code>",
     'en': "👮🏽 Enter correct <i>button name</i> for Enter control\n\n👉🏼 For example, <code>/button {0}</code>",
     'es': "👮🏽 Ingrese el <i>nombre del botón</i> correcto para el control Intro\n\n👉🏼 Por ejemplo, <código>/botón {0}</código>",
     'fr': "👮🏽 Saisissez le <i>nom du bouton</i> correct pour Entrer le contrôle\n\n👉🏼 Par exemple, <code>/bouton {0}</code>",
     'zh': "👮🏽 為 Enter 控件輸入正確的 <i>按鈕名稱</i>\n\n👉🏼 例如，<code>/button {0}</code>",
     'ar': "👮🏽 أدخل <i> اسم الزر </i> الصحيح لإدخال عنصر التحكم \n\n👉🏼 على سبيل المثال ، <code> / button {0}</code>",
 }
 l_channel_check = {
@@ -4371,15 +4371,15 @@
     'en': "👮🏽 Add @{0} to channel and send correct <i>link</i> of this channel\n\n👉🏼 For example, <code>/channel @{1}</code>",
     'es': "👮🏽 Agrega @{0} al canal y envía el <i>enlace</i> correcto de este canal\n\n👉🏼 Por ejemplo, <code>/channel @{1}</code>",
     'fr': "👮🏽 Ajoutez @{0} au canal et envoyez le <i>lien</i> correct de ce canal\n\n👉🏼 Par exemple, <code>/channel @{1}</code>",
     'zh': "👮🏽 將@{0} 添加到頻道並發送此頻道的正確<i>鏈接</i>\n\n👉🏼 例如，<code>/channel @{1}</code>",
     'ar': "👮🏽 إضافة @{0} إلى القناة وإرسال <i> الرابط </i> الصحيح لهذه القناة \n \n👉🏼 على سبيل المثال ، <code> / channel @{1}</code>",
 }
 l_delay_correct = {
-    'ru': "👥 Введи корректное <i>число</i> минут для первичного ограничения новых пользователей\n\n👉🏼 Например, <code>/delay 1</code>\n\nИли используй <b>медленный режим</b> в настройках группы для <u>1</u> сообщения",
+    'ru': "👥 <b>Введи</b> корректное <i>число</i> минут для первичного ограничения новых пользователей\n\n👉🏼 Например, <code>/delay 1</code>\n\nИли используй <b>медленный режим</b> в настройках группы для <u>1</u> сообщения",
     'en': "👥 Enter correct <i>number</i> in minutes for primary mute-restriction for new users\n\n👉🏼 For example, <code>/delay 1</code>\n\nOr use <b>Slow Mode</b> in group Settings for <u>1</u>st message",
     'es': "👥 Ingrese el <i>número</i> correcto en minutos para la restricción de silencio principal para nuevos usuarios\n\n👉🏼 Por ejemplo, <code>/delay 1</code>\n\nO use <b>Slow Mode </b> en Configuración de grupo para <u>1</u>er mensaje",
     'fr': "👥 Entrez le <i>nombre</i> correct en minutes pour la restriction principale de mise en sourdine pour les nouveaux utilisateurs\n\n👉🏼 Par exemple, <code>/delay 1</code>\n\nOu utilisez le <b>mode lent </b> dans le groupe Paramètres pour le <u>1</u>er message",
     'zh': "👥 在分鐘內輸入正確的 <i>number</i> 用於新用戶的主要靜音限制\n\n👉🏼 例如，<code>/delay 1</code>\n\n或使用 <b>Slow Mode <u>1</u>st 消息的組設置中的</b>",
     'ar': "👥 أدخل <i> الرقم الصحيح </i> في دقائق لتقييد كتم الصوت الأساسي للمستخدمين الجدد \n \n👉🏼 على سبيل المثال ، <code> / تأخير 1 </code> \n \n أو استخدم <b> الوضع البطيء </b> في إعدادات المجموعة لرسالة <u> 1 </u> st",
 }
 l_parse_error = {
@@ -4628,15 +4628,15 @@
     'en': "🎥 Send this command as reply to message",
     'es': "🎥 Enviar este comando como respuesta al mensaje",
     'fr': "🎥 Envoyez cette commande en réponse au message",
     'zh': "🎥 將此命令作為對消息的回復發送",
     'ar': "🎉 أرسل هذا الأمر كرد على الرسالة",
 }
 l_flood_text = {
-    'ru': "💬 Введи корректное <i>число</i> сообщений от <u>3</u> до <u>10</u>\n\n👉🏼 Текущее значение <code>/flood {0}</code>\n\n👩🏽‍💻 Например, /flood 3 (идентификация 3х сообщений подряд как flood)\n/flood 0 (отключение опции)",
+    'ru': "💬 <b>Введи</b> корректное <i>число</i> сообщений от <u>3</u> до <u>10</u>\n\n👉🏼 Текущее значение <code>/flood {0}</code>\n\n👩🏽‍💻 Например, /flood 3 (идентификация 3х сообщений подряд как flood)\n/flood 0 (отключение опции)",
     'en': "🎥 Send this command as reply to message",
     'es': "🎥 Enviar este comando como respuesta al mensaje",
     'fr': "🎥 Envoyez cette commande en réponse au message",
     'zh': "🎥 將此命令作為對消息的回復發送",
     'ar': "🎉 أرسل هذا الأمر كرد على الرسالة",
 }
 l_flood_on = {
@@ -4652,15 +4652,15 @@
     'en': "🎥 Send this command as reply to message",
     'es': "🎥 Enviar este comando como respuesta al mensaje",
     'fr': "🎥 Envoyez cette commande en réponse au message",
     'zh': "🎥 將此命令作為對消息的回復發送",
     'ar': "🎉 أرسل هذا الأمر كرد على الرسالة",
 }
 l_delay_text = {
-    'ru': "👥 Введи корректное <i>число</i> минут для первичного ограничения новых пользователей\n\n👉🏼 Текущее значение <code>/delay {0}</code>\n\n👩🏽‍💻 Например, /delay 3 (ограничение на 3 min)\n/delay 0 (отключение опции)",
+    'ru': "👥 <b>Введи</b> корректное <i>число</i> минут для первичного ограничения новых пользователей\n\n👉🏼 Текущее значение <code>/delay {0}</code>\n\n👩🏽‍💻 Например, /delay 3 (ограничение на 3 min)\n/delay 0 (отключение опции)",
     'en': "🎥 Send this command as reply to message",
     'es': "🎥 Enviar este comando como respuesta al mensaje",
     'fr': "🎥 Envoyez cette commande en réponse au message",
     'zh': "🎥 將此命令作為對消息的回復發送",
     'ar': "🎉 أرسل هذا الأمر كرد على الرسالة",
 }
 l_delay_on = {
@@ -4953,23 +4953,23 @@
     'en': "🚶🏽 No available subscribers",
     'es': "🚶🏽 No hay suscriptores disponibles",
     'fr': "🚶🏽 Aucun abonné disponible",
     'zh': "🚶🏽 沒有可用的訂閱者",
     'ar': "🚶🏽 لا يوجد مشتركون متاحون",
 }
 l_current_participants = {
-    'ru': "🚶🏽 Для {0}<b>текущее количество</b> реальных подписчиков: <u>{1}</u>\n\n▪️ Введи <i>число</i> подписчиков, которое необходимо подписывать <b>ежедневно</b> от 1 до 3 (без подписки +{2}):",
+    'ru': "🚶🏽 Для {0}<b>текущее количество</b> реальных подписчиков: <u>{1}</u>\n\n▪️ <b>Введи</b> <i>число</i> подписчиков, которое необходимо подписывать <b>ежедневно</b> от 1 до 3 (без подписки +{2}):",
     'en': "🚶🏽 For {0}<b>current number</b> of real members: <u>{1}</u>\n\n▪️ Enter <i>number</i> of members to subscribe <b>everyday</b> from 1 to 3 (without subscription +{2}):",
     'es': "🚶🏽 Para {0}<b>número actual</b> de miembros reales: <u>{1}</u>\n\n▪️ Ingrese <i>número</i> de miembros para suscribirse <b>todos los días </b> del 1 al 3 (sin suscripción +{2}):",
     'fr': "🚶🏽 Pour {0}<b>nombre actuel</b> de membres réels : <u>{1}</u>\n\n▪️ Saisissez le <i>nombre</i> de membres à souscrire <b>tous les jours </b> de 1 à 3 (sans abonnement +{2}) :",
     'zh': "🚶🏽 {0}<b>當前人數</b> 的真實會員：<u>{1}</u>\n\n▪️ 輸入 <i>會員人數</i> 以訂閱<b>每天 </b> 從 1 到 3（無訂閱 +{2}）：",
     'ar': "🚶🏽 بالنسبة إلى {0}<b> العدد الحالي </b> للأعضاء الحقيقيين: <u>{1}</u> \n\n▪️ أدخل <i> عدد </i> من الأعضاء للاشتراك <b> كل يوم </b> من 1 إلى 3 (بدون اشتراك + {2}):",
 }
 l_everyday_participants = {
-    'ru': "🚶🏽 Введи количество пользователей для ежедневной подписки от 1 до 3 включительно",
+    'ru': "🚶🏽 <b>Введи</b> количество пользователей для ежедневной подписки от 1 до 3 включительно",
     'en': "🚶🏽 Enter number of users for everyday inviting from 1 to 3",
     'es': "🚶🏽 Ingrese el número de usuarios para invitar todos los días de 1 a 3",
     'fr': "🚶🏽 Entrez le nombre d'utilisateurs pour l'invitation quotidienne de 1 à 3",
     'zh': "🚶🏽 輸入每天邀請的用戶數，從 1 到 3",
     'ar': "🚶🏽 أدخل عدد المستخدمين للدعوة اليومية من 1 إلى 3",
 }
 l_invite_need_subscribe = {
@@ -4977,15 +4977,15 @@
     'en': "🚶🏽 For inviting > 1 members per day you have to subscribe or type 1:",
     'es': "🚶🏽 Para invitar > 1 miembros por día tienes que suscribirte o escribir 1:",
     'fr': "🚶🏽 Pour inviter > 1 membres par jour il faut s'inscrire ou taper 1 :",
     'zh': "🚶🏽 每天邀請 > 1 個成員，您必須訂閱或輸入 1：",
     'ar': "🚶🏽 لدعوة> عضو واحد يوميًا ، يجب عليك الاشتراك أو اكتب 1:",
 }
 l_invite_correct_num = {
-    'ru': "🚶🏽 Введи корректное число",
+    'ru': "🚶🏽 <b>Введи</b> корректное число",
     'en': "🚶🏽 Enter correct number",
     'es': "🚶🏽 Ingrese el número correcto",
     'fr': "🚶🏽 Entrez le bon numéro",
     'zh': "🚶輸入正確的數字",
     'ar': "🚶🏽 Enter correct number",
 }
 l_fsm_invite_finish = {
@@ -5033,15 +5033,15 @@
     'en': "🚶🏽 Ready! <b>Auto</b>-inviting <u>{0}</u> users per day from group {1}",
     'es': "🚶🏽 Listo! Invitación <b>automática</b> a <u>{0}</u> usuarios por día del grupo {1}",
     'fr': "🚶🏽 Prêt ! <b>Auto</b>-inviter <u>{0}</u> utilisateurs par jour du groupe {1}",
     'zh': "🚶🏽 準備好了！ <b>自動</b>-每天從組 {1} 中邀請 <u>{0}</u> 個用戶",
     'ar': "🚶🏽 جاهز! <b> دعوة تلقائية </b> <u>{0}</u> للمستخدمين يوميًا من المجموعة {1}",
 }
 l_cinvite_choose_cnt = {
-    'ru': "🚶🏽 Введи <b>количество</b> пользователей для авто-инвайта, которые будут приглашаться ежедневно (без подписки: 1 польз)",
+    'ru': "🚶🏽 <b>Введи</b> <b>количество</b> пользователей для авто-инвайта, которые будут приглашаться ежедневно (без подписки: 1 польз)",
     'en': "🚶🏽 Ready! <b>Auto</b>-inviting <u>{0}</u> users per day from group {1}",
     'es': "🚶🏽 Listo! Invitación <b>automática</b> a <u>{0}</u> usuarios por día del grupo {1}",
     'fr': "🚶🏽 Prêt ! <b>Auto</b>-inviter <u>{0}</u> utilisateurs par jour du groupe {1}",
     'zh': "🚶🏽 準備好了！ <b>自動</b>-每天從組 {1} 中邀請 <u>{0}</u> 個用戶",
     'ar': "🚶🏽 جاهز! <b> دعوة تلقائية </b> <u>{0}</u> للمستخدمين يوميًا من المجموعة {1}",
 }
 l_cinvite_choose_group = {
@@ -5626,23 +5626,23 @@
     'en': "\n\n▪️word case is not important\n▪️set * after word to account for occurrence\n▪️for example, if write <b>psy*</b>, then <u>all</u> messages, which are <b>contained</b> this combination of letters will be removed: <i>anti-<u>psy</u>chologist, <u>Psy</u>chotherapist..</i>",
     'es': "\n\n▪️las mayúsculas y minúsculas no son importantes\n▪️establezca * después de la palabra para tener en cuenta la ocurrencia\n▪️por ejemplo, si escribe <b>psi*</b>, entonces <u>todos</u> los mensajes, que están <b>contenidos</b> se eliminará esta combinación de letras: <i>anti-<u>psicólogo</u>, <u>Psi</u>coterapeuta..</i>",
     'fr': "\n\n▪️la casse des mots n'est pas importante\n▪️définissez * après le mot pour tenir compte de l'occurrence\n▪️par exemple, si écrivez <b>psy*</b>, alors <u>tous</u> les messages, qui sont <b>contenues</b> cette combinaison de lettres sera supprimée : <i>anti-<u>psychologue</u>, <u>Psy</u>chothérapeute..</i>",
     'zh': "\n\n▪️單詞大小寫不重要\n▪️在單詞之後設置*以說明出現\n▪️例如，如果寫<b>psy*</b>，則<u>所有</u>消息， <b>包含</b>這些字母組合將被刪除：<i>anti-<u>psy</u>chologist, <u>Psy</u>chotherapy..</i>",
     'ar': "\n\n▪️ حالة الكلمة ليست مهمة \n▪️ اضبط * بعد كلمة لحساب الحدوث \n▪️ على سبيل المثال ، إذا كتبت <b>psy*</b> ، ثم <u> كل </u> الرسائل ، التي <b> احتوت </b> ستتم إزالة هذه المجموعة من الأحرف:",
 }
 l_cstartoperation_answer = {
-    'ru': "🚀 Введи <u>старт-слова</u> <b>через</b> пробелы или разделители, чтобы <i>добавить</i> их в базу{0}",
+    'ru': "🚀 <b>Введи</b> <u>старт-слова</u> <b>через</b> пробелы или разделители, чтобы <i>добавить</i> их в базу{0}",
     'en': "🚀 Enter <u>start-words</u> <b>via</b> spaces or separators to <i>add</i> them to Base{0}",
     'es': "🚀 Ingrese <u>palabras de inicio</u> <b>mediante</b> espacios o separadores para <i>agregarlos</i> a la Base{0}",
     'fr': "🚀 Saisissez des <u>start-words</u> <b>via</b> des espaces ou des séparateurs pour les <i>ajouter</i> à Base{0}",
     'zh': "🚀 輸入 <u>start-words</u> <b>via</b> 空格或分隔符以將它們<i>添加</i>到 Base{0}",
     'ar': "✅ أدخل كلمات البداية عبر مسافات أو فواصل من أجل <i> إضافتها </i> إلى القاعدة {0}",
 }
 l_cstartoperation_noanswer = {
-    'ru': "🚫 Введи <u>старт-слова</u> <b>через</b> пробелы или разделители, чтобы их <i>удалить</i> из базы{0}",
+    'ru': "🚫 <b>Введи</b> <u>старт-слова</u> <b>через</b> пробелы или разделители, чтобы их <i>удалить</i> из базы{0}",
     'en': "🚫 Enter <u>start-words</u> <b>via</b> spaces or separators to <i>remove</i> them from Base{0}",
     'es': "🚫 Ingrese <u>palabras de inicio</u> <b>mediante</b> espacios o separadores para <i>eliminarlos</i> de la Base{0}",
     'fr': "🚫 輸入 <u>start-words</u> <b>via</b> 空格或分隔符以將它們從 Base 中<i>刪除</i>{0}",
     'zh': "🚫 輸入 <u>start-words</u> <b>via</b> 空格或分隔符以將它們從 Base 中<i>刪除</i>{0}",
     'ar': "🚫 أدخل كلمات البداية عبر مسافات أو فواصل <i> لإزالتها </i> من Base {0}",
 }
 l_fsm_start_add_caption = {
@@ -5711,23 +5711,23 @@
     'en': "\n\n▪️word case is not important\n▪️set * after word to account for occurrence\n▪️for example, if write <b>psy*</b>, then <u>all</u> messages, which are <b>contained</b> this combination of letters will be removed: <i>anti-<u>psy</u>chologist, <u>Psy</u>chotherapist..</i>",
     'es': "\n\n▪️las mayúsculas y minúsculas no son importantes\n▪️establezca * después de la palabra para tener en cuenta la ocurrencia\n▪️por ejemplo, si escribe <b>psi*</b>, entonces <u>todos</u> los mensajes, que están <b>contenidos</b> se eliminará esta combinación de letras: <i>anti-<u>psicólogo</u>, <u>Psi</u>coterapeuta..</i>",
     'fr': "\n\n▪️la casse des mots n'est pas importante\n▪️définissez * après le mot pour tenir compte de l'occurrence\n▪️par exemple, si écrivez <b>psy*</b>, alors <u>tous</u> les messages, qui sont <b>contenues</b> cette combinaison de lettres sera supprimée : <i>anti-<u>psychologue</u>, <u>Psy</u>chothérapeute..</i>",
     'zh': "\n\n▪️單詞大小寫不重要\n▪️在單詞之後設置*以說明出現\n▪️例如，如果寫<b>psy*</b>，則<u>所有</u>消息， <b>包含</b>這些字母組合將被刪除：<i>anti-<u>psy</u>chologist, <u>Psy</u>chotherapy..</i>",
     'ar': "\n\n▪️ حالة الكلمة ليست مهمة \n▪️ اضبط * بعد كلمة لحساب الحدوث \n▪️ على سبيل المثال ، إذا كتبت <b>psy*</b> ، ثم <u> كل </u> الرسائل ، التي <b> احتوت </b> ستتم إزالة هذه المجموعة من الأحرف:",
 }
 l_cstopchange_answer = {
-    'ru': "✅ Введи <u>стоп-слова</u> <b>через</b> пробелы или разделители, чтобы <i>добавить</i> их в базу{0}",
+    'ru': "✅ <b>Введи</b> <u>стоп-слова</u> <b>через</b> пробелы или разделители, чтобы <i>добавить</i> их в базу{0}",
     'en': "✅ Enter <u>stop-words</u> <b>via</b> spaces or separators to <i>add</i> them to Base{0}",
     'es': "✅ Ingrese <u>palabras vacías</u> <b>a través de</b> espacios o separadores para <i>agregarlos</i> a la Base{0}",
     'fr': "✅ Saisissez des <u>mots vides</u> <b>via</b> des espaces ou des séparateurs pour les <i>ajouter</i> à Base{0}",
     'zh': "✅ 輸入 <u>停用詞</u> <b>通過</b> 空格或分隔符將它們<i>添加</i>到 Base{0}",
     'ar': "✅ أدخل <u> كلمات الإيقاف </u> <b> عبر </b> مسافات أو فواصل من أجل <i> إضافتها </i> إلى القاعدة {0}",
 }
 l_cstopchange_noanswer = {
-    'ru': "🚫 Введи <u>стоп-слова</u> <b>через</b> пробелы или разделители, чтобы их <i>удалить</i> из базы{0}",
+    'ru': "🚫 <b>Введи</b> <u>стоп-слова</u> <b>через</b> пробелы или разделители, чтобы их <i>удалить</i> из базы{0}",
     'en': "🚫 Enter <u>stop-words</u> <b>via</b> spaces or separators to <i>removed </i> them from Base{0}",
     'es': "🚫 Ingrese <u>palabras vacías</u> <b>a través de</b> espacios o separadores para <i>eliminarlos </i> de la base {0}",
     'fr': "🚫 Saisissez des <u>mots vides</u> <b>via</b> des espaces ou des séparateurs pour les <i>supprimer </i> de Base {0}",
     'zh': "🚫 輸入 <u>stop-words</u> <b>via</b> 空格或分隔符以將它們從 Base 中<i>刪除 </i>{0}",
     'ar': "🚫 أدخل <u> كلمات الإيقاف </u> <b> عبر </b> مسافات أو فواصل لـ <i> إزالتها </i> من Base {0}",
 }
 l_fsm_stop_add_caption = {
@@ -6281,15 +6281,15 @@
     'fr': "➕ Retour..",
     'zh': "➕ 回來..",
     'ar': "🔙 رجوع ..",
 }
 
 # region commands
 l_bot_commands_handler = {
-    'ru': "⚙️ <b>Команды</b> /cmd для <b>@{0}</b>\n\n/info   <i>информация</i>\n/stat   <i>аналитика</i>\n/on     <i>включение</i>\n<code>/off</code>    <i>выключение</i>\n<code>/restart</code>  <i>перезагрузка</i>\n/status <i>статус</i>\n\n/parse [аргумент]  <i>участники</i>\n/admin      <i>администраторы</i>\n/promo      <i>промокод</i>\n/ban [id/@username]   <i>список</i>/unban     <i>разбан</i>",
+    'ru': "⚙️ <b>Команды</b> /cmd для <b>@{0}</b>\n\n/info   <i>информация</i>\n/stat   <i>аналитика</i>\n/status <i>статус</i>\n/on     <i>включение</i>\n<code>/off</code>    <i>выключение</i>\n<code>/restart</code>  <i>перезагрузка</i>\n\n/parse [premium|admin|utm|ban]\n/admin [id]    <i>администраторы</i>\n/promo      <i>промокод</i>\n/ban [id/@username]   <i>список</i>\n/unban     <i>разбан</i>",
     'en': "⚙️ <b>Account commands</b> /cmd for <b>{0}</b> in @{1} works also and in the target bot\n\n/update <i>profile copy</i>\n/info   <i>information</i>\n/stat   <i>statistics</i>\n/status <i>bot status</i>\n/log    <i>recent actions</i>\n/on     <i>enable bot</i>\n<code>/off</code>    <i>disable bot</i>\n<code>/repair</code> <i>accout clear: reading history</i>\n<code>/reset</code>  <i>bot reset: deleting dialogs</i>\n\n/parse      <i>[link/id on chat] [argument]</i>\n/login      <i>login to bot</i>\n/spambot    <i>bot karma</i>\n/autodel+days   <i>auto-deletion 1-365 days</i>\n/delay+sec  <i>auto-delay of auto-answer</i>\n/join+file  <i>join to groups/channels</i>\n/vote       <i>[id of chat] [option]</i>\n<code>/leaveall</code>   <i>leave all groups/channels</i>\n<code>/deleteall</code>  <i>delete all dialogs</i>\n\n# only from bot name\n/screen <i>screenshort-nortification</i>\n/type+msg     <i>typing</i>\n/think          <i>thinking</i>\n<code>* geo-location sending returns @username-list</code>",
     'es': "⚙️ Configuración de <b>Grupo</b> de <b>{0}</b>{1}\n\n<b>⛏ Comandos de administración @{2}</b>\n/update <i>parameters</i>\n/transfer   <i>admin-settings</i>\n/info   <i>information</i>\n/stat   <i>statistics</i>\n/parse  <i>[all|old|premium|active|online]</i>\n<code>/parse old</code> - <i>parsing old id-bots</i>\n\n/channel NAME   <i>add channel for subscribe checking</i>\n/button NAME    <i>add button's name for Enter Control</i>\n/delay MIN      <i>set delay number [min] for 1st message</i>\n/flood NUM      <i>set msg-number for flood</i>\n\n<b>⛏ Commands for other administrations</b>\n/ban 5m|1h|10d <i>delete from bot for time</i>\n/unban\n/mute 5m|1h|10d <i>restriction in bot for time</i>\n/unmute\n/warn+msg <i>warning</i>\n/status\n/karma  [+|-]\n/tag+msg   <i>@tager random-bots</i>\n\n<b>⛏ Commands for users</b>\n/help   <i>show commands</i>\n/rules  <i>for bot</i>\n/report <i>about violation</i>\n/happy  <i>get happyness</i>\n/thanks <i>say to user thank you</i>",
     'fr': "⚙️ Paramètres de <b>bote</b> de <b>{0}</b>{1}\n\n<b>⛏ Commandes d'administration @{2}</b>\n/update <i>parameters</i>\n/transfer   <i>admin-settings</i>\n/info   <i>information</i>\n/stat   <i>statistics</i>\n/parse  <i>[all|old|premium|active|online]</i>\n<code>/parse old</code> - <i>parsing old id-bots</i>\n\n/channel NAME   <i>add channel for subscribe checking</i>\n/button NAME    <i>add button's name for Enter Control</i>\n/delay MIN      <i>set delay number [min] for 1st message</i>\n/flood NUM      <i>set msg-number for flood</i>\n\n<b>⛏ Commands for other administrations</b>\n/ban 5m|1h|10d <i>delete from bot for time</i>\n/unban\n/mute 5m|1h|10d <i>restriction in bot for time</i>\n/unmute\n/warn+msg <i>warning</i>\n/status\n/karma  [+|-]\n/tag+msg   <i>@tager random-bots</i>\n\n<b>⛏ Commands for users</b>\n/help   <i>show commands</i>\n/rules  <i>for bot</i>\n/report <i>about violation</i>\n/happy  <i>get happyness</i>\n/thanks <i>say to user thank you</i>",
     'zh': "⚙️ <b>組</b>設置 <b>{0}</b>{1}\n\n<b>⛏ 管理員命令 @{2}</b>\n/update <i>parameters</i>\n/transfer   <i>admin-settings</i>\n/info   <i>information</i>\n/stat   <i>statistics</i>\n/parse  <i>[all|old|premium|active|online]</i>\n<code>/parse old</code> - <i>parsing old id-bots</i>\n\n/channel NAME   <i>add channel for subscribe checking</i>\n/button NAME    <i>add button's name for Enter Control</i>\n/delay MIN      <i>set delay number [min] for 1st message</i>\n/flood NUM      <i>set msg-number for flood</i>\n\n<b>⛏ Commands for other administrations</b>\n/ban 5m|1h|10d <i>delete from bot for time</i>\n/unban\n/mute 5m|1h|10d <i>restriction in bot for time</i>\n/unmute\n/warn+msg <i>warning</i>\n/status\n/karma  [+|-]\n/tag+msg   <i>@tager random-bots</i>\n\n<b>⛏ Commands for users</b>\n/help   <i>show commands</i>\n/rules  <i>for bot</i>\n/report <i>about violation</i>\n/happy  <i>get happyness</i>\n/thanks <i>say to user thank you</i>",
     'ar': "⚙️ إعدادات <b> المجموعة </b> الخاصة بـ <b>{0}</b>{1}\n\n<b>⛏ أوامر المسؤول @{2}</b>\n/update <i>parameters</i>\n/transfer   <i>admin-settings</i>\n/info   <i>information</i>\n/stat   <i>statistics</i>\n/parse  <i>[all|old|premium|active|online]</i>\n<code>/parse old</code> - <i>parsing old id-bots</i>\n\n/channel NAME   <i>add channel for subscribe checking</i>\n/button NAME    <i>add button's name for Enter Control</i>\n/delay MIN      <i>set delay number [min] for 1st message</i>\n/flood NUM      <i>set msg-number for flood</i>\n\n<b>⛏ Commands for other administrations</b>\n/ban 5m|1h|10d <i>delete from bot for time</i>\n/unban\n/mute 5m|1h|10d <i>restriction in bot for time</i>\n/unmute\n/warn+msg <i>warning</i>\n/status\n/karma  [+|-]\n/tag+msg   <i>@tager random-bots</i>\n\n<b>⛏ Commands for users</b>\n/help   <i>show commands</i>\n/rules  <i>for bot</i>\n/report <i>about violation</i>\n/happy  <i>get happyness</i>\n/thanks <i>say to user thank you</i>",
 }
 l_bot_status_handler = {
@@ -6867,31 +6867,31 @@
     'en': "👮🏽 Push the ✅/☑️ to <b>On/Off</b> auto-transcribe (speach to text) for <i><b>income</b>/<b>outgoing</b> messages</i>",
     'es': "👮🏽 Presiona ✅/☑️ para <b>Encender/Apagar</b> <i>sistema</i> mensajes\n\n👩🏽‍💻 Por ejemplo, <i>Usuario se unió al grupo</i>",
     'fr': "👮🏽 Appuyez sur ✅/☑️ pour <b>Activer/Désactiver</b> les messages <i>système</i>\n\n👩🏽‍💻 Par exemple, <i>L'utilisateur a rejoint le bote</i>",
     'zh': "👮🏽 將 ✅/☑️ 推送到 <b>On/Off</b> <i>system</i> 消息\n\n👩🏽‍💻 例如，<i>用戶加入群組</i>",
     'ar': "👣 اضغط على ✅ / ☑️ ، إلى رسائل <b> تشغيل / إيقاف </b> <i> النظام </i>\n\n👩🏽‍💻 على سبيل المثال ، <i> انضم المستخدم إلى المجموعة </i>",
 }
 l_cadmin_done = {
-    'ru': "👮🏽 <b>Готово!</b>/admin-список администраторов @{0}-бота\n\n👩🏽‍💻 <b>Команды</b>:\n/cmd - все команды\n/admin - добавить/удалить администратора\n/parse - вывести всех пользователей\n\n👩🏽‍💻 Текущее число администраторов: <u>{1}</u>",
+    'ru': "👮🏽 <b>Готово!</b>/admin-список @{0}-бота:\n\n{1}\n\n👩🏽‍💻 <b>Команды</b>:\n/cmd - все команды\n/admin - добавить/удалить администратора\n/parse - вывести всех пользователей\n\n👩🏽‍💻 Текущее число администраторов: <u>{2}/10</u>",
     'en': "🗣 Push the ✅/☑️ to <b>On/Off</b> auto-transcribe (speach to text) for <i><b>income</b>/<b>outgoing</b> messages</i>",
     'es': "🗣 Presiona ✅/☑️ para <b>Encender/Apagar</b> <i>sistema</i> mensajes\n\n👩🏽‍💻 Por ejemplo, <i>Usuario se unió al grupo</i>",
     'fr': "🗣 Appuyez sur ✅/☑️ pour <b>Activer/Désactiver</b> les messages <i>système</i>\n\n👩🏽‍💻 Par exemple, <i>L'utilisateur a rejoint le bote</i>",
     'zh': "🗣 將 ✅/☑️ 推送到 <b>On/Off</b> <i>system</i> 消息\n\n👩🏽‍💻 例如，<i>用戶加入群組</i>",
     'ar': "👣 اضغط على ✅ / ☑️ ، إلى رسائل <b> تشغيل / إيقاف </b> <i> النظام </i>\n\n👩🏽‍💻 على سبيل المثال ، <i> انضم المستخدم إلى المجموعة </i>",
 }
 l_cadmin_add = {
-    'ru': "👮🏽 Введи <code>id</code> или <code>@username</code> пользователей из <u>{0}</u>-файла через пробельные символы или разделители, чтобы добавить их в /admin-список\n\n👩🏽‍💻 Текущее число администраторов: <u>{1}</u>",
+    'ru': "👮🏽 <b>Введи</b> <code>id</code> пользователей через пробельные символы или разделители, чтобы добавить их в /admin-список\n\n👩🏽‍💻 Текущее число администраторов: <u>{0}</u>",
     'en': "🗣 Push the ✅/☑️ to <b>On/Off</b> auto-transcribe (speach to text) for <i><b>income</b>/<b>outgoing</b> messages</i>",
     'es': "🗣 Presiona ✅/☑️ para <b>Encender/Apagar</b> <i>sistema</i> mensajes\n\n👩🏽‍💻 Por ejemplo, <i>Usuario se unió al grupo</i>",
     'fr': "🗣 Appuyez sur ✅/☑️ pour <b>Activer/Désactiver</b> les messages <i>système</i>\n\n👩🏽‍💻 Par exemple, <i>L'utilisateur a rejoint le bote</i>",
     'zh': "🗣 將 ✅/☑️ 推送到 <b>On/Off</b> <i>system</i> 消息\n\n👩🏽‍💻 例如，<i>用戶加入群組</i>",
     'ar': "👣 اضغط على ✅ / ☑️ ، إلى رسائل <b> تشغيل / إيقاف </b> <i> النظام </i>\n\n👩🏽‍💻 على سبيل المثال ، <i> انضم المستخدم إلى المجموعة </i>",
 }
 l_cadmin_remove = {
-    'ru': "👮🏽 Введи <code>id</code> или <code>@username</code> пользователей из <u>{0}</u>-файла через пробельные символы или разделители, чтобы удалить их из /admin-список\n\n👩🏽‍💻 Текущее число администраторов: <u>{1}</u>",
+    'ru': "👮🏽 <b>Введи</b> <code>id</code> пользователей через пробельные символы или разделители, чтобы удалить их из /admin-список\n\n👩🏽‍💻 Текущее число администраторов: <u>{0}</u>",
     'en': "🗣 Push the ✅/☑️ to <b>On/Off</b> auto-transcribe (speach to text) for <i><b>income</b>/<b>outgoing</b> messages</i>",
     'es': "🗣 Presiona ✅/☑️ para <b>Encender/Apagar</b> <i>sistema</i> mensajes\n\n👩🏽‍💻 Por ejemplo, <i>Usuario se unió al grupo</i>",
     'fr': "🗣 Appuyez sur ✅/☑️ pour <b>Activer/Désactiver</b> les messages <i>système</i>\n\n👩🏽‍💻 Par exemple, <i>L'utilisateur a rejoint le bote</i>",
     'zh': "🗣 將 ✅/☑️ 推送到 <b>On/Off</b> <i>system</i> 消息\n\n👩🏽‍💻 例如，<i>用戶加入群組</i>",
     'ar': "👣 اضغط على ✅ / ☑️ ، إلى رسائل <b> تشغيل / إيقاف </b> <i> النظام </i>\n\n👩🏽‍💻 على سبيل المثال ، <i> انضم المستخدم إلى المجموعة </i>",
 }
 l_parse_text = {
```

### Comparing `yeref-0.1.66/yeref/yeref.py` & `yeref-0.1.67/yeref/yeref.py`

 * *Files 0% similar despite different names*

```diff
@@ -447,14 +447,15 @@
 
             for page_ in pages_['pages']:
                 if page_['url'] != url: continue
 
                 get_page_ = await telegraph_.get_page(path=page_['path'], return_content=True, return_html=False)
                 try:
                     content_json = json.loads(str(get_page_['content'][0]))
+                    if len(content_json) > 20: raise Exception
                 except:
                     content_json = {}
 
                 timestamp_ = str(utils.datetime_to_timestamp(datetime.datetime.utcnow()))
                 content_json[timestamp_] = json_
                 post_dumps = json.dumps(content_json, ensure_ascii=False)
                 await telegraph_.edit_page(path=page_['path'], title=page_['title'], html_content=post_dumps)
```

