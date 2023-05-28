# Comparing `tmp/UnlimitedGPT-0.0.8.tar.gz` & `tmp/UnlimitedGPT-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "UnlimitedGPT-0.0.8.tar", last modified: Sat May 27 14:00:55 2023, max compression
+gzip compressed data, was "UnlimitedGPT-0.0.9.tar", last modified: Sun May 28 15:55:56 2023, max compression
```

## Comparing `UnlimitedGPT-0.0.8.tar` & `UnlimitedGPT-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 sxvxge    (1000) sxvxge    (1000)        0 2023-05-27 14:00:55.179473 UnlimitedGPT-0.0.8/
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)     5126 2023-05-27 14:00:55.179473 UnlimitedGPT-0.0.8/PKG-INFO
-drwxrwxr-x   0 sxvxge    (1000) sxvxge    (1000)        0 2023-05-27 14:00:55.175473 UnlimitedGPT-0.0.8/UnlimitedGPT/
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)    13097 2023-05-27 10:02:18.000000 UnlimitedGPT-0.0.8/UnlimitedGPT/UnlimitedGPT.py
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)      249 2023-05-27 12:22:12.000000 UnlimitedGPT-0.0.8/UnlimitedGPT/__init__.py
-drwxrwxr-x   0 sxvxge    (1000) sxvxge    (1000)        0 2023-05-27 14:00:55.179473 UnlimitedGPT-0.0.8/UnlimitedGPT/internal/
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)     1710 2023-05-27 09:21:23.000000 UnlimitedGPT-0.0.8/UnlimitedGPT/internal/chatgpt_data.py
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)      294 2023-05-27 10:01:38.000000 UnlimitedGPT-0.0.8/UnlimitedGPT/internal/driver.py
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)      494 2023-05-27 09:58:48.000000 UnlimitedGPT-0.0.8/UnlimitedGPT/internal/objects.py
-drwxrwxr-x   0 sxvxge    (1000) sxvxge    (1000)        0 2023-05-27 14:00:55.179473 UnlimitedGPT-0.0.8/UnlimitedGPT.egg-info/
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)     5126 2023-05-27 14:00:54.000000 UnlimitedGPT-0.0.8/UnlimitedGPT.egg-info/PKG-INFO
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)      344 2023-05-27 14:00:54.000000 UnlimitedGPT-0.0.8/UnlimitedGPT.egg-info/SOURCES.txt
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)        1 2023-05-27 14:00:54.000000 UnlimitedGPT-0.0.8/UnlimitedGPT.egg-info/dependency_links.txt
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)       36 2023-05-27 14:00:54.000000 UnlimitedGPT-0.0.8/UnlimitedGPT.egg-info/requires.txt
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)       35 2023-05-27 14:00:54.000000 UnlimitedGPT-0.0.8/UnlimitedGPT.egg-info/top_level.txt
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)       38 2023-05-27 14:00:55.179473 UnlimitedGPT-0.0.8/setup.cfg
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)     1686 2023-05-27 14:00:49.000000 UnlimitedGPT-0.0.8/setup.py
+drwxrwxr-x   0 sxvxge    (1000) sxvxge    (1000)        0 2023-05-28 15:55:56.646984 UnlimitedGPT-0.0.9/
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)     5974 2023-05-28 15:55:56.642984 UnlimitedGPT-0.0.9/PKG-INFO
+drwxrwxr-x   0 sxvxge    (1000) sxvxge    (1000)        0 2023-05-28 15:55:56.606984 UnlimitedGPT-0.0.9/UnlimitedGPT/
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)    20332 2023-05-28 14:23:24.000000 UnlimitedGPT-0.0.9/UnlimitedGPT/UnlimitedGPT.py
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)      268 2023-05-28 13:45:50.000000 UnlimitedGPT-0.0.9/UnlimitedGPT/__init__.py
+drwxrwxr-x   0 sxvxge    (1000) sxvxge    (1000)        0 2023-05-28 15:55:56.630984 UnlimitedGPT-0.0.9/UnlimitedGPT/internal/
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)     2036 2023-05-28 13:36:32.000000 UnlimitedGPT-0.0.9/UnlimitedGPT/internal/chatgpt_data.py
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)     1065 2023-05-28 11:02:47.000000 UnlimitedGPT-0.0.9/UnlimitedGPT/internal/driver.py
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)     3024 2023-05-28 11:29:18.000000 UnlimitedGPT-0.0.9/UnlimitedGPT/internal/objects.py
+drwxrwxr-x   0 sxvxge    (1000) sxvxge    (1000)        0 2023-05-28 15:55:56.610984 UnlimitedGPT-0.0.9/UnlimitedGPT.egg-info/
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)     5974 2023-05-28 15:55:54.000000 UnlimitedGPT-0.0.9/UnlimitedGPT.egg-info/PKG-INFO
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)      344 2023-05-28 15:55:54.000000 UnlimitedGPT-0.0.9/UnlimitedGPT.egg-info/SOURCES.txt
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)        1 2023-05-28 15:55:54.000000 UnlimitedGPT-0.0.9/UnlimitedGPT.egg-info/dependency_links.txt
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)       36 2023-05-28 15:55:54.000000 UnlimitedGPT-0.0.9/UnlimitedGPT.egg-info/requires.txt
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)       35 2023-05-28 15:55:54.000000 UnlimitedGPT-0.0.9/UnlimitedGPT.egg-info/top_level.txt
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)       38 2023-05-28 15:55:56.646984 UnlimitedGPT-0.0.9/setup.cfg
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)     1686 2023-05-28 14:37:21.000000 UnlimitedGPT-0.0.9/setup.py
```

### Comparing `UnlimitedGPT-0.0.8/PKG-INFO` & `UnlimitedGPT-0.0.9/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UnlimitedGPT
-Version: 0.0.8
+Version: 0.0.9
 Summary: An unofficial Python wrapper for OpenAI's ChatGPT API
 Home-page: https://github.com/Sxvxgee/UnlimitedGPT
 Author: Sxvxge
 License: GPL-3.0 license
 Project-URL: Documentation, https://github.com/Sxvxgee/UnlimitedGPT/blob/main/README.md
 Project-URL: Issue tracker, https://github.com/Sxvxgee/UnlimitedGPT/issues
 Classifier: Development Status :: 5 - Production/Stable
