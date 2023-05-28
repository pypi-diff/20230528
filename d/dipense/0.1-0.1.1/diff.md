# Comparing `tmp/dipense-0.1.tar.gz` & `tmp/dipense-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dipense-0.1.tar", last modified: Sun Nov 13 11:13:11 2022, max compression
+gzip compressed data, was "dipense-0.1.1.tar", last modified: Sun May 28 20:35:38 2023, max compression
```

## Comparing `dipense-0.1.tar` & `dipense-0.1.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 usman     (1000) usman     (1000)        0 2022-11-13 11:13:11.869059 dipense-0.1/
--rw-rw-r--   0 usman     (1000) usman     (1000)       81 2022-11-13 11:06:46.000000 dipense-0.1/CHANGELOG
--rw-rw-r--   0 usman     (1000) usman     (1000)     1077 2022-11-13 11:06:57.000000 dipense-0.1/LICENSE
--rw-rw-r--   0 usman     (1000) usman     (1000)       54 2022-11-13 11:07:07.000000 dipense-0.1/MANIFEST.in
--rw-rw-r--   0 usman     (1000) usman     (1000)     2682 2022-11-13 11:13:11.869059 dipense-0.1/PKG-INFO
--rw-rw-r--   0 usman     (1000) usman     (1000)     1990 2022-11-13 11:07:18.000000 dipense-0.1/README.md
-drwxrwxr-x   0 usman     (1000) usman     (1000)        0 2022-11-13 11:13:11.829057 dipense-0.1/dipense/
--rw-rw-r--   0 usman     (1000) usman     (1000)     2277 2022-11-13 11:04:26.000000 dipense-0.1/dipense/__init__.py
--rw-rw-r--   0 usman     (1000) usman     (1000)     1357 2022-11-13 11:04:26.000000 dipense-0.1/dipense/default.py
--rw-rw-r--   0 usman     (1000) usman     (1000)     9408 2022-11-13 11:04:26.000000 dipense-0.1/dipense/drone.py
--rw-rw-r--   0 usman     (1000) usman     (1000)     4610 2022-11-13 11:05:07.000000 dipense-0.1/dipense/icheckp.py
--rw-rw-r--   0 usman     (1000) usman     (1000)     1763 2022-11-13 11:05:07.000000 dipense-0.1/dipense/structure.py
-drwxrwxr-x   0 usman     (1000) usman     (1000)        0 2022-11-13 11:13:11.865059 dipense-0.1/dipense.egg-info/
--rw-rw-r--   0 usman     (1000) usman     (1000)     2682 2022-11-13 11:13:09.000000 dipense-0.1/dipense.egg-info/PKG-INFO
--rw-rw-r--   0 usman     (1000) usman     (1000)      298 2022-11-13 11:13:10.000000 dipense-0.1/dipense.egg-info/SOURCES.txt
--rw-rw-r--   0 usman     (1000) usman     (1000)        1 2022-11-13 11:13:09.000000 dipense-0.1/dipense.egg-info/dependency_links.txt
--rw-rw-r--   0 usman     (1000) usman     (1000)       90 2022-11-13 11:13:09.000000 dipense-0.1/dipense.egg-info/requires.txt
--rw-rw-r--   0 usman     (1000) usman     (1000)        8 2022-11-13 11:13:09.000000 dipense-0.1/dipense.egg-info/top_level.txt
--rw-rw-r--   0 usman     (1000) usman     (1000)       38 2022-11-13 11:13:11.869059 dipense-0.1/setup.cfg
--rw-rw-r--   0 usman     (1000) usman     (1000)     1581 2022-11-13 11:09:06.000000 dipense-0.1/setup.py
+drwxrwxr-x   0 usman     (1000) usman     (1000)        0 2023-05-28 20:35:38.296496 dipense-0.1.1/
+-rw-rw-r--   0 usman     (1000) usman     (1000)      138 2023-05-28 20:01:27.000000 dipense-0.1.1/CHANGELOG
+-rw-rw-r--   0 usman     (1000) usman     (1000)     1077 2023-05-28 19:56:33.000000 dipense-0.1.1/LICENSE
+-rw-rw-r--   0 usman     (1000) usman     (1000)       64 2023-05-28 20:31:21.000000 dipense-0.1.1/MANIFEST.in
+-rw-rw-r--   0 usman     (1000) usman     (1000)     3657 2023-05-28 20:35:38.292496 dipense-0.1.1/PKG-INFO
+-rw-rw-r--   0 usman     (1000) usman     (1000)     2043 2023-05-28 19:59:14.000000 dipense-0.1.1/README.md
+drwxrwxr-x   0 usman     (1000) usman     (1000)        0 2023-05-28 20:35:38.280495 dipense-0.1.1/dipense/
+-rw-rw-r--   0 usman     (1000) usman     (1000)     2637 2023-05-28 20:01:37.000000 dipense-0.1.1/dipense/__init__.py
+-rw-rw-r--   0 usman     (1000) usman     (1000)     1379 2023-05-28 19:56:33.000000 dipense-0.1.1/dipense/default.py
+-rw-rw-r--   0 usman     (1000) usman     (1000)     9288 2023-05-28 19:56:33.000000 dipense-0.1.1/dipense/drone.py
+-rw-rw-r--   0 usman     (1000) usman     (1000)     4601 2023-05-28 19:56:33.000000 dipense-0.1.1/dipense/icheckp.py
+-rw-rw-r--   0 usman     (1000) usman     (1000)     1770 2023-05-28 19:56:33.000000 dipense-0.1.1/dipense/structure.py
+drwxrwxr-x   0 usman     (1000) usman     (1000)        0 2023-05-28 20:35:38.292496 dipense-0.1.1/dipense.egg-info/
+-rw-rw-r--   0 usman     (1000) usman     (1000)     3657 2023-05-28 20:35:37.000000 dipense-0.1.1/dipense.egg-info/PKG-INFO
+-rw-rw-r--   0 usman     (1000) usman     (1000)      298 2023-05-28 20:35:38.000000 dipense-0.1.1/dipense.egg-info/SOURCES.txt
+-rw-rw-r--   0 usman     (1000) usman     (1000)        1 2023-05-28 20:35:37.000000 dipense-0.1.1/dipense.egg-info/dependency_links.txt
+-rw-rw-r--   0 usman     (1000) usman     (1000)       90 2023-05-28 20:35:37.000000 dipense-0.1.1/dipense.egg-info/requires.txt
+-rw-rw-r--   0 usman     (1000) usman     (1000)        8 2023-05-28 20:35:37.000000 dipense-0.1.1/dipense.egg-info/top_level.txt
+-rw-rw-r--   0 usman     (1000) usman     (1000)       38 2023-05-28 20:35:38.296496 dipense-0.1.1/setup.cfg
+-rw-rw-r--   0 usman     (1000) usman     (1000)     1706 2023-05-28 20:33:28.000000 dipense-0.1.1/setup.py
```

### Comparing `dipense-0.1/LICENSE` & `dipense-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dipense-0.1/dipense/__init__.py` & `dipense-0.1.1/dipense/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-
-
+# -*- coding: utf-8 -*-
 """
   An OSINT tool for it ninjas
   
   _____________
   ICHECKP usage:
   from dipense.icheckp import ICHECKP
   --- OR ---
@@ -16,33 +15,41 @@
   into the ICHECKP class, this will automatically open a map in
   your webbrowser, e.g
     _______________________________________________
     ICHECKP(autoOpenMap=True).icheckp('197.3.11.7')
     
 """
 
