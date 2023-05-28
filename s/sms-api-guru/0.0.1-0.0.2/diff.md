# Comparing `tmp/sms_api_guru-0.0.1.tar.gz` & `tmp/sms_api_guru-0.0.2.tar.gz`

## Comparing `sms_api_guru-0.0.1.tar` & `sms_api_guru-0.0.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 sms_api_guru-0.0.1/aa.py
--rw-r--r--   0        0        0     5783 2020-02-02 00:00:00.000000 sms_api_guru-0.0.1/src/sms_api_guru/__init__.py
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 sms_api_guru-0.0.1/.gitignore
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 sms_api_guru-0.0.1/LICENSE
--rw-r--r--   0        0        0     2618 2020-02-02 00:00:00.000000 sms_api_guru-0.0.1/README.md
--rw-r--r--   0        0        0      929 2020-02-02 00:00:00.000000 sms_api_guru-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     3335 2020-02-02 00:00:00.000000 sms_api_guru-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 sms_api_guru-0.0.2/aa.py
+-rw-r--r--   0        0        0     5795 2020-02-02 00:00:00.000000 sms_api_guru-0.0.2/src/sms_api_guru/__init__.py
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 sms_api_guru-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 sms_api_guru-0.0.2/LICENSE
+-rw-r--r--   0        0        0     2618 2020-02-02 00:00:00.000000 sms_api_guru-0.0.2/README.md
+-rw-r--r--   0        0        0      929 2020-02-02 00:00:00.000000 sms_api_guru-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     3335 2020-02-02 00:00:00.000000 sms_api_guru-0.0.2/PKG-INFO
```

### Comparing `sms_api_guru-0.0.1/src/sms_api_guru/__init__.py` & `sms_api_guru-0.0.2/src/sms_api_guru/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,30 +24,30 @@
     def __init__(self, obj):
         self.ok:bool = obj["ok"]
         self.message:str = obj["message"]
         self.valid:bool = obj["valid"]
     def __str__(self) -> str:
         return json.dumps(self.__dict__, default=vars)
 
-apiKey:str = ""
+api_key:str = ""
 
 def set_key(key:str):
     """
     Set the API key, so that the service knows that you are authorized to use it.
 
     Parameters:
 
     key (string): Unique key created using the [API Console](https://smsapiguru.com/api)
 
     Examples:
     >>> import sms_api_guru as api
     >>> api.set_key("YOUR_API_KEY")
     """
-    global apiKey
-    apiKey = key
+    global api_key
+    api_key = key
 
 
 def send_sms(phone_number:str, text:str)->SendMessageResult:
     """
     Function that is used to send an SMS. 
 
     Parameters:
@@ -61,29 +61,29 @@
 
     Examples:
 
     >>> import sms_api_guru as api
     >>> api.set_key("YOUR_API_KEY")
     >>> api.send_sms("+11234567890", text="Message text...")
     """
-    global apiKey
+    global api_key
     if(len(phone_number) == 0):
         return dict(ok=False, status=400, message="You have not specified the recipient phone number. ")
     if(len(text) == 0):
         return dict(ok=False, status=400, message="You have not specified the message body. ")
-    if(len(apiKey) == 0):
+    if(len(api_key) == 0):
         return dict(ok=False, status=400, message="You have not specified the API key. ")
     data = dict(phone_number=phone_number, text=text)
     
     r = requests.post(
         url="https://smsapiguru.com/v1/sms",
         json=data,
         headers={
             'Content-Type': 'application/json',
-            'Authorization': 'Bearer '+ apiKey
+            'Authorization': 'Bearer '+ api_key
         })
     return SendMessageResult(json.loads(r.text)) 
 
 
 def send_verification_code(phone_number:str, service_name:str = "", seconds:int = 600)->VerifyPhoneResult:
     """
     Function that is used to send a phone number verification SMS to your customer. 
@@ -112,27 +112,27 @@
     if res.valid:
         print("Real user")
     
     ```
     
 
     """