@@ -21,14 +21,15 @@
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 
 # UnlimitedGPT
 
+[![Downloads](https://static.pepy.tech/badge/unlimitedgpt)](https://pepy.tech/project/unlimitedgpt)
 [![PyPi](https://img.shields.io/pypi/v/UnlimitedGPT.svg)](https://pypi.python.org/pypi/UnlimitedGPT)
 [![License](https://img.shields.io/github/license/Sxvxgee/UnlimitedGPT.svg?color=green)](https://github.com/Sxvxgee/UnlimitedGPT/blob/main/LICENSE)
 
 > This is a maintained, modified and improved package of the original [pyChatGPT](https://github.com/terry3041/pyChatGPT) package. The original package is in slow development and has many issues. This package is actively maintained and updated.
 
 An unofficial Python wrapper for OpenAI's ChatGPT API
 
@@ -65,29 +66,39 @@
 
 #### Import as a module
 
 ```python
 from UnlimitedGPT import ChatGPT
 
 session_token = 'abc123'  # `__Secure-next-auth.session-token` cookie from https://chat.openai.com/chat
-api = ChatGPT(session_token)  # auth with session token
-api = ChatGPT(session_token, conversation_id='some-random-uuid')  # specify conversation id
-api = ChatGPT(session_token, proxy='https://proxy.example.com:8080')  # specify proxy
-api = ChatGPT(session_token, chrome_args=['--window-size=1920,768'])  # specify chrome args
-api = ChatGPT(session_token, disable_moderation=True)  # disable moderation
-api = ChatGPT(session_token, verbose=True)  # verbose mode (print debug messages)
+api = ChatGPT(
+    session_token, # Specify session token
+    conversation_id='some-random-uuid', # Specify conversation ID (Defaults to None)
+    proxy='https://proxy.example.com:8080', # Specify proxy (Defaults to None)
+    chrome_args=['--window-size=1920,768'], # Specify chrome args (optional)
+    disable_moderation=True, # Disable moderation (Defaults to False)
+    verbose=True, # Verbose mode (Defaults to False)
+)
 
 message = api.send_message('Hello, world!')
 print(message.response, message.conversation_id)
 
 api.reset_conversation()  # reset the conversation
+api.clear_conversations() # clear all conversations
+api.switch_theme('DARK') # switch themes (DARK, LIGHT, SYSTEM, OPPOSITE)
+data = api.get_session_data() # Returns SessionData object with some data, also User object inside of it
+api.logout() # Logout from the session
+api.switch_account("some-other-token") # Switch to another account
 ```
 
 ## Frequently Asked Questions
 
+### When is proper documentation coming?
+Documentation of every function, class and object will be coming very soon. For now, all information of current exisiting functions can be found [here](#import-as-a-module).
+
 ### How do I get it to work on headless linux server?
 
 ```bash
 # install chromium & X virtual framebuffer
 sudo apt install chromium-browser xvfb
 
 # start your script
@@ -104,30 +115,26 @@
 !pip install -U selenium_profiles UnlimitedGPT
 
 # install chromedriver
 from selenium_profiles.utils.installer import install_chromedriver
 install_chromedriver()
 ```
 
-```python
-# start your script as normal
-!python3 -m UnlimitedGPT
-```
-
 ## Insipration
 
 This project is inspired by
 
 -   [ChatGPT](https://github.com/acheong08/ChatGPT)
 -   [chatgpt-api](https://github.com/transitive-bullshit/chatgpt-api)
 -   [pyChatGPT](https://github.com/terry3041/pyChatGPT)
 
 ## Disclaimer
 
-This project is not affiliated with OpenAI in any way. Use at your own risk. I am not responsible for any damage caused by this project. Please read the [OpenAI Terms of Service](https://beta.openai.com/terms) before using this project.
+- This project is not affiliated with OpenAI in any way. Use at your own risk. I am not responsible for any damage caused by this project. Please read the [OpenAI Terms of Service](https://beta.openai.com/terms) before using this project.
+- This project is not built from scratch by me, I just modified, improved and fixed the original code of [pyChatGPT](https://github.com/terry3041/pyChatGPT) since I noticed there were already some PRs and they were not responded to by the terry3041. I also added some new features to the package, and will keep on doing so.
 
 ## License
 
 This project is licensed under the GPLv3 License - see the [LICENSE](LICENSE) file for details.
 
 ## Star History
```

### Comparing `UnlimitedGPT-0.0.8/UnlimitedGPT/UnlimitedGPT.py` & `UnlimitedGPT-0.0.9/UnlimitedGPT/UnlimitedGPT.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,42 +1,45 @@
 import re
-from typing import Optional
+from typing import Optional, Literal
 from time import sleep, time
 from threading import Thread
 from platform import system
 from os import environ
 from json import loads
 from logging import getLogger, DEBUG, Formatter, StreamHandler
 from weakref import finalize
 
 from markdownify import markdownify
 from selenium.webdriver.common.by import By
 from selenium.webdriver.support import expected_conditions as EC
 from selenium.webdriver.support.wait import WebDriverWait
 from selenium.common.exceptions import TimeoutException, NoSuchElementException
 from selenium.webdriver.common.keys import Keys
+from selenium.webdriver.common.action_chains import ActionChains
 from undetected_chromedriver import ChromeOptions
 
 from .internal.driver import ChatGPTDriver
 from .internal.chatgpt_data import ChatGPTVariables as CGPTV
-from .internal.objects import ChatGPTResponse
+from .internal.objects import ChatGPTResponse, User, SessionData
 
 class ChatGPT:
     """
     A class for interacting with ChatGPT.
 
     Args:
     ----------
         session_token (str): The session token for authentication.
         conversation_id (str, optional): The conversation ID. Defaults to ''.
         proxy (Optional[str], optional): The proxy server URL. Defaults to None.
         disable_moderation (bool, optional): Whether to disable moderation. Defaults to True.
         verbose (bool, optional): Whether to enable verbose logging. Defaults to False.
         headless (bool, optional): Whether to run the browser in headless mode. Defaults to False.
         chrome_args (list, optional): Additional arguments for the Chrome browser. Defaults to [].
+        input_mode(list, options): The input mode. Defaults to 'INSTANT'.
+        input_delay(int, options): The input delay. Defaults to 0.2.
     
     Raises:
     ----------
         ValueError: If the session token is not provided.
         ValueError: If the proxy is invalid.
     """
 
@@ -45,22 +48,26 @@
         session_token: str,
         conversation_id: str = '',
         proxy: Optional[str] = None,
         disable_moderation: bool = True,
         verbose: bool = False,
         headless: bool = False,
         chrome_args: list = [],
+        input_mode: Literal['INSTANT', 'SLOW'] = 'INSTANT',
+        input_delay: int = 0.2,
     ) -> None:
         self._session_token = session_token
         self._conversation_id = conversation_id
         self._proxy = proxy
         self._disable_moderation = disable_moderation
         self._headless = headless
         self._chrome_args = chrome_args
         self._clicked_buttons = False
+        self._input_mode = input_mode
+        self._input_delay = input_delay
         self._init_logger(verbose)
 
         if not self._session_token:
             raise ValueError("session_token is required")
         if self._proxy and not re.findall(
             r'(https?|socks(4|5)?):\/\/.+:\d{1,5}', self._proxy # type: ignore
         ):
@@ -77,14 +84,24 @@
         if hasattr(self, 'driver'):
             self.logger.debug('Closing browser...')
             self.driver.quit()
         if hasattr(self, 'display'):
             self.logger.debug('Closing display...')
             self.display.stop()
 
+    def get_out_of_menu(self) -> None:
+        """
+        Get out of any menu present.
+        """
+        for i in range(5):
+            # First escape click is to remove the options menu
+            # Second escape click is to get out of the settings menu
+            # The rest are just to be safe
+            self.driver.find_element(By.TAG_NAME, 'body').send_keys(Keys.ESCAPE)
+
     def _init_logger(self, verbose: bool) -> None:
         """
         Initialize the logger.
 
         Args:
         ----------
             verbose (bool): Whether to enable verbose logging.
@@ -204,14 +221,22 @@
             pass
 
         alerts = self.driver.find_elements(*CGPTV.chatgpt_alert)
         if alerts:
             self.logger.debug('Dismissing alert...')
             self.driver.execute_script('arguments[0].remove()', alerts[0])
 
+        if not self._clicked_buttons:
+            for button in CGPTV.chatgpt_info_buttons:
+                btn = WebDriverWait(self.driver, 60).until(
+                    EC.element_to_be_clickable(button)
+                )
+                btn.click()
+            self._clicked_buttons = True
+
     def _ensure_cf(self, retry: int = 3) -> None:
         """
         Ensure Cloudflare cookies are set.
 
         Args:
         ----------
             retry (int, optional): Number of retries. Defaults to 3.
@@ -270,32 +295,25 @@
 
         Raises:
         ----------
             TimeoutException: If the message fails to send.
             ValueError: If the response is invalid.
             ValueError: If the response is not found.
         """
-        self.logger.debug('Ensuring Cloudflare cookies...')
-        self._ensure_cf()
-
-        self.logger.debug('Sending message...')
-        
-        if not self._clicked_buttons:
-            for button in CGPTV.chatgpt_info_buttons:
-                btn = WebDriverWait(self.driver, 60).until(
-                    EC.element_to_be_clickable(button)
-                )
-                btn.click()
-            self._clicked_buttons = True
+        self.logger.debug(f'Sending message with mode {self._input_mode}{f" with {self._input_delay} delay" if self._input_mode == "SLOW" else ""}...')
 
         textbox = WebDriverWait(self.driver, 60).until(
             EC.element_to_be_clickable(CGPTV.chatgpt_textbox)
         )
-        # textbox.send_keys(message)
-        self.driver.execute_script("arguments[0].value = arguments[1];", textbox, message)
+        if self._input_mode == 'INSTANT':
+            self.driver.execute_script("arguments[0].value = arguments[1];", textbox, message)
+        else:
+            for char in message:
+                textbox.send_keys(char)
+                sleep(self._input_delay)
 
         textbox.send_keys(Keys.ENTER)
 
         self.logger.debug('Waiting for completion...')
         WebDriverWait(self.driver, 240).until_not(
             EC.presence_of_element_located(CGPTV.chatgpt_streaming)
         )
@@ -345,7 +363,166 @@
 
         self.logger.debug('Resetting conversation...')
         try:
             self.driver.find_element(*CGPTV.chatgpt_new_chat).click()
         except NoSuchElementException:
             self.logger.debug('New chat button not found')
             self.driver.save_screenshot('reset_conversation_failed.png')
+
+    def clear_conversations(self) -> None:
+        """
+        Clears all conversations.
+        """
+        self.logger.debug('Clearing all conversations...')
+        try:
+            menu_button = self.driver.find_element(*CGPTV.chatgpt_menu_button)
+            menu_button.click()
+            clear_conversations = self.driver.find_element(*CGPTV.chatgpt_menu_clear_conversations)
+            clear_conversations.click()
+            clear_conversations.click() # Confirm button is the same path
+        except NoSuchElementException:
+            self.logger.debug('Could not find menu buttons')
+            self.driver.save_screenshot('clear_conversations_failed.png')
+
+    def switch_theme(self, theme: Literal['LIGHT', 'DARK', 'OPPOSITE', 'SYSTEM']) -> None:
+        """
+        Switch the theme.
+
+        Args:
+        ----------
+            theme (Literal['LIGHT', 'DARK', 'OPPOSITE']): The theme to switch to.
+
+        Notes:
+        ----------
+            - `LIGHT`: Light theme.
+            - `DARK`: Dark theme.
+            - `OPPOSITE`: Switch to the opposite theme.
+            - `SYSTEM`: Switch to the system theme.
+        """
+        self.logger.debug(f'Switching theme to {theme}...')
+        try:
+            menu_button_clicked = self.driver.safe_click(CGPTV.chatgpt_menu_button)
+            if not menu_button_clicked:
+                self.logger.debug('Could not click menu button')
+                return self.get_out_of_menu()
+
+            self.logger.debug('Clicked menu button')
+            
+            settings_button_clicked = self.driver.safe_click(CGPTV.chatgpt_menu_settings_button)
+            if not settings_button_clicked:
+                self.logger.debug('Could not click settings button')
+                return self.get_out_of_menu()
+
+            self.logger.debug('Clicked settings button')
+            
+            current_theme_value = self.driver.find_element(*CGPTV.chatgpt_outer_html).get_attribute('class')
+            current_theme = 'LIGHT' if 'light' in current_theme_value else 'DARK'
+            if theme == current_theme:
+                self.logger.debug('Theme is already set to the desired theme')
+                return self.get_out_of_menu()
+
+            select_element = self.driver.find_element(By.CSS_SELECTOR, 'select.rounded')
+            ActionChains(self.driver).move_to_element(select_element).click().perform()
+
+            if theme == 'OPPOSITE':
+                if current_theme == 'SYSTEM':
+                    self.logger.debug('Theme cannot be set to opposite of system theme')
+                    return self.get_out_of_menu()
+                    
+                opposite_theme = 'dark' if current_theme == 'LIGHT' else 'light'
+                option = self.driver.find_element(By.CSS_SELECTOR, f'select.rounded option[value={opposite_theme}]')
+                option.click()
+                self.logger.debug(f'Selected opposite theme of {current_theme}')
+            else:
+                option = self.driver.find_element(By.CSS_SELECTOR, f'select.rounded option[value={theme.lower()}]')
+                option.click()
+                self.logger.debug(f'Selected theme {theme}')
+            
+            self.get_out_of_menu()
+        except NoSuchElementException:
+            self.logger.debug('Could not find theme buttons')
+            self.driver.save_screenshot('theme_switch_failed.png')
+
+    def switch_account(self, session_token: str):
+        """
+        Switch the account.
+
+        Args:
+        ----------
+            session_token (str): The session token for authentication.
+
+        Raises:
+        ----------
+            ValueError: If the session token is not provided.
+            ValueError: If the response is invalid.
+        """
+        self.logger.debug('Switching account...')
+        self.driver.execute_cdp_cmd(
+            'Network.setCookie',
+            {
+                'domain': 'chat.openai.com',
+                'path': '/',
+                'name': '__Secure-next-auth.session-token',
+                'value': session_token,
+                'httpOnly': True,
+                'secure': True,
+            },
+        )
+
+        self.logger.debug('Validating authorization...')
+        self.driver.get('https://chat.openai.com/api/auth/session')
+        response = self.driver.page_source
+        if response[0] != '{':
+            response = self.driver.find_element(By.TAG_NAME, 'pre').text
+        response = loads(response)
+        if (not response) or (
+            'error' in response and response['error'] == 'RefreshAccessTokenError'
+        ):
+            raise ValueError('Invalid session token')
+        self.logger.debug('Authorization is valid')
+
+        self.logger.debug('Opening chat page...')
+        self.driver.get(f'{CGPTV.chatgpt_chat_url}/{self._conversation_id}')
+        self._check_blocking_elements()
+    
+    def get_session_data(self) -> SessionData:
+        """
+        Get the session data.
+
+        Returns:
+        ----------
+            SessionData: The ChatGPT session data.
+        """
+        self.logger.debug('Getting account data...')
+        self.driver.get('https://chat.openai.com/api/auth/session')
+        response = self.driver.page_source
+        if response[0] != '{':
+            response = self.driver.find_element(By.TAG_NAME, 'pre').text
+        response = loads(response)
+        session_data = SessionData(
+            User(**response['user']),
+            response["expires"],
+            response["accessToken"],
+            response["authProvider"]
+        )
+        return session_data
+
+    def logout(self) -> None:
+        """
+        Logs out of the current account signed into https://chat.openai.com
+        """
+        self.logger.debug('Logging out...')
+        self.driver.execute_cdp_cmd(
+            'Network.deleteCookies',
+            {
+                'name': '__Secure-next-auth.session-token',
+                'url': 'https://chat.openai.com',
+            },
+        )
+        self.driver.get('https://chat.openai.com/api/auth/session')
+        response = self.driver.page_source
+        if response[0] != '{':
+            response = self.driver.find_element(By.TAG_NAME, 'pre').text
+        response = loads(response)
+        if response == {}:
+            self.logger.debug('Logout successful')
+            return
```

### Comparing `UnlimitedGPT-0.0.8/UnlimitedGPT.egg-info/PKG-INFO` & `UnlimitedGPT-0.0.9/UnlimitedGPT.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UnlimitedGPT
-Version: 0.0.8
+Version: 0.0.9
 Summary: An unofficial Python wrapper for OpenAI's ChatGPT API
 Home-page: https://github.com/Sxvxgee/UnlimitedGPT
 Author: Sxvxge
 License: GPL-3.0 license
 Project-URL: Documentation, https://github.com/Sxvxgee/UnlimitedGPT/blob/main/README.md
 Project-URL: Issue tracker, https://github.com/Sxvxgee/UnlimitedGPT/issues
 Classifier: Development Status :: 5 - Production/Stable
@@ -21,14 +21,15 @@
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 
 # UnlimitedGPT
 
+[![Downloads](https://static.pepy.tech/badge/unlimitedgpt)](https://pepy.tech/project/unlimitedgpt)
 [![PyPi](https://img.shields.io/pypi/v/UnlimitedGPT.svg)](https://pypi.python.org/pypi/UnlimitedGPT)
 [![License](https://img.shields.io/github/license/Sxvxgee/UnlimitedGPT.svg?color=green)](https://github.com/Sxvxgee/UnlimitedGPT/blob/main/LICENSE)
 
 > This is a maintained, modified and improved package of the original [pyChatGPT](https://github.com/terry3041/pyChatGPT) package. The original package is in slow development and has many issues. This package is actively maintained and updated.
 
 An unofficial Python wrapper for OpenAI's ChatGPT API
 
@@ -65,29 +66,39 @@
 
 #### Import as a module
 
 ```python
 from UnlimitedGPT import ChatGPT
 
 session_token = 'abc123'  # `__Secure-next-auth.session-token` cookie from https://chat.openai.com/chat
-api = ChatGPT(session_token)  # auth with session token
-api = ChatGPT(session_token, conversation_id='some-random-uuid')  # specify conversation id
-api = ChatGPT(session_token, proxy='https://proxy.example.com:8080')  # specify proxy
-api = ChatGPT(session_token, chrome_args=['--window-size=1920,768'])  # specify chrome args
-api = ChatGPT(session_token, disable_moderation=True)  # disable moderation
-api = ChatGPT(session_token, verbose=True)  # verbose mode (print debug messages)
+api = ChatGPT(
+    session_token, # Specify session token
+    conversation_id='some-random-uuid', # Specify conversation ID (Defaults to None)
+    proxy='https://proxy.example.com:8080', # Specify proxy (Defaults to None)
+    chrome_args=['--window-size=1920,768'], # Specify chrome args (optional)
+    disable_moderation=True, # Disable moderation (Defaults to False)
+    verbose=True, # Verbose mode (Defaults to False)
+)
 
 message = api.send_message('Hello, world!')
 print(message.response, message.conversation_id)
 
 api.reset_conversation()  # reset the conversation
+api.clear_conversations() # clear all conversations
+api.switch_theme('DARK') # switch themes (DARK, LIGHT, SYSTEM, OPPOSITE)
+data = api.get_session_data() # Returns SessionData object with some data, also User object inside of it
+api.logout() # Logout from the session
+api.switch_account("some-other-token") # Switch to another account
 ```
 
 ## Frequently Asked Questions
 
+### When is proper documentation coming?
+Documentation of every function, class and object will be coming very soon. For now, all information of current exisiting functions can be found [here](#import-as-a-module).
+
 ### How do I get it to work on headless linux server?
 
 ```bash
 # install chromium & X virtual framebuffer
 sudo apt install chromium-browser xvfb
 
 # start your script
@@ -104,30 +115,26 @@
 !pip install -U selenium_profiles UnlimitedGPT
 
 # install chromedriver
 from selenium_profiles.utils.installer import install_chromedriver
 install_chromedriver()
 ```
 
-```python
-# start your script as normal
-!python3 -m UnlimitedGPT
-```
-
 ## Insipration
 
 This project is inspired by
 
 -   [ChatGPT](https://github.com/acheong08/ChatGPT)
 -   [chatgpt-api](https://github.com/transitive-bullshit/chatgpt-api)
 -   [pyChatGPT](https://github.com/terry3041/pyChatGPT)
 
 ## Disclaimer
 
-This project is not affiliated with OpenAI in any way. Use at your own risk. I am not responsible for any damage caused by this project. Please read the [OpenAI Terms of Service](https://beta.openai.com/terms) before using this project.
+- This project is not affiliated with OpenAI in any way. Use at your own risk. I am not responsible for any damage caused by this project. Please read the [OpenAI Terms of Service](https://beta.openai.com/terms) before using this project.
+- This project is not built from scratch by me, I just modified, improved and fixed the original code of [pyChatGPT](https://github.com/terry3041/pyChatGPT) since I noticed there were already some PRs and they were not responded to by the terry3041. I also added some new features to the package, and will keep on doing so.
 
 ## License
 
 This project is licensed under the GPLv3 License - see the [LICENSE](LICENSE) file for details.
 
 ## Star History
```

### Comparing `UnlimitedGPT-0.0.8/setup.py` & `UnlimitedGPT-0.0.9/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     name='UnlimitedGPT',
     author='Sxvxge',
     url='https://github.com/Sxvxgee/UnlimitedGPT',
     project_urls={
         'Documentation': 'https://github.com/Sxvxgee/UnlimitedGPT/blob/main/README.md',
         'Issue tracker': 'https://github.com/Sxvxgee/UnlimitedGPT/issues',
     },
-    version="0.0.8",
+    version="0.0.9",
     packages=['UnlimitedGPT', 'UnlimitedGPT/internal'],
     py_modules=['UnlimitedGPT'],
     license='GPL-3.0 license',
     description='An unofficial Python wrapper for OpenAI\'s ChatGPT API',
     long_description=readme,
     long_description_content_type='text/markdown',
     include_package_data=True,
```