+__title__ = "dipense"
+__version__ = "0.1.1"
+__author__ = "Usman Musa"
+__author_email__ = "usmanmusa1920@gmail.com"
+__author_website__ = "https://usmanmusa1920.github.io"
+__repository__ = "https://github.com/usmanmusa1920/dipense-lib"
+__website__ = "https://dipense-lib.readthedocs.io"
+__copyright__ = "Copyright (C) 2022 - 2023 Usman Musa"
+
 import argparse
 from .icheckp import ICHECKP
 from .default import default
 from .default import Default
 
 
 # def icheckp(ip, autoOpenMap=False):
-#   print('The year is', default()['the_year'])
+#   print("The year is", default()["the_year"])
 
 getout = print
 def ipLoad():
   # prog is the name of the program, default=sys.argv[0]
-  parser = argparse.ArgumentParser(prog='scan an ip address', description='This scan an ip address!')
+  parser = argparse.ArgumentParser(prog="scan an ip address", description="This scan an ip address!")
   
   # metavar make the -help to look cleaan
-  parser.add_argument('--ip', '-i', required=True, type=str, metavar='', help='What is the ip address?')
-  parser.add_argument('--open', '-o', default=False, required=False, type=str, metavar='', help='This will automatic open your map in web browser, it is a boolean of `True or False`')
-  parser.add_argument(dest="payloadip", default="payloadip", type=str, metavar='', help='The payload is to find an ip address infomation')
-  
+  parser.add_argument("--ip", "-i", required=True, type=str, metavar="", help="What is the ip address?")
+  parser.add_argument("--open", "-o", default=False, required=False, type=str, metavar="", help="This will automatic open your map in web browser, it is a boolean of `True or False`")
+  parser.add_argument(dest="payloadip", default="payloadip", type=str, metavar="", help="The payload is to find an ip address infomation")
   
   args = parser.parse_args()
   ICHECKP(autoOpenMap=args.open).icheckp(args.ip)
   
   
 def payloads(helper):
   import sys