-    global apiKey
+    global api_key
     if(len(phone_number) == 0):
         return dict(ok=False, status=400, message="You have not specified the recipient phone number. ")
-    if(len(apiKey) == 0):
+    if(len(api_key) == 0):
         return dict(ok=False, status=400, message="You have not specified the API key. ")
     data = dict(phone_number=phone_number, service_name=service_name, seconds = seconds)
     
     r = requests.post(
         url="https://smsapiguru.com/v1/code",
         json=data,
         headers={
             'Content-Type': 'application/json',
-            'Authorization': 'Bearer '+ apiKey
+            'Authorization': 'Bearer '+ api_key
         })
     return VerifyPhoneResult(json.loads(r.text)) 
 
 def verify_code(phone_number:str, code:str)->VerifyCodeResult:
     """
     Function that is used to verify the code that the customer has submitted. 
 
@@ -157,24 +157,24 @@
     if res.valid:
         print("Real user")
     
     ```
     
 
     """
-    global apiKey
+    global api_key
     if(len(phone_number) == 0):
         return dict(ok=False, status=400, message="You have not specified the recipient phone number. ", valid=False)
     if(len(code) == 0):
         return dict(ok=False, status=400, message="You have not specified the recipient phone number. ", valid=False)
-    if(len(apiKey) == 0):
+    if(len(api_key) == 0):
         return dict(ok=False, status=400, message="You have not specified the API key. ", valid=False)
     data = dict(phone_number=phone_number, code=code)
     
     r = requests.post(
         url="https://smsapiguru.com/v1/check",
         json=data,
         headers={
             'Content-Type': 'application/json',
-            'Authorization': 'Bearer '+ apiKey
+            'Authorization': 'Bearer '+ api_key
         })
     return VerifyCodeResult(json.loads(r.text))
```

### Comparing `sms_api_guru-0.0.1/LICENSE` & `sms_api_guru-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sms_api_guru-0.0.1/README.md` & `sms_api_guru-0.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 * Python 3.7
 * Python 3.8
 * Python 3.9
 * Python 3.10
 * Python 3.11
 
 ## Installation
-`pip install sms_api_guru`
+`pip install sms-api-guru`
 
 ## Sending an SMS
 
 To send an SMS, you have to create an API key using the [SMS API Guru dashboard](https://smsapiguru.com/api). When you register an account, you automatically get an API key with one free SMS which you can send anywhere.
 
 ### Just send a message
```

### Comparing `sms_api_guru-0.0.1/pyproject.toml` & `sms_api_guru-0.0.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "sms_api_guru"
-version = "0.0.1"
+version = "0.0.2"
 description = "Python library that helps you send SMS using SMS API Guru API"
 license = "MIT"
 authors = [
   { name="SMS API Guru", email="admin@smsapiguru.com" },
 ]
 readme = "README.md"
 homepage = "https://textflow.me"
```

### Comparing `sms_api_guru-0.0.1/PKG-INFO` & `sms_api_guru-0.0.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sms_api_guru
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python library that helps you send SMS using SMS API Guru API
 Author-email: SMS API Guru <admin@smsapiguru.com>
 License-Expression: MIT
 License-File: LICENSE
 Keywords: api,api-client,simple-sms,sms,sms-api,sms-verification,text-message,user-verification
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -31,15 +31,15 @@
 * Python 3.7
 * Python 3.8
 * Python 3.9
 * Python 3.10
 * Python 3.11
 
 ## Installation
-`pip install sms_api_guru`
+`pip install sms-api-guru`
 
 ## Sending an SMS
 
 To send an SMS, you have to create an API key using the [SMS API Guru dashboard](https://smsapiguru.com/api). When you register an account, you automatically get an API key with one free SMS which you can send anywhere.
 
 ### Just send a message
```

