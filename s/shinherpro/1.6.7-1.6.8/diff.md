# Comparing `tmp/shinherpro-1.6.7.tar.gz` & `tmp/shinherpro-1.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shinherpro-1.6.7.tar", last modified: Sat May 27 14:35:03 2023, max compression
+gzip compressed data, was "shinherpro-1.6.8.tar", last modified: Sun May 28 15:22:38 2023, max compression
```

## Comparing `shinherpro-1.6.7.tar` & `shinherpro-1.6.8.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-27 14:35:03.293031 shinherpro-1.6.7/
--rw-rw-rw-   0        0        0      178 2023-05-27 14:35:03.292534 shinherpro-1.6.7/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-05-27 14:35:03.293031 shinherpro-1.6.7/setup.cfg
--rw-rw-rw-   0        0        0      785 2023-05-27 14:34:59.000000 shinherpro-1.6.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-27 14:35:03.278150 shinherpro-1.6.7/shinherpro/
--rw-rw-rw-   0        0        0    16753 2023-05-27 06:07:28.000000 shinherpro-1.6.7/shinherpro/TYAI.py
--rw-rw-rw-   0        0        0        0 2023-05-22 15:34:31.000000 shinherpro-1.6.7/shinherpro/__init__.py
--rw-rw-rw-   0        0        0     1293 2023-05-23 15:25:54.000000 shinherpro-1.6.7/shinherpro/chormeDriver.py
--rw-rw-rw-   0        0        0     1186 2023-05-22 15:33:52.000000 shinherpro-1.6.7/shinherpro/serverLog.py
--rw-rw-rw-   0        0        0     2127 2023-05-21 08:58:49.000000 shinherpro-1.6.7/shinherpro/vfcModel.py
-drwxrwxrwx   0        0        0        0 2023-05-27 14:35:03.291543 shinherpro-1.6.7/shinherpro.egg-info/
--rw-rw-rw-   0        0        0      178 2023-05-27 14:35:03.000000 shinherpro-1.6.7/shinherpro.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      293 2023-05-27 14:35:03.000000 shinherpro-1.6.7/shinherpro.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-27 14:35:03.000000 shinherpro-1.6.7/shinherpro.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       77 2023-05-27 14:35:03.000000 shinherpro-1.6.7/shinherpro.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-27 14:35:03.000000 shinherpro-1.6.7/shinherpro.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-28 15:22:38.497342 shinherpro-1.6.8/
+-rw-rw-rw-   0        0        0      178 2023-05-28 15:22:38.496845 shinherpro-1.6.8/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-05-28 15:22:38.497342 shinherpro-1.6.8/setup.cfg
+-rw-rw-rw-   0        0        0      785 2023-05-28 14:42:22.000000 shinherpro-1.6.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-28 15:22:38.487918 shinherpro-1.6.8/shinherpro/
+-rw-rw-rw-   0        0        0    19609 2023-05-28 15:22:35.000000 shinherpro-1.6.8/shinherpro/TYAI.py
+-rw-rw-rw-   0        0        0        0 2023-05-22 15:34:31.000000 shinherpro-1.6.8/shinherpro/__init__.py
+-rw-rw-rw-   0        0        0     1293 2023-05-23 15:25:54.000000 shinherpro-1.6.8/shinherpro/chormeDriver.py
+-rw-rw-rw-   0        0        0    10438 2023-05-28 14:57:43.000000 shinherpro-1.6.8/shinherpro/html.py
+-rw-rw-rw-   0        0        0     1186 2023-05-22 15:33:52.000000 shinherpro-1.6.8/shinherpro/serverLog.py
+-rw-rw-rw-   0        0        0     2127 2023-05-21 08:58:49.000000 shinherpro-1.6.8/shinherpro/vfcModel.py
+drwxrwxrwx   0        0        0        0 2023-05-28 15:22:38.495854 shinherpro-1.6.8/shinherpro.egg-info/
+-rw-rw-rw-   0        0        0      178 2023-05-28 15:22:38.000000 shinherpro-1.6.8/shinherpro.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      312 2023-05-28 15:22:38.000000 shinherpro-1.6.8/shinherpro.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-28 15:22:38.000000 shinherpro-1.6.8/shinherpro.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       77 2023-05-28 15:22:38.000000 shinherpro-1.6.8/shinherpro.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-28 15:22:38.000000 shinherpro-1.6.8/shinherpro.egg-info/top_level.txt
```

### Comparing `shinherpro-1.6.7/setup.py` & `shinherpro-1.6.8/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,16 +6,16 @@
     def run(self):
         print("\033[98m 正在安裝shinher-pro...")
         install.run(self)
         print("shinherpro安裝完成！ \033[0m")
 
 setup(
     name='shinherpro',
-    version='1.6.7',
-    description='shinher-pro 1.6.7',
+    version='1.6.8',
+    description='shinher-pro 1.6.8',
     author='Yihuan',
     author_email='ivan17.lai@gmail.com',
     packages=['shinherpro'],
     install_requires=[
         'selenium',
         'beautifulsoup4',
         'keras',
```

### Comparing `shinherpro-1.6.7/shinherpro/TYAI.py` & `shinherpro-1.6.8/shinherpro/TYAI.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from selenium.webdriver.chrome.options import Options
 from selenium.webdriver.common.by import By
 from selenium.webdriver.support.ui import Select
 from selenium.webdriver.support.ui import WebDriverWait
 from selenium.webdriver.support import expected_conditions as EC
 from selenium.webdriver.common.alert import Alert
 from bs4 import BeautifulSoup
+import bs4
 from keras.utils import img_to_array
 from keras.utils import load_img
 from keras.models import load_model
 from PIL import Image
 from io import BytesIO
 import requests
 from urllib.parse import unquote
@@ -95,15 +96,16 @@
     }
     ]
 
     result['log'] = new_log
     return result
 
 def login(username, password, driver, model,LowConfidence=85,stepPrint=False):