```

### Comparing `dipense-0.1/dipense/default.py` & `dipense-0.1.1/dipense/default.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# -*- coding: utf-8 -*-
 from datetime import datetime
 
 
 class Default:
   
   @staticmethod
   def default():
@@ -18,31 +19,31 @@
       
       Also for the notification of new recent comment, reply, search, or message
       that will show on the menu bar button (in the header)
     """
     
     the_year = datetime.utcnow().year
     data = {
-      'the_year': the_year,
+      "the_year": the_year,
     }
     
     return data
-  
-  payload = 'payload'
-  suffix_payload = ['num', 'who', 'ip']
+
+  payload = "payload"
+  suffix_payload = ["num", "who", "ip"]
   sites_list = [
-    'site:facebook.com',
-    'site:twitter.com',
-    'site:instagram.com',
-    'site:tiktok.com',
-    'site:youtube.com',
-    'site:linkedin.com',
-    'site:github.com',
+    "site:facebook.com",
+    "site:twitter.com",
+    "site:instagram.com",
+    "site:tiktok.com",
+    "site:youtube.com",
+    "site:linkedin.com",
+    "site:github.com",
   ]
   
   
 def default():
   """
-    this is the function (shortcut of `Default.default') that we will call in some of our site view
-    instead of calling the `Default.default' which will make our code so large
+    this is the function (shortcut of `Default.default") that we will call in some of our site view
+    instead of calling the `Default.default" which will make our code so large
   """
   return Default.default()
```

### Comparing `dipense-0.1/dipense/drone.py` & `dipense-0.1.1/dipense/drone.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,91 +1,85 @@
-
-import os
-import sys
-import shlex
+# -*- coding: utf-8 -*-
 import argparse
-import subprocess as sp
 
 from .default import Default
 from . import getout
 
 import whois
 import phonenumbers
 from termcolor import colored
 from phonenumbers import carrier
 from phonenumbers import geocoder
 from phonenumbers import timezone
 
 
-
 def numLoad():
   # prog is the name of the program, default=sys.argv[0]
-  parser = argparse.ArgumentParser(prog='scan phone number', description='This scan a phone number!')
+  parser = argparse.ArgumentParser(prog="scan phone number", description="This scan a phone number!")
   
   # metavar make the -help to look cleaan
-  parser.add_argument('--number', '-n', required=True, type=str, metavar='', help='What is the phone number? it should start with country code e.g +2348123456789')
-  parser.add_argument(dest="payloadnum", default="payloadnum", type=str, metavar='', help='The payload is to find phone number infomation')
-  
+  parser.add_argument("--number", "-n", required=True, type=str, metavar="", help="What is the phone number? it should start with country code e.g +2348123456789")
+  parser.add_argument(dest="payloadnum", default="payloadnum", type=str, metavar="", help="The payload is to find phone number infomation")
   
   args = parser.parse_args()
   p_num = args.number
-    
+
   try:
     num_parse = phonenumbers.parse(p_num, None)
     num_valid = phonenumbers.is_valid_number(num_parse)
     p_nation = phonenumbers.format_number(num_parse, phonenumbers.PhoneNumberFormat.NATIONAL)
     inter_nation = phonenumbers.format_number(num_parse, phonenumbers.PhoneNumberFormat.INTERNATIONAL)
     p_e164 = phonenumbers.format_number(num_parse, phonenumbers.PhoneNumberFormat.E164)
-    p_geo = geocoder.description_for_number(num_parse, 'en')
-    p_carr = carrier.name_for_number(num_parse, 'en')
+    p_geo = geocoder.description_for_number(num_parse, "en")
+    p_carr = carrier.name_for_number(num_parse, "en")
     time_zone_1 = timezone.time_zones_for_number(num_parse)
     time_zone_2 = timezone.time_zones_for_geographical_number(num_parse)
     
     """
-        >>> p_num = '+2349083513047'
-        >>> num_parse = phonenumbers.parse(p_num, None)
-        >>> num_parse
-        PhoneNumber(country_code=234, national_number=9083513047, extension=None, italian_leading_zero=None, number_of_leading_zeros=None, country_code_source=0, preferred_domestic_carrier_code=None)
-        >>> num_valid = phonenumbers.is_valid_number(num_parse)
-        >>> num_valid
-        True
-        >>> p_nation = phonenumbers.format_number(num_parse, phonenumbers.PhoneNumberFormat.NATIONAL)
-        >>> p_nation
-        '0908 351 3047'
-        >>> inter_nation = phonenumbers.format_number(num_parse, phonenumbers.PhoneNumberFormat.INTERNATIONAL)
-        >>> inter_nation
-        '+234 908 351 3047'
-        >>> p_e164 = phonenumbers.format_number(num_parse, phonenumbers.PhoneNumberFormat.E164)
-        >>> p_e164
-        '+2349083513047'
-        >>> p_geo = geocoder.description_for_number(num_parse, 'en')
-        >>> p_geo
-        'Nigeria'
-        >>> p_carr = carrier.name_for_number(num_parse, 'en')
-        >>> p_carr
-        '9mobile'
-        >>> time_zone_1 = timezone.time_zones_for_number(num_parse)
-        >>> time_zone_1
-        ('Africa/Lagos',)
-        >>> time_zone_2 = timezone.time_zones_for_geographical_number(num_parse)
-        >>> time_zone_2
-        ('Africa/Lagos',)
+      >>> p_num = '+2349083513047'
+      >>> num_parse = phonenumbers.parse(p_num, None)
+      >>> num_parse
+      PhoneNumber(country_code=234, national_number=9083513047, extension=None, italian_leading_zero=None, number_of_leading_zeros=None, country_code_source=0, preferred_domestic_carrier_code=None)
+      >>> num_valid = phonenumbers.is_valid_number(num_parse)
+      >>> num_valid
+      True
+      >>> p_nation = phonenumbers.format_number(num_parse, phonenumbers.PhoneNumberFormat.NATIONAL)
+      >>> p_nation
+      '0908 351 3047'
+      >>> inter_nation = phonenumbers.format_number(num_parse, phonenumbers.PhoneNumberFormat.INTERNATIONAL)
+      >>> inter_nation
+      '+234 908 351 3047'
+      >>> p_e164 = phonenumbers.format_number(num_parse, phonenumbers.PhoneNumberFormat.E164)
+      >>> p_e164
+      '+2349083513047'
+      >>> p_geo = geocoder.description_for_number(num_parse, 'en')
+      >>> p_geo
+      'Nigeria'
+      >>> p_carr = carrier.name_for_number(num_parse, 'en')
+      >>> p_carr
+      '9mobile'
+      >>> time_zone_1 = timezone.time_zones_for_number(num_parse)
+      >>> time_zone_1
+      ('Africa/Lagos',)
+      >>> time_zone_2 = timezone.time_zones_for_geographical_number(num_parse)
+      >>> time_zone_2
+      ('Africa/Lagos',)
     """
-    
+
     context = {
-      'num_parse': num_parse,
-      'num_valid': num_valid,
-      'p_nation': p_nation,
-      'inter_nation': inter_nation,
-      'p_e164': p_e164,
-      'p_geo': p_geo,
-      'p_carr': p_carr,
-      'time_zone_1': time_zone_1,
-      'time_zone_2': time_zone_2,
-      'sites_list': Default.sites_list,
+      "num_parse": num_parse,
+      "num_valid": num_valid,
+      "p_nation": p_nation,
+      "inter_nation": inter_nation,
+      "p_e164": p_e164,
+      "p_geo": p_geo,
+      "p_carr": p_carr,
+      "time_zone_1": time_zone_1,
+      "time_zone_2": time_zone_2,
+      "sites_list": Default.sites_list,
     }
     
     getout(colored(r"""
            _..._
          .'     '.
         /  _   _  \
         | (o)_(o) |
@@ -94,55 +88,54 @@
         //   .   \ \
        ||   .     \ \
        |\   :     / |
        \ `) '   (`  /_
      _)``".____,.'"` (_
      )     )'--'(     (
       '---`      `---`
-""", 'cyan', attrs=['blink']))
+""", "cyan", attrs=["blink"]))
     
