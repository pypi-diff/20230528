# Comparing `tmp/streamlit_chatbox-0.1.0-py3-none-any.whl.zip` & `tmp/streamlit_chatbox-0.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 3615 bytes, number of entries: 5
--rw-rw-rw-  2.0 fat     6250 b- defN 23-May-28 07:03 streamlit_chatbox/__init__.py
--rw-rw-rw-  2.0 fat     1374 b- defN 23-May-28 07:13 streamlit_chatbox-0.1.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-28 07:13 streamlit_chatbox-0.1.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       18 b- defN 23-May-28 07:13 streamlit_chatbox-0.1.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      424 b- defN 23-May-28 07:13 streamlit_chatbox-0.1.0.dist-info/RECORD
-5 files, 8158 bytes uncompressed, 2819 bytes compressed:  65.4%
+Zip file size: 3924 bytes, number of entries: 5
+-rw-rw-rw-  2.0 fat     7601 b- defN 23-May-28 14:21 streamlit_chatbox/__init__.py
+-rw-rw-rw-  2.0 fat     1252 b- defN 23-May-28 14:25 streamlit_chatbox-0.1.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-28 14:25 streamlit_chatbox-0.1.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       18 b- defN 23-May-28 14:25 streamlit_chatbox-0.1.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      424 b- defN 23-May-28 14:25 streamlit_chatbox-0.1.1.dist-info/RECORD
+5 files, 9387 bytes uncompressed, 3128 bytes compressed:  66.7%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
 Filename: streamlit_chatbox/__init__.py
 Comment: 
 
-Filename: streamlit_chatbox-0.1.0.dist-info/METADATA
+Filename: streamlit_chatbox-0.1.1.dist-info/METADATA
 Comment: 
 
-Filename: streamlit_chatbox-0.1.0.dist-info/WHEEL
+Filename: streamlit_chatbox-0.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: streamlit_chatbox-0.1.0.dist-info/top_level.txt
+Filename: streamlit_chatbox-0.1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: streamlit_chatbox-0.1.0.dist-info/RECORD
+Filename: streamlit_chatbox-0.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## streamlit_chatbox/__init__.py