-    
+    driver.delete_all_cookies()
+    driver.refresh()
     try:
         if stepPrint == False :
             sys.stdout = open(os.devnull, 'w')
 
         start_time = time.time()
         while True:
             allConfidence = 0
@@ -220,15 +222,15 @@
     class_name = student_info[0].split('：')[1]
     seat_number = student_info[2].split('：')[1]
     student_id = student_info[4].split('：')[1]
     student_name = student_info[6].split('：')[1]
 
     subjects = []
     table_rows = soup.find('table', id='restudyList').find_all('tr')
-    print(table_rows)
+    #print(table_rows)
     for row in table_rows[1:]:
         cells = row.find_all('td')
         subject_code = cells[0].text.strip()
         subject_name = cells[1].text.strip()
         retake_semester = cells[2].text.strip()
         historical_records = cells[3].text.strip()
         credits = cells[4].text.strip()
@@ -320,15 +322,14 @@
         chormeDriver.switch_frame(True, ["right", "right_below"], driver)
         # 獲取新窗口的頁面內容(成績表格)
         new_page_source = driver.page_source
         # 成績表格分析
         JsonGrade = score_tolist(new_page_source)
         loginScess = True
 
-        driver.delete_all_cookies()
         driver.refresh()
 
         stepSave = 4
 
         JsonResult = JsonGrade
 
         if stepPrint==False : sys.stdout = sys.__stdout__
@@ -357,15 +358,14 @@
 
         stepSave = 2
         driver.switch_to.default_content()
         chormeDriver.switch_frame(False,['right'],driver)
 
         new_page_source = driver.page_source
 
-        driver.delete_all_cookies()
         driver.refresh()
 
         json_result = Credit_html_to_json(new_page_source)
 
         if stepPrint==False : sys.stdout = sys.__stdout__
         return json_result
     except:
@@ -426,7 +426,77 @@
 
     screenshot = Image.open('PhotoSave\\screenshot.png')
     image_cropped = screenshot.crop((x, y, x + width, y + height))
     imgPath = 'PhotoSave\\UserPhoto' + username + '.png'
     image_cropped.save(imgPath)
     return {'code':0,'imgPath':imgPath,'url':url}
 
+def getUserAbsentFromWork(username,driver):
+    driver.refresh()
+    stepSave = 0
+    try:
+        stepSave = 1
+
+        # 進入成績查詢頁面
+        # 切換到左測選單
+        chormeDriver.switch_frame(False, ["left"], driver)
+        student_data_link = driver.find_element(By.ID, 'lnkStudentData')  # 按鈕名稱 "學生 xxx 的資料"
+        student_data_link.click()
+        # 尋找按鈕名稱 "查詢學生資料"
+        button_name = '查詢學生資料'
+        button_elements = driver.find_elements(By.CSS_SELECTOR, 'td.SubMenuItem') 
+        for button in button_elements:
+            button_text = button.text
+            if button_text == button_name:
+                button.click()
+                break
+                
+        stepSave = 2
+
+        # 切換到框架"right"的框架"right_below"
+        chormeDriver.switch_frame(True, ["right", "right_below"], driver)
+        # 找到查詢資料按鈕
+        button = driver.find_element(By.CSS_SELECTOR, "button[onclick*='window.open']")
+        button.click()
+        # 切換到框架"right"的框架"right_below"
+        chormeDriver.switch_frame(True, ["right", "right_top"], driver)
+        # 找到各式成績查詢按鈕
+        button = driver.find_element(By.XPATH, "//img[@title='查詢缺曠統計資料']")
+        button.click()
+        chormeDriver.switch_frame(True, ["right", "right_below"], driver)
+        new_page_source = driver.page_source
+
+        soup = BeautifulSoup(new_page_source, 'html.parser')
+        rows = soup.find_all('tr')
+
+        time_slots = ["早", "升", "1", "2", "3", "4", "午", "5", "6", "7", "8", "降", "9", "10", "11", "12"]
+        special_dict = {"曠課": [], "公假": [], "請假": []}
+
+        for row in rows[1:]:
+            columns = row.find_all('td')
+            
+            # Get the date from the first column
+            date = columns[0].get_text(strip=True)
+
+            # Start from the second column and only handle existing columns
+            for i, col in enumerate(columns[1: min(len(columns), len(time_slots) + 1)]):  # +1 for the date column
+                text = col.get_text(strip=True)
+                slot = time_slots[slot]
+                if text == "缺":
+                    special_dict["曠課"].append(f"{date} {slot}")
+                elif text == "公":
+                    special_dict["公假"].append(f"{date} {slot}")
+                elif text == "事":
+                    special_dict["請假"].append(f"{date} {slot}")
+
+        json_output = json.dumps(special_dict, ensure_ascii=False, separators=(',', ':'))
+
+        return json_output
+
+
+    except Exception as e:
+        error_message = str(e) 
+        return {'code': 33, 'reason': f'something Wrong, step {stepSave}try的錯誤原應: {error_message}'}
+    
+
+
+
```

### Comparing `shinherpro-1.6.7/shinherpro/chormeDriver.py` & `shinherpro-1.6.8/shinherpro/chormeDriver.py`

 * *Files identical despite different names*

### Comparing `shinherpro-1.6.7/shinherpro/serverLog.py` & `shinherpro-1.6.8/shinherpro/serverLog.py`

 * *Files identical despite different names*

### Comparing `shinherpro-1.6.7/shinherpro/vfcModel.py` & `shinherpro-1.6.8/shinherpro/vfcModel.py`

 * *Files identical despite different names*