-    # q1 = f'{site} intext: "{p_e164}" OR intex: "{inter_nation}" OR intex: "{p_nation}"'
-    # q2 = q1.replace(' ', '+')
+    # q1 = f"{site} intext: "{p_e164}" OR intex: "{inter_nation}" OR intex: "{p_nation}""
+    # q2 = q1.replace(" ", "+")
     # for site in context["sites_list"]:
-    #   # q1 = f'{site} intext: "{p_e164}" OR intex: "{inter_nation}" OR intex: "{p_nation}"'
-    #   # q2 = q1.replace(' ', '+')
-    #   url_g = '[+] ' + f'https://www.google.com/search?q={site}+intext%3A{p_e164}"+OR+intext"{inter_nation}"+OR +ntext:"{p_nation}"'
+    #   # q1 = f"{site} intext: "{p_e164}" OR intex: "{inter_nation}" OR intex: "{p_nation}""
+    #   # q2 = q1.replace(" ", "+")
+    #   url_g = "[+] " + f'https://www.google.com/search?q={site}+intext%3A{p_e164}"+OR+intext"{inter_nation}"+OR +ntext:"{p_nation}"'
     #   getout(colored(url_g, "magenta"))
-      
+    
   except:
     context = {
-      'p_num': p_num,
+      "p_num": p_num,
     }
     
   for k, v in context.items():