```diff
@@ -1,61 +1,58 @@
 import streamlit as st
+import time
 
 
 class MsgType:
     TEXT = 1
     IMAGE = 2
     VIDEO = 3
     AUDIO = 4
 
 
 class StChatBox:
     def __init__(
         self,
         chat_box,
-        session_var = 'chat_box',
-        greetings = [],
-        box_margin = '10%',
-        user_bg_color = '#77ff77',
-        user_icon = 'https://tse2-mm.cn.bing.net/th/id/OIP-C.LTTKrxNWDr_k74wz6jKqBgHaHa?w=203&h=203&c=7&r=0&o=5&pid=1.7',
-        robot_bg_color = '#ccccee',
-        robot_icon = 'https://ts1.cn.mm.bing.net/th/id/R-C.5302e2cc6f5c7c4933ebb3394e0c41bc?rik=z4u%2b7efba5Mgxw&riu=http%3a%2f%2fcomic-cons.xyz%2fwp-content%2fuploads%2fStar-Wars-avatar-icon-C3PO.png&ehk=kBBvCvpJMHPVpdfpw1GaH%2brbOaIoHjY5Ua9PKcIs%2bAc%3d&risl=&pid=ImgRaw&r=0',
+        session_var='chat_box',
+        greetings=[],
+        box_margin='10%',
+        user_bg_color='#77ff77',
+        user_icon='',
+        robot_bg_color='#ccccee',
+        robot_icon='',
     ):
         self.session_var = session_var
         self.greetings = greetings
         self.box_margin = box_margin
         self.user_bg_color = user_bg_color
         self.user_icon = user_icon
         self.robot_bg_color = robot_bg_color
         self.robot_icon = robot_icon
         self.last_response = None
         self.chat_box = chat_box
         self.init_session()
         self.show_welcome()
 
-
     def init_session(self):
-        st.session_state.setdefault(self.session_var, {'history': [], 'welcomed': False})
-
+        st.session_state.setdefault(
+            self.session_var, {'history': [], 'welcomed': False})
 
     @property
     def history(self):
         return st.session_state.get(self.session_var, {}).get('history', [])
 
-
     @property
     def welcomed(self):
         return st.session_state.get(self.session_var, {}).get('welcomed', False)
 
-
     @welcomed.setter
     def welcomed(self, val):
         st.session_state[self.session_var]['welcomed'] = bool(val)
 
-
     def format_md(self, msg, is_user=False, bg_color=None, margin=None):
         '''
         将文本消息格式化为markdown文本
         '''
         margin = margin or self.box_margin
         if is_user:
             bg_color = bg_color or self.user_bg_color
@@ -78,33 +75,30 @@
                             padding:2%;
                             border-radius:20px 0 0 0;">
                     {msg}
                     </div>
                     '''
         return text
 
-
     def robot_say(self, msg, msg_type=MsgType.TEXT, **kw):
         kw.update(is_user=False, content=msg, msg_type=msg_type)
         self.history.append(kw)
 
-
     def user_say(self, msg, msg_type=MsgType.TEXT, **kw):
         kw.update(is_user=True, content=msg, msg_type=msg_type)
         self.history.append(kw)
 
-
     def render_msg(self,
-                msg,
-                is_user=False,
-                msg_type=MsgType.TEXT,
-                icon=None,
-                bg_color=None,
-                margin=None,
-                ):
+                   msg,
+                   is_user=False,
+                   msg_type=MsgType.TEXT,
+                   icon=None,
+                   bg_color=None,
+                   margin=None,
+                   ):
         '''
         渲染单条消息。目前仅支持文本
         '''
         margin = margin or self.box_margin
         cols = st.columns([1, 10, 1])
         empty = cols[1].empty()
         if is_user:
@@ -125,62 +119,93 @@
             if msg_type == MsgType.TEXT:
                 text = self.format_md(msg, is_user, bg_color, margin)
                 empty.markdown(text, unsafe_allow_html=True)
             else:
                 raise RuntimeError('only support text message now.')
         return empty
 
-
     def show_welcome(self):
         if self.greetings and not self.welcomed:
             greetings = self.greetings
             if not isinstance(greetings, list):
                 greetings = [greetings]
             for g in greetings:
                 if isinstance(g, str):
                     self.robot_say(g)
                 elif isinstance(g, dict):
                     self.robot_say(**g)
             self.welcomed = True
 
-
     def output_messages(
         self,
         user_bg_color=None,
         robot_bg_color=None,
         user_icon=None,
         robot_icon=None,
     ):
         with self.chat_box.container():
             for msg in self.history:
                 bg_color = user_bg_color if msg['is_user'] else robot_bg_color
                 icon = user_icon if msg['is_user'] else robot_icon
                 empty = self.render_msg(msg['content'],
-                                is_user=msg['is_user'],
-                                icon=icon,
-                                msg_type=msg['msg_type'],
-                                bg_color=bg_color,
-                                )
+                                        is_user=msg['is_user'],
+                                        icon=icon,
+                                        msg_type=msg['msg_type'],
+                                        bg_color=bg_color,
+                                        )
                 if not msg['is_user']:
                     self.last_response = empty
         return self.last_response
 
-
     def update_last_box_text(self, msg):
         if self.last_response is not None:
             self.history[-1]['content'] = msg
             self.last_response.markdown(
-                        self.format_md(msg, False),
-                        unsafe_allow_html=True
-                    )
-
+                self.format_md(msg, False),
+                unsafe_allow_html=True
+            )
+
+    def robot_stream(self, msg, words_per_sec=10, max_seconds=10):
+        step = max(words_per_sec, len(msg) // max_seconds + 1) // 5 + 1
+        self.robot_say('')
+        self.output_messages()
+        for i in range(step, len(msg) + step * 2, step):
+            print(i, msg[:i])
+            time.sleep(0.2)
+            self.update_last_box_text(msg[:i])
 
     def clear_history(self, welcome_again=False):
         self.history = []
         if welcome_again:
             self.show_welcome()
 
 
-def st_chatbox(**kw):
+def st_chatbox(
+        session_var='chat_box',
+        greetings=[],
+        box_margin='10%',
+        user_bg_color='#77ff77',
+        user_icon='https://tse2-mm.cn.bing.net/th/id/OIP-C.LTTKrxNWDr_k74wz6jKqBgHaHa?w=203&h=203&c=7&r=0&o=5&pid=1.7',
+        robot_bg_color='#ccccee',
+        robot_icon='https://ts1.cn.mm.bing.net/th/id/R-C.5302e2cc6f5c7c4933ebb3394e0c41bc?rik=z4u%2b7efba5Mgxw&riu=http%3a%2f%2fcomic-cons.xyz%2fwp-content%2fuploads%2fStar-Wars-avatar-icon-C3PO.png&ehk=kBBvCvpJMHPVpdfpw1GaH%2brbOaIoHjY5Ua9PKcIs%2bAc%3d&risl=&pid=ImgRaw&r=0',
+):
+    '''
+    :param session_var: variable name used to store chat history in session_state
+    :param greetings: show messages when chat box first inited
+    :param box_margin: blank area of a single message box
+    :param user_bg_color: background color of user's message box
+    :param user_icon: icon of user
+    :param robot_bg_color: background color of robot's message box
+    :param robot_icon: icon of robot
+    :return: instance of StChatBox, use it to append and render messages
+    '''
     empty = st.empty()
-    return StChatBox(empty, **kw)
-
+    return StChatBox(
+        chat_box=empty,
+        session_var=session_var,
+        greetings=greetings,
+        box_margin=box_margin,
+        user_bg_color=user_bg_color,
+        user_icon=user_icon,
+        robot_bg_color=robot_bg_color,
+        robot_icon=robot_icon
+    )
```