-    if k == 'sites_list':
+    if k == "sites_list":
       pass
     else:
-      r = k + ': '
+      r = k + ": "
       getout(colored(" =>", "magenta"), colored(r, "green"), v)
-  # if args.kind == 'nmap':
-  #   n_cmd = 'nmap -v -A -sV ' + args.ip
+  # if args.kind == "nmap":
+  #   n_cmd = "nmap -v -A -sV " + args.ip
   #   n = sp.run(shlex.split(n_cmd))
-  #   getout('This', n.args)
+  #   getout("This", n.args)
   #   return [args, n]
   return args
-
+  
 
 def whoLoad():
   # prog is the name of the program, default=sys.argv[0]
-  parser = argparse.ArgumentParser(prog='who is', description='This scan and find info of a domain!')
+  parser = argparse.ArgumentParser(prog="who is", description="This scan and find info of a domain!")
   
   # metavar make the -help to look cleaan
-  parser.add_argument('--domain', '-d', required=True, type=str, metavar='', help='What is the domain name? probably it gives infoof most TLD, while others like ().tk, .io, .org) it capture less')
-  parser.add_argument(dest="payloadwho", default="payloadwho", type=str, metavar='', help='The payload is to find domain name infomation')
-  
+  parser.add_argument("--domain", "-d", required=True, type=str, metavar="", help="What is the domain name? probably it gives infoof most TLD, while others like ().tk, .io, .org) it capture less")
+  parser.add_argument(dest="payloadwho", default="payloadwho", type=str, metavar="", help="The payload is to find domain name infomation")
   
   args = parser.parse_args()
   domain = args.domain
-    
+
   try:
     howis = whois.whois(domain)
     """
       >>> import whois
       >>> howis = whois.whois('google.com')
       >>> howis
       {'domain_name': ['GOOGLE.COM', 'google.com'], 'registrar': 'MarkMonitor, Inc.', 'whois_server': 'whois.markmonitor.com', 'referral_url': None, 'updated_date': [datetime.datetime(2019, 9, 9, 15, 39, 4), datetime.datetime(2019, 9, 9, 15, 39, 4, tzinfo=datetime.timezone.utc)], 'creation_date': [datetime.datetime(1997, 9, 15, 4, 0), datetime.datetime(1997, 9, 15, 7, 0, tzinfo=datetime.timezone.utc)], 'expiration_date': [datetime.datetime(2028, 9, 14, 4, 0), datetime.datetime(2028, 9, 13, 7, 0, tzinfo=datetime.timezone.utc)], 'name_servers': ['NS1.GOOGLE.COM', 'NS2.GOOGLE.COM', 'NS3.GOOGLE.COM', 'NS4.GOOGLE.COM', 'ns3.google.com', 'ns1.google.com', 'ns4.google.com', 'ns2.google.com'], 'status': ['clientDeleteProhibited https://icann.org/epp#clientDeleteProhibited', 'clientTransferProhibited https://icann.org/epp#clientTransferProhibited', 'clientUpdateProhibited https://icann.org/epp#clientUpdateProhibited', 'serverDeleteProhibited https://icann.org/epp#serverDeleteProhibited', 'serverTransferProhibited https://icann.org/epp#serverTransferProhibited', 'serverUpdateProhibited https://icann.org/epp#serverUpdateProhibited', 'clientUpdateProhibited (https://www.icann.org/epp#clientUpdateProhibited)', 'clientTransferProhibited (https://www.icann.org/epp#clientTransferProhibited)', 'clientDeleteProhibited (https://www.icann.org/epp#clientDeleteProhibited)', 'serverUpdateProhibited (https://www.icann.org/epp#serverUpdateProhibited)', 'serverTransferProhibited (https://www.icann.org/epp#serverTransferProhibited)', 'serverDeleteProhibited (https://www.icann.org/epp#serverDeleteProhibited)'], 'emails': ['abusecomplaints@markmonitor.com', 'whoisrequest@markmonitor.com'], 'dnssec': 'unsigned', 'name': None, 'org': 'Google LLC', 'address': None, 'city': None, 'state': 'CA', 'registrant_postal_code': None, 'country': 'US'}
@@ -164,59 +157,57 @@
     address = howis.address
     city = howis.city
     state = howis.state
     registrant_postal_code = howis.registrant_postal_code
     country = howis.countr
     
     context = {
-      'howis': howis,
-      'domain': domain,
-      'domain_name': domain_name,
-      'registrar': registrar,
-      'whois_server': whois_server,
-      'referral_url': referral_url,
-      'updated_date': updated_date,
-      'creation_date': creation_date,
-      'expiration_date': expiration_date,
-      'name_servers': name_servers,
-      'status': status,
-      'emails': emails,
-      'dnssec': dnssec,
-      'name': name,
-      'org': org,
-      'address': address,
-      'city': city,
-      'state': state,
-      'registrant_postal_code': registrant_postal_code,
-      'country': country,
+      "howis": howis,
+      "domain": domain,
+      "domain_name": domain_name,
+      "registrar": registrar,
+      "whois_server": whois_server,
+      "referral_url": referral_url,
+      "updated_date": updated_date,
+      "creation_date": creation_date,
+      "expiration_date": expiration_date,
+      "name_servers": name_servers,
+      "status": status,
+      "emails": emails,
+      "dnssec": dnssec,
+      "name": name,
+      "org": org,
+      "address": address,
+      "city": city,
+      "state": state,
+      "registrant_postal_code": registrant_postal_code,
+      "country": country,
     }
   except:
     context = {
-      'domain': domain,
+      "domain": domain,
     }
     
-  
   if domain_name == None:
-    getout(colored(' => ', "cyan"), colored('domain:', "green"), domain)
-    getout(colored(' => ', "cyan", attrs=['blink']), colored('status:', "green"), colored('unauthorized', "red", attrs=['blink']))
+    getout(colored(" => ", "cyan"), colored("domain:", "green"), domain)
+    getout(colored(" => ", "cyan", attrs=["blink"]), colored("status:", "green"), colored("unauthorized", "red", attrs=["blink"]))
   else:
     for k, v in context.items():
-      
       # if the value of the result is None the color should be red
       if v == None:
-        r = k + ':'
-        getout(colored(' => ', "cyan"), colored(r, "green"), colored(v, "red", attrs=['blink']))
+        r = k + ":"
+        getout(colored(" => ", "cyan"), colored(r, "green"), colored(v, "red", attrs=["blink"]))
       else:
         # if the key is status, it will print different and do for loof over the result list
-        if k == 'status':
-          getout('\n', colored('=> ', "cyan"), colored('status', "yellow"), ':')
+        if k == "status":
+          getout("\n", colored("=> ", "cyan"), colored("status", "yellow"), ":")
           for s in v:
-            getout('\t\t', colored(' --- ', "green"), colored(s, 'yellow'))
+            getout("\t\t", colored(" --- ", "green"), colored(s, "yellow"))
           getout()
         # else if the key is howis, it will look different
-        elif k == 'howis':
-          r = k + ':'
-          getout(colored(' => ', "cyan"), colored(r, "blue"), colored(v, 'blue', attrs=['blink']))
+        elif k == "howis":
+          r = k + ":"
+          getout(colored(" => ", "cyan"), colored(r, "blue"), colored(v, "blue", attrs=["blink"]))
         else:
-          r = k + ':'
-          getout(colored(' => ', "cyan"), colored(r, "green"), v)
+          r = k + ":"
+          getout(colored(" => ", "cyan"), colored(r, "green"), v)
   return args
```

### Comparing `dipense-0.1/dipense/icheckp.py` & `dipense-0.1.1/dipense/icheckp.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,14 @@
-
-
+# -*- coding: utf-8 -*-
 import os
 import csv
 import subprocess as sp
 from termcolor import cprint
 from termcolor import colored
 
-
 from .structure import Filing
 from .structure import tracer
 from .structure import geoip
 
 
 class ICHECKP(Filing):
   """this class handle ip address payloads"""
@@ -20,16 +18,16 @@
       g = geoip.ip(i_num)
       cty = g.city # ip address city
       stt = g.state # ip address state
       ctry = g.country # ip address country
       
       json_raw = g.raw
       time_zone = list(list(json_raw.items())[6])[1] # ip address timezone area
-      d_longitude = list(list(json_raw.items())[4])[1].split(',')[1] # ip address longitude
-      d_latitude = list(list(json_raw.items())[4])[1].split(',')[0] # ip address latitude
+      d_longitude = list(list(json_raw.items())[4])[1].split(",")[1] # ip address longitude
+      d_latitude = list(list(json_raw.items())[4])[1].split(",")[0] # ip address latitude
       d_location = list(list(json_raw.items())[4])[1] # ip address coordinate
       
       location = g.latlng # a list which include latitude and longitude
       
       # creating a base map, making the `min_zoom=0`,
       # overide the `zoom_start=13` from default which is `10` to `13`, and
       # overide the `max_zoom=70` from default which is `18` to `70`
@@ -39,93 +37,89 @@
       tracer.CircleMarker(location=location, radius=50, color="#3186cc", fill=True, fill_color="#3186cc").add_to(Tmap)
       tracer.Circle(radius=100, location=location, popup="The Waterfront", color="crimson", fill=False).add_to(Tmap)
       # making the icon to be `cloud`
       tracer.Marker(location, icon=tracer.Icon(icon="cloud")).add_to(Tmap)
       
       self.dir_tree() # make the dir tree
       sp.run("cd .dipense/maps && sudo touch map.html", shell=True)
-      
       cwd = os.getcwd()
 
       os.chdir(os.path.join(cwd, ".dipense/maps"))
-      os.system('sudo touch test.py')
+      os.system("sudo touch test.py")
       
       map_file_method = self.mapName(i_num)
       mapF = map_file_method[0]
       csv_from_mapF = map_file_method[1]
       
-      html_map_file_cmd = 'sudo touch {}'.format(mapF)
-      csv_map_file_cmd = 'sudo touch {}'.format(csv_from_mapF)
+      html_map_file_cmd = "sudo touch {}".format(mapF)
+      csv_map_file_cmd = "sudo touch {}".format(csv_from_mapF)
       
       os.system(html_map_file_cmd)
       os.system(csv_map_file_cmd)
       
       for i in os.listdir():
-        sp.run(['sudo', 'chmod', '777', i])
-      
+        sp.run(["sudo", "chmod", "777", i])
+
       Tmap.save(mapF)
       cprint(os.getcwd(), "magenta")
       
       dummy = """# this is a test module
 
   # write with focus
   """
 
-      with open('test.py', 'w') as f:
+      with open("test.py", "w") as f:
         f.write(dummy)
-        
-      fieldnames = ['City', 'State', 'Country', 'time_zone', 'd_longitude', 'd_latitude', 'd_location', 'location', 'Map']
+      fieldnames = ["City", "State", "Country", "time_zone", "d_longitude", "d_latitude", "d_location", "location", "Map"]
       
-      with open(csv_from_mapF, 'w') as csv_f:
+      with open(csv_from_mapF, "w") as csv_f:
         csv_writer = csv.writer(csv_f)
         csv_writer.writerow(fieldnames)
         csv_writer.writerow([cty, stt, ctry, time_zone, d_longitude, d_latitude, d_location, location, mapF])
         
       csv_loc = "csv file is located in " + os.path.realpath(csv_from_mapF)
       cprint(csv_loc, "green")
       # cprint(csv_loc, "green", attrs=["bold"])
       
       if self.autoOpenMap:
         import webbrowser
         webbrowser.get().open(os.path.realpath(mapF))
-        openInfo = 'Soon to open ' + os.path.realpath(mapF)
+        openInfo = "Soon to open " + os.path.realpath(mapF)
         print(colored(openInfo, "magenta", attrs=["reverse", "blink"]))
-      
+        
       context = {
-        'cty': cty,
-        'stt': stt,
-        'ctry': ctry,
-        'json_raw': json_raw,
-        'time_zone': time_zone,
-        'd_longitude': d_longitude,
-        'd_latitude': d_latitude,
-        'd_location': d_location,
-        'location coordinate': location,
+        "cty": cty,
+        "stt": stt,
+        "ctry": ctry,
+        "json_raw": json_raw,
+        "time_zone": time_zone,
+        "d_longitude": d_longitude,
+        "d_latitude": d_latitude,
+        "d_location": d_location,
+        "location coordinate": location,
       }
       
     except:
       context = {
-        'i_num': i_num,
+        "i_num": i_num,
       }
       
     from . import getout
     if g.raw == None:
-      getout(colored(' => ', "cyan"), colored('domain:', "green"), i_num)
-      getout(colored(' => ', "cyan", attrs=['blink']), colored('status:', "green"), colored('unauthorized', "red", attrs=['blink']))
+      getout(colored(" => ", "cyan"), colored("domain:", "green"), i_num)
+      getout(colored(" => ", "cyan", attrs=["blink"]), colored("status:", "green"), colored("unauthorized", "red", attrs=["blink"]))
     else:
       for k, v in context.items():
-        
         # if the value of the result is None the color should be red
         if v == None:
-          r = k + ':'
-          getout(colored(' => ', "cyan"), colored(r, "green"), colored(v, "red", attrs=['blink']))
+          r = k + ":"
+          getout(colored(" => ", "cyan"), colored(r, "green"), colored(v, "red", attrs=["blink"]))
         else:
           # if the key is json_raw, it will print different and do for loof over the result list
-          if k == 'json_raw':
-            getout('\n', colored('=> ', "cyan"), colored('json_raw', "yellow"), ':')
+          if k == "json_raw":
+            getout("\n", colored("=> ", "cyan"), colored("json_raw", "yellow"), ":")
             for s in v.items():
-              getout('\t\t', colored(' --- ', "green"), colored(s, 'yellow'))
+              getout("\t\t", colored(" --- ", "green"), colored(s, "yellow"))
             getout()
           else:
-            r = k + ':'
-            getout(colored(' => ', "cyan"), colored(r, "green"), v)
-
+            r = k + ":"
+            getout(colored(" => ", "cyan"), colored(r, "green"), v)
```

### Comparing `dipense-0.1/setup.py` & `dipense-0.1.1/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,52 +1,48 @@
+# -*- coding: utf-8 -*-
 from setuptools import setup
 from setuptools import find_packages
 
 
-
 setup(
-  
-  # name of the main package (dipense)
-  name='dipense',
-  version='0.1',
-  
-  description='An OSINT tool for IT ninjas',
-  long_description=open('README.md').read() + '\n\n' + open('CHANGELOG').read(),
+  name = "dipense", # name of the main package (base folder i.e dipense)
+  version = "0.1.1",
+  description = "An OSINT tool for IT ninjas",
+  long_description = open("README.md").read() + "\n\n" + open("CHANGELOG").read(),
   long_description_content_type="text/markdown",
+  python_requires = ">=3.6",
+  # platforms="any",
   
-  # The URL of your package's (project) home page e.g. github link
-  url='https://github.com/usmanmusa1920/dipense-lib',
-  
-  # Author details
-  author='Usman Musa',
-  author_email='usmanmusa1920@gmail.com',
-  
-  # Choose your license, note the American spelling
-  License='MIT',
-  
+  url = "https://dipense.readthedocs.io",
+  repo = "https://github.com/usmanmusa1920/dipense",
+  author = "Usman Musa",
+  author_email = "usmanmusa1920@gmail.com",
+  license = "MIT", # Choose your license, note the American spelling
   classifiers = [
-    'Development Status :: 5 - Production/Stable',
-    'Intended Audience :: Developers',
-    'Natural Language :: English',
-    'Operating System :: POSIX :: Linux',
-    'License :: OSI Approved :: MIT License',
-    'Programming Language :: Python',
-    'Programming Language :: Python :: 3'
+    "Development Status :: 5 - Production/Stable",
+    "Intended Audience :: Developers",
+    "Natural Language :: English",
+    "Operating System :: POSIX :: Linux",
+    "License :: OSI Approved :: MIT License",
+    "Programming Language :: Python",
+    "Programming Language :: Python :: 3"
   ],
   
   # used when people are searching for a module, keywords separated with a space
-  keywords='dipense',
+  keywords = "dipense",
+  include_package_data = True, # include files listed in MANIFEST.in
   
   # The list of packages(directories) for your library
-  packages=find_packages(), # OR packages=['dipense'] 
-  
-  # py_modules=[''] # list of files (modules) that are not in any directory (at the root dir)
+  packages=find_packages(), # OR packages=["dipense"] 
+  # If your package is a single module, use this instead of "packages":
+  # py_modules=[""] # list of files (modules) that are not in any directory (at the root dir)
   # the libraries it depends on
   
-  include_package_data = True, # include files listed in MANIFEST.in
-  
   # List of other python modules which this module depends on.  For example RPi.GPIO
-  install_requires=[
-    'folium==0.13.0', 'phonenumbers==8.13.0', 'geocoder==1.38.1',
-    'python-whois==0.8.0', 'termcolor==2.1.0'
+  install_requires = [
+    "folium==0.13.0",
+    "phonenumbers==8.13.0",
+    "geocoder==1.38.1",
+    "python-whois==0.8.0",
+    "termcolor==2.1.0",
     ]
-)
+)
```

