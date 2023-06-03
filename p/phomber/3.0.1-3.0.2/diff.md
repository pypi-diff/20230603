# Comparing `tmp/phomber-3.0.1-py3.9.egg` & `tmp/phomber-3.0.2-py3.9.egg`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 43755 bytes, number of entries: 13
--rw-r--r--  2.0 unx     3512 b- defN 23-May-22 12:46 EGG-INFO/PKG-INFO
--rw-r--r--  2.0 unx      271 b- defN 23-May-22 12:46 EGG-INFO/SOURCES.txt
--rw-r--r--  2.0 unx        1 b- defN 23-May-22 12:46 EGG-INFO/dependency_links.txt
--rw-r--r--  2.0 unx       57 b- defN 23-May-22 12:46 EGG-INFO/entry_points.txt
--rw-r--r--  2.0 unx       35 b- defN 23-May-22 12:46 EGG-INFO/requires.txt
--rw-r--r--  2.0 unx       23 b- defN 23-May-22 12:46 EGG-INFO/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 23-May-22 12:46 EGG-INFO/zip-safe
+Zip file size: 52128 bytes, number of entries: 13
+-rw-r--r--  2.0 unx     3512 b- defN 23-Jun-03 14:23 EGG-INFO/PKG-INFO
+-rw-r--r--  2.0 unx      275 b- defN 23-Jun-03 14:23 EGG-INFO/SOURCES.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-Jun-03 14:23 EGG-INFO/dependency_links.txt
+-rw-r--r--  2.0 unx       50 b- defN 23-Jun-03 14:23 EGG-INFO/entry_points.txt
+-rw-r--r--  2.0 unx       76 b- defN 23-Jun-03 14:23 EGG-INFO/requires.txt
+-rw-r--r--  2.0 unx        8 b- defN 23-Jun-03 14:23 EGG-INFO/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-Jun-03 14:23 EGG-INFO/zip-safe
 -rw-r--r--  2.0 unx        0 b- defN 23-May-21 17:02 phomber/__init__.py
--rw-r--r--  2.0 unx    55263 b- defN 23-May-21 18:33 phomber/phomber.py
--rw-r--r--  2.0 unx    55263 b- defN 23-May-21 18:07 phomber/phomberv3_beta.py
--rw-r--r--  2.0 unx      139 b- defN 23-May-22 12:46 phomber/__pycache__/__init__.cpython-39.pyc
--rw-r--r--  2.0 unx    33451 b- defN 23-May-22 12:46 phomber/__pycache__/phomber.cpython-39.pyc
--rw-r--r--  2.0 unx    33458 b- defN 23-May-22 12:46 phomber/__pycache__/phomberv3_beta.cpython-39.pyc
-13 files, 181474 bytes uncompressed, 42051 bytes compressed:  76.8%
+-rw-r--r--  2.0 unx    68961 b- defN 23-Jun-03 14:22 phomber/phomber.py
+-rw-r--r--  2.0 unx    68961 b- defN 23-Jun-03 14:22 phomber/phomberv3.0.2_beta.py
+-rw-r--r--  2.0 unx      139 b- defN 23-Jun-03 14:23 phomber/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--  2.0 unx    40376 b- defN 23-Jun-03 14:23 phomber/__pycache__/phomber.cpython-39.pyc
+-rw-r--r--  2.0 unx    40387 b- defN 23-Jun-03 14:23 phomber/__pycache__/phomberv3.0.2_beta.cpython-39.pyc
+13 files, 222747 bytes uncompressed, 50408 bytes compressed:  77.4%
```

## zipnote «TEMP»/diffoscope_aguvzjek_/tmp4vshuhod_.zip

```diff
@@ -21,20 +21,20 @@
 
 Filename: phomber/__init__.py
 Comment: 
 
 Filename: phomber/phomber.py
 Comment: 
 
-Filename: phomber/phomberv3_beta.py
+Filename: phomber/phomberv3.0.2_beta.py
 Comment: 
 
 Filename: phomber/__pycache__/__init__.cpython-39.pyc
 Comment: 
 
 Filename: phomber/__pycache__/phomber.cpython-39.pyc
 Comment: 
 
-Filename: phomber/__pycache__/phomberv3_beta.cpython-39.pyc
+Filename: phomber/__pycache__/phomberv3.0.2_beta.cpython-39.pyc
 Comment: 
 
 Zip file comment:
```

## EGG-INFO/PKG-INFO

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phomber
-Version: 3.0.1
+Version: 3.0.2
 Summary: `PH0MBER` a simple yet powerful osint framework for reconnaissance and information gathering
 Home-page: https://github.com/s41r4j/phomber
 Author: s41r4j
 License: UNKNOWN
 Description: <p align=center>
                  <img src='.images/phomber_logo.png'>
         </p>
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: phomber Version: 3.0.1 Summary: `PH0MBER` a simple
+Metadata-Version: 2.1 Name: phomber Version: 3.0.2 Summary: `PH0MBER` a simple
 yet powerful osint framework for reconnaissance and information gathering Home-
 page: https://github.com/s41r4j/phomber Author: s41r4j License: UNKNOWN
 Description:
                           [.images/phomber_logo.png]
 ``` An open source infomation grathering & reconnaissance framework! ```
   [https://img.shields.io/badge/Etical_Hacking-OSINT-yellow.svg?logo=sharp]
 [https://img.shields.io/badge/Version-v3.0-orange.svg?logo=vectorworks] [https:
```

## EGG-INFO/SOURCES.txt

```diff
@@ -1,11 +1,11 @@
 README.md
 setup.py
 phomber/__init__.py
 phomber/phomber.py
-phomber/phomberv3_beta.py
+phomber/phomberv3.0.2_beta.py
 phomber.egg-info/PKG-INFO
 phomber.egg-info/SOURCES.txt
 phomber.egg-info/dependency_links.txt
 phomber.egg-info/entry_points.txt
 phomber.egg-info/requires.txt
 phomber.egg-info/top_level.txt
```

## EGG-INFO/entry_points.txt

```diff
@@ -1,3 +1,3 @@
 [console_scripts]
-phomber = phomber.phomberv3_beta:main
+phomber = phomber.phomber:main
```

## EGG-INFO/requires.txt

```diff
@@ -1,3 +1,6 @@
 beautifulsoup4
+dnspython
+mac-vendor-lookup
 phonenumbers
 psutil
+python-whois
```

## EGG-INFO/top_level.txt

```diff
@@ -1,2 +1 @@
 phomber
-phomberv3_beta
```

## phomber/phomber.py

```diff
@@ -1,17 +1,18 @@
 #!/usr/bin/python3
 
 #==============================================================================#
 #                                                                              #
-# [prog]   : Ph0mber                                                           #
-# [ver]    : 3.0 beta                                                          #
-# [desc]   : Multi-porpose osint framework for gathering information           #
+# [prog]   : PH0MBER                                                           #
+# [ver]    : 3.0.2 beta                                                        #
+# [desc]   : An open source infomation grathering & reconnaissance framework!  #
 # [dev]    : @s41r4j                                                           #
-# [github] : https://github.com/s41r4j/phomber                                 #
 # [license]: GNU GPLv3                                                         #
+# [github] : https://github.com/s41r4j/phomber                                 #
+# [pypi]   : https://pypi.org/project/phomber/                                 #
 #                                                                              #
 #==============================================================================#
 
 #==============================================================================#
 #                                                                              #
 #   [!] Legal/Ethical disclaimer:                                              #
 #                                                                              #
@@ -31,31 +32,38 @@
 import requests      # Default
 import os            # Default
 import sys           # Default
 import random        # Default
 import time          # Default
 import readline      # Default
 import re            # Default
+import uuid          # Default
+import socket        # Default
 import psutil        # pip install psutil
 import bs4           # pip install beautifulsoup4
 import phonenumbers  # pip install phonenumbers
+from mac_vendor_lookup import MacLookup # pip install mac-vendor-lookup
+import whois         # pip install python-whois
+import dns.resolver  # pip install dnspython
 
 
 # ------------------------ Global variables ------------------------ #
-avaliable_commands = ['help', 'exit', 'quit', 'dork', 'exp', 'check', 'clear', 'save', 'shell', 'info', 'change', 'number', 'ip']
+avaliable_commands = elements = ['change', 'check', 'clear', 'dork', 'dns', 'exit', 'exp', 'help', 'info', 'ip', 'mac', 'number', 'quit', 'save', 'shell', 'whois']
 prv_op = ''
+full_cmd = ''
 silent_mode = False
 
-
 # ------------------------ Scanner functions ------------------------ #
+
 # Check internet connection
-def check_connection(url):
+def check_connection():
     # Checking internet connection
+    urls = ['https://google.com', 'https://bing.com']
     try:
-        requests.get(url, timeout=10)
+        requests.get(random.choice(urls), timeout=10)
         return True
     except:
         return False
 
 # Reverse phone number lookup
 def number_lookup(phone_number):
     # Importing modules
@@ -65,29 +73,27 @@
     
     # Global variables
     global prv_op
     prv_op = '' # Resetting previous output
 
     # Information gathering about the number
     printit(f'    [+] Grathering information about \33[1;49;96m{phone_number}\33[1;49;93m...', coledt=[1, 49, 93], space_down=True)
-    prv_op += f'\n    \33[1;49;93m[#] Reverse phone number lookup for \33[1;49;96m{phone_number}\33[1;49;93m:\033[0m'+'\n'
+    prv_op += f'\n    \33[1;49;93m[#] Reverse phone number lookup for \33[1;49;96m{phone_number}\33[1;49;93m:\033[0m'+'\n\n'
 
     # Check if the number is valid or not (regex)
     if not re.match(r'^\+[1-9]\d{1,14}$', phone_number):
         printit('    > Invalid phone number format! (Example: +44xxxxxxxxxx)', coledt=[1, 49, 91])
-        prv_op += '    > Invalid phone number format! (Example: +44xxxxxxxxxx)'+'\n'
         return False
     
     # Country code check
     try:
         # Phone number format: (+Countrycode)xxxxxxxxxx
         phone_number_details = phonenumbers.parse(phone_number)
     except phonenumbers.phonenumberutil.NumberParseException:
         printit('    > Missing Country Code! (Example: +91, +44, +1)', coledt=[1, 49, 91])
-        prv_op += '    > Missing Country Code! (Example: +91, +44, +1)'+'\n'
         return False
 
     # extract country_code & only_number from "Country Code: xx National Number: xxxxxxxxxx"
     country_code = str(phone_number_details).split('Country Code:', 1)[1].split('National Number:', 1)[0].strip()
     only_number = str(phone_number_details).split('Country Code:', 1)[1].split('National Number:', 1)[1].strip()
     
     # Validating a phone number
@@ -130,14 +136,16 @@
         phone_number = str(phone_number)+' '*int(30-len(str(phone_number)))
         only_number = str(only_number)+' '*int(30-len(str(only_number)))
         r_format = str(r_format)+' '*int(30-len(str(r_format)))
         
         # Printing information
         final_output = f'''
     ┌──────────────────────────────────────────────────────┐
+    | Scanned Phone Number: \33[1;49;96m{phone_number}\033[0m |
+    |------------------------------------------------------|
     | INFORMATION         | DESCRIPTION                    |
     |------------------------------------------------------|
     | \33[1;49;97mPossible\033[0m            | {possible} |
     | \33[1;49;97mValid\033[0m               | {valid} |
     |------------------------------------------------------|
     | \33[1;49;97mCountry Code\033[0m        | {country_code} |
     | \33[1;49;97mCountry\033[0m             | {country} |
@@ -168,23 +176,29 @@
     \33[1;49;93m[+] Google Dork Queries:
 
     \33[1;49;92m> https://www.google.com/search?q={only_number.strip()}
     \033[0m'''
         print(google_dork_queries)
         prv_op += google_dork_queries+'\n'
 
+        # Scanning social media platforms
+        printit(f'    [+] Scanning social media platforms:', coledt=[1, 49, 93], space_down=True)
+
         return True
         
     else:
         # Reconfiguring variables
         possible = str(possible)+' '*int(30-len(str(possible)))
         valid = str(valid)+' '*int(30-len(str(valid)))
+        phone_number = str(phone_number)+' '*int(30-len(str(phone_number)))
 
         final_output = f'''
     ┌──────────────────────────────────────────────────────┐
+    | Scanned Phone Number: \33[1;49;96m{phone_number}\033[0m |
+    |------------------------------------------------------|
     | INFORMATION         | DESCRIPTION                    |
     |------------------------------------------------------|
     | \33[1;49;97mPossible\033[0m            | {possible} |
     | \33[1;49;97mValid\033[0m               | {valid} |
     └──────────────────────────────────────────────────────┘
         '''
         print(final_output)
@@ -195,28 +209,26 @@
 def ip_lookup(ip_address):
     # Global variables
     global prv_op
     prv_op = '' # Resetting previous output
     
     # Checking internet connection
     printit(f'    [+] Verifying internet connection...', coledt=[1, 49, 93], space_down=True)
-    if not check_connection('https://www.google.com'):
+    if not check_connection():
         printit('    > Internet connection not available!', coledt=[1, 49, 91], space_down=True)
-        prv_op += '\n    \33[1;49;91m> Internet connection not available!\033[0m'+'\n'
         return False
 
     # Information gathering about the ip address
     printit(f'    [+] Grathering information about \33[1;49;96m{ip_address}\33[1;49;93m...', coledt=[1, 49, 93], space_down=True)
-    prv_op += f'    \33[1;49;93m[#] Reverse ip address lookup for \33[1;49;96m{ip_address}\33[1;49;93m:\033[0m'+'\n'
+    prv_op += f'    \33[1;49;93m[#] Reverse ip address lookup for \33[1;49;96m{ip_address}\33[1;49;93m:\033[0m'+'\n\n'
 
     # Check if the ip address is valid or not (regex) [add IPv6 support]
     if not re.match(r'^\d{1,3}\.\d{1,3}\.\d{1,3}\.\d{1,3}$', ip_address) :
         printit('    > Invalid ip address format! (Example: 8.8.8.8)', coledt=[1, 49, 91])
-        prv_op += '   \33[1;49;91m> Invalid ip address format! (Example: 8.8.8.8)\033[0m'+'\n'
-        return 
+        return False
 
     # IP address lookup APIs
     ip_addresses = [f'http://ip-api.com/json/{ip_address}', f'https://ipapi.co/{ip_address}/json/', f'http://ipwho.is/{ip_address}']
     ip_address = str(ip_address)+' '*int(30-len(str(ip_address)))
 
     # Headers
     headers = {
@@ -264,15 +276,14 @@
             longitude = str(longitude)+' '*int(30-len(str(longitude)))
             ip = str(ip)+' '*int(30-len(str(ip)))
             
             # Printing information
             final_output = f'''
     ┌──────────────────────────────────────────────────────┐
     | Scanned IP Address: \33[1;49;96m{ip_address}\033[0m   |
-    | Server code name  : \33[1;49;96mreverse-ip-lookup-server-1\033[0m       |
     |------------------------------------------------------|
     | INFORMATION         | DESCRIPTION                    |
     |------------------------------------------------------|
     | \33[1;49;97mCountry\033[0m             | {country} |
     | \33[1;49;97mCountry Code\033[0m        | {countryCode} |
     | \33[1;49;97mRegion\033[0m              | {region} |
     | \33[1;49;97mRegion Code\033[0m         | {regionCode} |
@@ -291,15 +302,14 @@
             prv_op += final_output+'\n'
 
         except Exception as e:
             print(e)
             final_output = f'''
     ┌──────────────────────────────────────────────────────┐
     | Scanned IP Address: \33[1;49;96m{ip_address}\033[0m   |
-    | Server code name  : \33[1;49;96mreverse-ip-lookup-server-1\033[0m       |
     |------------------------------------------------------|
     | \33[1;49;91mFailed to Fetch information from this server!\033[0m        |
     └──────────────────────────────────────────────────────┘
     '''
             print(final_output)
             prv_op += final_output+'\n'
 
@@ -371,15 +381,14 @@
             asn = str(asn)+' '*int(30-len(str(asn)))
             org = str(org)+' '*int(30-len(str(org)))
             
             # Printing information
             final_output = f'''
     ┌──────────────────────────────────────────────────────┐
     | Scanned IP Address: \33[1;49;96m{ip_address}\033[0m   |
-    | Server code name  : \33[1;49;96mreverse-ip-lookup-server-2\033[0m       |
     |------------------------------------------------------|
     | INFORMATION         | DESCRIPTION                    |
     |------------------------------------------------------|
     | \33[1;49;97mIP Type\033[0m             | {version} |
     | \33[1;49;97mNetwork\033[0m             | {network} |
     |------------------------------------------------------|
     | \33[1;49;97mCountry\033[0m             | {country} |
@@ -414,15 +423,14 @@
             print(final_output)
             prv_op += final_output+'\n'
 
         except:
             final_output = f'''
     ┌──────────────────────────────────────────────────────┐
     | Scanned IP Address: \33[1;49;96m{ip_address}\033[0m   |
-    | Server code name  : \33[1;49;96mreverse-ip-lookup-server-2\033[0m       |
     |------------------------------------------------------|
     | \33[1;49;91mFailed to Fetch information from this server!\033[0m        |
     └──────────────────────────────────────────────────────┘
     '''
             print(final_output)
             prv_op += final_output+'\n'
 
@@ -498,15 +506,14 @@
             timezone_utc = str(timezone_utc)+' '*int(30-len(str(timezone_utc)))
             timezone_current_time = str(timezone_current_time)+' '*int(30-len(str(timezone_current_time)))
                     
             # Printing information
             final_output = f'''
     ┌──────────────────────────────────────────────────────┐
     | Scanned IP Address: \33[1;49;96m{ip_address}\033[0m   |
-    | Server code name  : \33[1;49;96mreverse-ip-lookup-server-3\033[0m       |
     |------------------------------------------------------|
     | INFORMATION         | DESCRIPTION                    |
     |------------------------------------------------------|
     | \33[1;49;97mIP Type\033[0m             | {ip_type} |
     |------------------------------------------------------|
     | \33[1;49;97mCountry\033[0m             | {country} |
     | \33[1;49;97mCountry Code\033[0m        | {country_code} |
@@ -541,24 +548,196 @@
             print(final_output)
             prv_op += final_output+'\n'
 
         except:
             final_output = f'''
     ┌──────────────────────────────────────────────────────┐
     | Scanned IP Address: \33[1;49;96m{ip_address}\033[0m   |
-    | Server code name  : \33[1;49;96mreverse-ip-lookup-server-3\033[0m       |
     |------------------------------------------------------|
     | \33[1;49;91mFailed to Fetch information from this server!\033[0m        |
     └──────────────────────────────────────────────────────┘
     '''
             print(final_output)
             prv_op += final_output+'\n'
 
     return True
 
+# Reverse mac address lookup
+def mac_lookup(mac_address):
+    # https://api.macvendors.com/<mac_address>
+    
+    # Global variables
+    global prv_op
+    prv_op = '' # Resetting previous output
+
+    # Information gathering about the mac address
+    printit(f'    [+] Grathering information about \33[1;49;96m{mac_address}\33[1;49;93m...', coledt=[1, 49, 93], space_down=True)
+    prv_op += f'    \33[1;49;93m[#] Reverse mac address lookup for \33[1;49;96m{mac_address}\33[1;49;93m:\033[0m'+'\n\n'
+
+    # Check if the mac address is valid or not (regex)
+    if not re.match(r'^([0-9A-Fa-f]{2}[:-]){5}([0-9A-Fa-f]{2})$', mac_address) :
+        printit('    > Invalid mac address format! (Example: 00:00:00:00:00:00)', coledt=[1, 49, 91])
+        return False
+
+    # Getting mac address vendor
+    try:
+        vendor = MacLookup().lookup(mac_address)
+        bol_val = True
+    except KeyError:
+        vendor = '\33[1;49;91mNot Found\033[0m'
+        bol_val = False
+
+    # Reconfiguring variables
+    mac_address = str(mac_address)+' '*int(31-len(str(mac_address)))
+    vendor = str(vendor)+' '*int(36-len(str(vendor)))
+
+    # Printing information
+    final_output = f'''
+    ┌──────────────────────────────────────────────────────┐
+    | Scanned MAC Address: \33[1;49;96m{mac_address}\033[0m |
+    |------------------------------------------------------|
+    | INFORMATION   | DESCRIPTION                          |
+    |------------------------------------------------------|
+    | \33[1;49;97mVendor\033[0m        | {vendor} |
+    └──────────────────────────────────────────────────────┘
+    '''
+    print(final_output)
+    prv_op += final_output+'\n'
+
+    return bol_val
+
+# Reverse whois lookup
+def whois_lookup(domain):
+    # Global variables
+    global prv_op
+    prv_op = '' # Resetting previous output
+
+    # Checking internet connection
+    printit(f'    [+] Verifying internet connection...', coledt=[1, 49, 93], space_down=True)
+    if not check_connection():
+        printit('    > Internet connection not available!', coledt=[1, 49, 91], space_down=True)
+        return False
+
+    # Information gathering about the domain
+    printit(f'    [+] Grathering information about \33[1;49;96m{domain}\33[1;49;93m...', coledt=[1, 49, 93], space_down=True)
+    prv_op += f'    \33[1;49;93m[#] Reverse whois lookup for \33[1;49;96m{domain}\33[1;49;93m:\033[0m'+'\n\n'
+
+    # Domain validation (regex)
+    if not re.match(r'^([a-zA-Z0-9]+(-[a-zA-Z0-9]+)*\.)+[a-zA-Z]{2,}$', domain) :
+        printit('    > Invalid domain format! (Example: example.com)', coledt=[1, 49, 91])
+        return False
+
+    # Getting whois information
+    try:
+        whois_info = whois.whois(domain)
+        bol_val = True
+    except:
+        bol_val = False
+
+    # Reconfiguring variables
+    domain = str(domain)+' '*int(36-len(str(domain)))
+
+    # Printing information
+    final_output = f'''
+    ┌──────────────────────────────────────────────────────┐
+    | Scanned Domain: \33[1;49;96m{domain}\033[0m |
+    |------------------------------------------------------|
+    | INFORMATION   | DESCRIPTION                          |
+    |------------------------------------------------------|'''
+
+    # If whois information is available
+    if bol_val:
+        # Loop through whois information & add it to the final output
+        for key, value in whois_info.items():
+            # Filtering out some keys
+            if key == 'status': continue
+            if key == 'expiration_date': key = 'expiry_date'
+            if key == 'registrant_postal_code': key = 'postal_code'
+
+            # Reconfiguring variables
+            key = key.replace('_', ' ').capitalize()
+
+            # Adding formatted information to the final output
+            if type(value) == list:
+                key = str(key)+' '*int(13-len(str(key)))
+                value_1 = str(value[0])+' '*int(36-len(str(value[0])))
+                final_output += f'''\n    | \33[1;49;97m{key}\033[0m | {value_1} |'''
+                if len(value) > 1:
+                    for i in range(1, len(value)):
+                        value_2 = str(value[i])+' '*int(36-len(str(value[i])))
+                        final_output += f'''\n    |               | {value_2} |'''
+            else:
+                key = str(key)+' '*int(13-len(str(key)))
+                value = str(value)+' '*int(36-len(str(value)))
+                final_output += f'''\n    | \33[1;49;97m{key}\033[0m | {value} |'''            
+    else:
+        final_output += f'''\n    | \33[1;49;97mInformation\033[0m   | \33[1;49;91mNot Found\033[0m{' '*int(36-len('Not Found'))} |'''
+
+    # Add the last part of the final output
+    final_output += f'''\n    └──────────────────────────────────────────────────────┘'''
+
+    print(final_output)
+    prv_op += final_output+'\n'
+
+    return bol_val
+
+# Reverse domain lookup
+def dns_lookup(ip_or_domain):
+    # Global variables
+    global prv_op
+    prv_op = '' # Resetting previous output
+
+    # Checking internet connection
+    printit(f'    [+] Verifying internet connection...', coledt=[1, 49, 93], space_down=True)
+    if not check_connection():
+        printit('    > Internet connection not available!', coledt=[1, 49, 91], space_down=True)
+        return False
+
+    # Information gathering about the domain    
+    printit(f'    [+] Grathering information about \33[1;49;96m{ip_or_domain}\33[1;49;93m...', coledt=[1, 49, 93], space_down=True)
+
+    # Validating ip address or domain name (regex)
+    if re.match(r'^([a-zA-Z0-9]+(-[a-zA-Z0-9]+)*\.)+[a-zA-Z]{2,}$', ip_or_domain):
+        prv_op += f'    \33[1;49;93m[#] DNS lookup for \33[1;49;96m{ip_or_domain}\33[1;49;93m:\033[0m'+'\n\n'
+        domain = ip_or_domain + ' '*int(36-len(ip_or_domain))
+        final_output_scanned = f'    | Scanned Domain: \33[1;49;96m{domain}\033[0m |'
+        try:
+            ip = socket.gethostbyname(ip_or_domain)
+            ip = str(ip)+' '*int(36-len(str(ip)))
+        except:
+            ip = '\33[1;49;91mNot Found\033[0m' + ' '*int(36-len('Not Found'))
+    elif re.match(r'^([0-9]{1,3}\.){3}[0-9]{1,3}$', ip_or_domain):
+        prv_op += f'    \33[1;49;93m[#] Reverse DNS lookup for \33[1;49;96m{ip_or_domain}\33[1;49;93m:\033[0m'+'\n\n'
+        ip = ip_or_domain + ' '*int(36-len(ip_or_domain))
+        final_output_scanned = f'    | Scanned IP: \33[1;49;96m{ip}\033[0m     |'
+        try:
+            domain = socket.gethostbyaddr(ip_or_domain)[0]
+            domain = str(domain)+' '*int(36-len(str(domain)))
+        except:
+            domain = '\33[1;49;91mNot Found\033[0m' + ' '*int(36-len('Not Found'))
+    else:
+        printit('    > Invalid ip address or domain name!', coledt=[1, 49, 91], space_down=True)
+        return False
+
+    # Expcepts: socket.gaierror, socket.herror
+
+    # Printing information
+    final_output_remaining = f'''
+    |------------------------------------------------------|
+    | INFORMATION   | DESCRIPTION                          |
+    |------------------------------------------------------|
+    | \33[1;49;97mIP\033[0m            | {ip} |
+    | \33[1;49;97mDomain\033[0m        | {domain} |
+    └──────────────────────────────────────────────────────┘
+    '''
+
+    print('\n    ┌──────────────────────────────────────────────────────┐\n'+final_output_scanned+final_output_remaining)
+    prv_op += '\n    ┌──────────────────────────────────────────────────────┐'+'\n'+final_output_scanned+final_output_remaining
+
+    return True
 
 # --------------------------- Basic functions ------------------------ #
 
 def printit(text, center='', line_up=False, line_down=False, space_up=False, space_down=False, coledt=[0, 0, 0], normaltxt_start='', normaltxt_end='', hide=False, verbose_mode=False, input_mode=False):
     if not hide or verbose_mode:
         # get terminal width
         width = os.get_terminal_size().columns
@@ -573,46 +752,63 @@
             new_width = int((width - len(text))/2)
             print(center*new_width, end='')
             print(f'\33[{coledt[0]};{coledt[1]};{coledt[2]}m', end='')
             if input_mode: input_var = input(text)
             else: print(str(text), end='')
             print('\033[0m', end='')
             print(center*new_width)
+        else:
+            print(f'\33[{coledt[0]};{coledt[1]};{coledt[2]}m', end='')
+            if input_mode: input_var = input(text)
+            else: print(str(text), end='')
+            print('\033[0m', end='')
 
         print(normaltxt_end, end='')
 
         if line_down: print('⸺'*width)
         if space_down: print()
 
         if input_mode: return input_var
 
 def save_output(prv_cmd):
     try:
-        filename = prv_cmd+'_'+str(time.strftime("%d-%m-%Y_%H-%M-%S"))+'.txt'
+        filename = prv_cmd+'_ph0mber_'+str(time.strftime("%d-%m-%Y_%H-%M-%S"))+'.txt'
         pwd = os.getcwd()
         os_name = os.uname()
         path = pwd+'/'+filename
 
         file_save_info = f'''
     \33[1;49;93m[#] Output File Name: \33[1;49;97m{filename}\033[0m
     \33[1;49;93m[#] Output File Path: \33[1;49;97m{path}\033[0m
         '''
         print(file_save_info)
+    
+        header = f'''
+    \33[1;49;93m[@] Osint framework: \33[1;49;96mPH0MBER
+    \33[1;49;93m[@] Github: \33[1;49;96mhttps://github.com/s41r4j/phomber
+
+    \33[1;49;93m[#] Output File Name: \33[1;49;97m{filename}
+    \33[1;49;93m[#] Output File Path: \33[1;49;97m{path}
+    \33[1;49;93m[#] Date: \33[1;49;97m{str(time.strftime("%d-%m-%Y"))}
+    \33[1;49;93m[#] Time: \33[1;49;97m{str(time.strftime("%H:%M:%S"))}
+
+    \33[1;49;93m[#] Command Executed: \33[1;49;96m{full_cmd.strip()}\n'''
 
         with open(path, 'w') as f:
+            f.write(header)
             f.write(prv_op)
     
         printit(f'    [+] Excute following commands to view output:', coledt=[1, 49, 93], space_down=True, space_up=True)
         
         if os_name == 'nt':
-            exe_cmd = f'''    \33[1;49;92m> shell more {path}\033[0m
-    \33[1;49;92m> shell type {path}\033[0m'''
+            exe_cmd = f'''    \33[1;49;93m> \33[1;49;92mshell more {filename}\033[0m
+    \33[1;49;93m> \33[1;49;92mshell type {filename}\033[0m'''
         else:
-            exe_cmd = f'''    \33[1;49;92m> shell cat {path}\033[0m
-    \33[1;49;92m> shell less {path}\033[0m'''
+            exe_cmd = f'''    \33[1;49;93m> \33[1;49;92mshell cat {filename}\033[0m
+    \33[1;49;93m> \33[1;49;92mshell less {filename}\033[0m'''
         print(exe_cmd)
 
         return True
     except:
         printit(f'    [!] Output could not be saved!', coledt=[1, 49, 91], space_down=True)
         return False
 
@@ -704,91 +900,107 @@
     # Variables
     user = '\33[1;49;96m'+str(os.getlogin())+'\033[0m'+ ' '*int(34-len(str(os.getlogin())))
     hostname = '\33[1;49;96m'+str(os.uname().nodename)+'\033[0m'+' '*int(34-len(str(os.uname().nodename)))
     os_name = '\33[1;49;96m'+str(os.uname().sysname)+'\033[0m'+' '*int(34-len(str(os.uname().sysname)))
     ram = '\33[1;49;96m'+str(psutil.virtual_memory().percent)+"%"+'\033[0m'+' '*int(33-len(str(psutil.virtual_memory().percent)))
     cpu = '\33[1;49;96m'+str(psutil.cpu_percent())+"%"+'\033[0m'+' '*int(32-len(str(psutil.cpu_percent())))
     disk = '\33[1;49;96m'+str(psutil.disk_usage('/').percent)+"%"+'\033[0m'+' '*int(33-len(str(psutil.disk_usage('/').percent)))
+    sys_mac = '\33[1;49;96m'+str(':'.join(re.findall('..', '%012x' % uuid.getnode())))+'\033[0m'+' '*int(34-len(str(':'.join(re.findall('..', '%012x' % uuid.getnode())))))
+    arch = '\33[1;49;96m'+str(os.uname().machine)+'\033[0m'+' '*int(34-len(str(os.uname().machine)))
 
-    ver = '\33[1;49;96m3.0 beta\033[0m'+' '*int(34-len(str(3.0)))
+    ver = '\33[1;49;96m3.0.2 (beta)\033[0m'+' '*int(34-len(str('3.0.2 (beta)')))
 
     sysinfo = f'''
     ┌────────────────────────────────────────────────────┐
     | SYSTEM INFO   | DESCRIPTION                        |
     |----------------------------------------------------|
     | \33[1;49;97mUser\033[0m          | {user} |
     | \33[1;49;97mHostname\033[0m      | {hostname} |
     | \33[1;49;97mOS\033[0m            | {os_name} |
+    | \33[1;49;97mArchitecture\033[0m  | {arch} |
+    | \33[1;49;97mSystem MAC\033[0m    | {sys_mac} |
+    |----------------------------------------------------|
     | \33[1;49;97mRAM Usage\033[0m     | {ram} |
     | \33[1;49;97mCPU Usage\033[0m     | {cpu} |
     | \33[1;49;97mDisk Usage\033[0m    | {disk} |
     └────────────────────────────────────────────────────┘
 
     ┌────────────────────────────────────────────────────┐
     | FRAMEWORK INFO| DESCRIPTION                        |
     |----------------------------------------------------|
     | \33[1;49;97mName\033[0m          | \33[1;49;96mPH0MBER\033[0m                            |
     | \33[1;49;97mVersion\033[0m       | {ver} |
-    | \33[1;49;97mType\033[0m          | \33[1;49;96mOSINT\033[0m                              |
-    | \33[1;49;97mAuthor\033[0m        | \33[1;49;96ms41r4j\033[0m                             |
+    | \33[1;49;97mType\033[0m          | \33[1;49;96mOSINT Framework\033[0m                    |
+    | \33[1;49;97mDeveloper\033[0m     | \33[1;49;96ms41r4j\033[0m                             |
     | \33[1;49;97mGithub\033[0m        | \33[1;49;96mhttps://github.com/s41r4j/phomber\033[0m  |
     └────────────────────────────────────────────────────┘
     '''
 
     help = '''
     ┌────────────────────────────────────────────────────┐
     | COMMANDS      | DESCRIPTION                        |
     |----------------------------------------------------|
     |                <Basic Commands>                    |
     |----------------------------------------------------|
     | \33[1;49;97mhelp\033[0m          | Display this help menu             | 
     | \33[1;49;97mexit/quit\033[0m     | Exit the framework                 |
-    | \33[1;49;97mdork\033[0m          | Show a random google dork query    |  
+    | \33[1;49;97mdork\033[0m          | Show a random google dork query *  |  
     | \33[1;49;97mexp\033[0m           | Show info about all available      |       
     |               | expressions                        |
     | \33[1;49;97mcheck\033[0m         | Check internet connection          |
     | \33[1;49;97mclear\033[0m         | Clear screen                       |
     | \33[1;49;97msave\033[0m          | Save output of previous scanner    |
     |               | command in a file                  |
     | \33[1;49;97mshell <cmd>\033[0m   | Execute native shell/cmd commands  |
     | \33[1;49;97minfo\033[0m          | Show info about framework & system |
     | \33[1;49;97mchange\033[0m        | Change user command input color    |
     |----------------------------------------------------|
     |                 <Scanner Commands>                 |
     |----------------------------------------------------|
-    | \33[1;49;97mnumber\033[0m        | Reverse phone number lookup        |
-    | \33[1;49;97mip\033[0m            | Reverse ip address lookup          |
+    | \33[1;49;97mnumber\033[0m        | Reverse phone number lookup *      |
+    | \33[1;49;97mip\033[0m            | Reverse ip address lookup *        |
+    | \33[1;49;97mmac\033[0m           | Reverse mac address lookup         |
+    | \33[1;49;97mwhois\033[0m         | Reverse whois lookup *             |
+    | \33[1;49;97mdns\033[0m           | Reverse or normal DNS lookup       |
+    |----------------------------------------------------|
     | \33[1;49;91mMORE SCANNERS COMING SOON, THIS IS A BETA VER\033[0m      |
     └────────────────────────────────────────────────────┘
+    '''
 
-    \33[1;49;93m> Type `help <command>` to see more info about a command\033[0m
-    \33[1;49;93m> Use `Tab` key to auto-complete commands\033[0m
-    \33[1;49;93m> Try silent mode by using `-s`/`--silent` flag\033[0m'''
+    tips = ['Type `\33[7;49;93mhelp <command>\033[0m\33[1;49;93m` to see more info about a command',
+            'Use `\33[7;49;93mTab\033[0m\33[1;49;93m` key to auto-complete commands',
+            'Try silent mode by using `\33[7;49;93m-s\033[0m\33[1;49;93m`/`\33[7;49;93m--silent\033[0m\33[1;49;93m` flag',
+            'You can also use `\33[7;49;93mCtrl+C\033[0m\33[1;49;93m` to exit',
+            'Descriptions ending with `\33[7;49;93m*\033[0m\33[1;49;93m` needs internet connection'
+            ]
 
     # Previous command
     prv_cmd = ''
-    global prv_op
+    global prv_op 
+    global full_cmd
 
     # Setting up auto-complete
     readline.parse_and_bind('tab: complete')
     readline.set_completer(completer)
 
     # Command prompt color
     cmd_color = ['\33[1;49;90m', '\33[1;49;97m']
     crt_color = cmd_color[1]
 
     # Control center loop
     while True:
         # [user@phomber]⸺[:D] $
-        cmd = (printit(f'\n[{user.strip()}@ph0mber]⸺ [{crt_exp}] $ {crt_color}', input_mode=True, space_up=True)).strip()
+        cmd = (printit(f'\n\033[0m[{user.strip()}@ph0mber]⸺ [{crt_exp}] $ {crt_color}', input_mode=True, space_up=True)).strip()
 
         if cmd == 'help':
             crt_exp = exp[1]
             prv_op = ''
             print(help)
+            tip = random.choice(tips)
+            print(f'\33[1;49;93m    > {tip}\033[0m')
         elif cmd[:4] == 'help':
             if (cmd+'#')[4] == ' ':
                 cmd = cmd[5:]
                 if cmd == 'help':
                     crt_exp = exp[1]
                     help_help = '''  \33[1;49;93m[+] Command Info: \33[1;49;93mhelp\n
     \33[1;49;92m> DESCRIPTION: \33[1;49;97mWhen you type `help`, the help menu will be displayed
@@ -864,46 +1076,63 @@
     \33[1;49;92m> SYNTAX: \33[1;49;97mchange <color_code>
     \33[1;49;92m> EXAMPLE: \33[1;49;97mchange 0
     \033[0m'''
                     print(change_help)
                 elif cmd == 'number':
                     crt_exp = exp[1]
                     number_help = '''  \33[1;49;93m[+] Command Info: \33[1;49;93mnumber\n
-    \33[1;49;92m> DESCRIPTION: \33[1;49;97mWhen you type `number`, it will perform reverse phone number lookup
+    \33[1;49;92m> DESCRIPTION: \33[1;49;97mWhen you type `number`, it will reverse lookup phone number over internet and show public info associated with it
     \33[1;49;92m> SYNTAX: \33[1;49;97mnumber <phone_number>
     \33[1;49;92m> EXAMPLE: \33[1;49;97mnumber +1234567890
     \033[0m'''
                     print(number_help)
-                elif cmd == 'email':
+                elif cmd == 'whois':
+                    crt_exp = exp[1]
+                    whois_help = '''  \33[1;49;93m[+] Command Info: \33[1;49;93mwhois\n
+    \33[1;49;92m> DESCRIPTION: \33[1;49;97mWhen you type `whois`, it will perform reverse whois lookup
+    \33[1;49;92m> SYNTAX: \33[1;49;97mwhois <domain_name>
+    \33[1;49;92m> EXAMPLE: \33[1;49;97mwhois example.com
+    \033[0m'''
+                    print(whois_help)
+                elif cmd == 'dns':
                     crt_exp = exp[1]
-                    email_help = f'''  \33[1;49;93m[+] Command Info: \33[1;49;93memail\n
-    \33[1;49;92m> DESCRIPTION: \33[1;49;97mWhen you type `email`, it will perform reverse email lookup
-    \33[1;49;92m> SYNTAX: \33[1;49;97memail <email_address>
-    \33[1;49;92m> EXAMPLE: \33[1;49;97memail {user.strip()}\33[1;49;96m@gmail.com
+                    dns_help = '''  \33[1;49;93m[+] Command Info: \33[1;49;93mdns\n
+    \33[1;49;92m> DESCRIPTION: \33[1;49;97mWhen you type `dns`, it will perform dns lookup for given domain name or reverse dns lookup for given ip address
+    \33[1;49;92m> SYNTAX: \33[1;49;97mdns <ip_address/domain_name>
+    \33[1;49;92m> EXAMPLE: \33[1;49;97mdns 192.168.1.1 \33[1;49;92mOR \33[1;49;97mdns example.com
     \033[0m'''
-                    print(email_help)
+                    print(dns_help)
                 elif cmd == 'ip':
                     crt_exp = exp[1]
                     ip_help = '''  \33[1;49;93m[+] Command Info: \33[1;49;93mip\n
-    \33[1;49;92m> DESCRIPTION: \33[1;49;97mWhen you type `ip`, it will perform reverse ip address lookup
+    \33[1;49;92m> DESCRIPTION: \33[1;49;97mWhen you type `ip`, it will perform an ip address lookup over internet and show info about given ip address
     \33[1;49;92m> SYNTAX: \33[1;49;97mip <ip_address>
     \33[1;49;92m> EXAMPLE: \33[1;49;97mip 8.8.8.8
     \033[0m'''
                     print(ip_help)
+                elif cmd == 'mac':
+                    crt_exp = exp[1]
+                    mac_help = '''  \33[1;49;93m[+] Command Info: \33[1;49;93mmac\n
+    \33[1;49;92m> DESCRIPTION: \33[1;49;97mWhen you type `mac`, it will lookup probable vendor/manufacture of given mac address
+    \33[1;49;92m> SYNTAX: \33[1;49;97mmac <mac_address>
+    \33[1;49;92m> EXAMPLE: \33[1;49;97mmac ff:ff:ff:ff:ff:ff
+    \033[0m'''
+                    print(mac_help)
                 else:
                     crt_exp = exp[3]
                     printit('    [!] Invalid sub-command! Type `help` to see all available commands.', coledt=[1, 49, 91])
             else:
                 crt_exp = exp[3]
                 printit('    [!] Invalid command! Type `help` to see all available commands.', coledt=[1, 49, 91])
             prv_op = ''
 
         # Basic commands
         elif cmd == 'exit' or cmd == 'quit':
-            printit('    [@] Thank you for using `PH0MBER` osint framework :)', coledt=[1, 49, random.choice([92, 96, 97])])
+            if not silent_mode: printit('    [@] Thank you for using `PH0MBER` osint framework :)', coledt=[1, 49, random.choice([92, 96, 97])])
+            # printit('    [@] Support this project: https://www.buymeacoffee.com/s41r4j', coledt=[1, 49, random.choice([92, 97])])
             raise KeyboardInterrupt
         elif cmd == 'dork':
             crt_exp = exp[1]
             prv_op = ''
             printit('    [+] Generating random dork query...', coledt=[1, 49, 93], space_down=True)
             printit('    > '+dork_query(), coledt=[1, 49, 92])
         elif cmd == 'exp':
@@ -959,15 +1188,15 @@
                 print(exec_cmd)
             
                 output = os.system(cmd)
                 if output == 0:
                     printit('> Command executed successfully!', coledt=[7, 49, 92], normaltxt_start='\n    ')
                     crt_exp = exp[0]
                 else:
-                    printit('\n    > Command execution failed!', coledt=[1, 49, 91])
+                    printit('> Command execution failed!', coledt=[7, 49, 91], normaltxt_start='\n    ')
                     crt_exp = exp[3]
             else:
                 crt_exp = exp[3]
                 printit('    [!] Invalid command! Type `help` to see all available commands.', coledt=[1, 49, 91])
             prv_op = ''
         elif cmd == 'info':
             crt_exp = exp[1]
@@ -997,35 +1226,87 @@
             prv_op = ''
 
         # Scanner commands
         elif cmd == 'number':
             crt_exp = exp[2]
             printit('    > No phone number found! Type `help number` to see more info', coledt=[1, 49, 91])
         elif cmd[:6] == 'number':
+            full_cmd = cmd
             if (cmd+'#')[6]  == ' ':
                 cmd = cmd[7:]
                 printit('    [+] Performing reverse phone number lookup...', coledt=[1, 49, 93], space_down=True)
                 if number_lookup(cmd):
                     crt_exp = exp[4]
                 else:
                     crt_exp = exp[3]
+                    prv_op = ''
             else:
                 crt_exp = exp[3]
                 printit('    [!] Invalid command! Type `help` to see all available commands.', coledt=[1, 49, 91])
         elif cmd == 'ip':
             crt_exp = exp[2]
             printit('    > No ip address found! Type `help ip` to see more info', coledt=[1, 49, 91])
         elif cmd[:2] == 'ip':
+            full_cmd = cmd
             if (cmd+'#')[2]  == ' ':
                 cmd = cmd[3:]
                 printit('    [+] Performing reverse ip address lookup...', coledt=[1, 49, 93], space_down=True)
                 if ip_lookup(cmd):
                     crt_exp = exp[4]
                 else:
                     crt_exp = exp[3]
+                    prv_op = ''
+            else:
+                crt_exp = exp[3]
+                printit('    [!] Invalid command! Type `help` to see all available commands.', coledt=[1, 49, 91])
+        elif cmd == 'mac':
+            crt_exp = exp[2]
+            printit('    > No mac address found! Type `help mac` to see more info', coledt=[1, 49, 91])
+        elif cmd[:3] == 'mac':
+            full_cmd = cmd
+            if (cmd+'#')[3]  == ' ':
+                cmd = cmd[4:]
+                printit('    [+] Performing reverse mac address lookup...', coledt=[1, 49, 93], space_down=True)
+                if mac_lookup(cmd):
+                    crt_exp = exp[4]
+                else:
+                    crt_exp = exp[3]
+                    prv_op = ''
+            else:
+                crt_exp = exp[3]
+                printit('    [!] Invalid command! Type `help` to see all available commands.', coledt=[1, 49, 91])
+        elif cmd == 'whois':
+            crt_exp = exp[2]
+            printit('    > No domain found! Type `help whois` to see more info', coledt=[1, 49, 91])
+        elif cmd[:5] == 'whois':
+            full_cmd = cmd
+            if (cmd+'#')[5]  == ' ':
+                cmd = cmd[6:]
+                printit('    [+] Performing reverse domain lookup...', coledt=[1, 49, 93], space_down=True)
+                if whois_lookup(cmd):
+                    crt_exp = exp[4]
+                else:
+                    crt_exp = exp[3]
+                    prv_op = ''
+            else:
+                crt_exp = exp[3]
+                printit('    [!] Invalid command! Type `help` to see all available commands.', coledt=[1, 49, 91])
+        elif cmd == 'dns':
+            crt_exp = exp[2]
+            printit('    > No domain found! Type `help dns` to see more info', coledt=[1, 49, 91])
+        elif cmd[:3] == 'dns':
+            full_cmd = cmd
+            if (cmd+'#')[3]  == ' ':
+                cmd = cmd[4:]
+                printit('    [+] Performing dns lookup...', coledt=[1, 49, 93], space_down=True)
+                if dns_lookup(cmd):
+                    crt_exp = exp[4]
+                else:
+                    crt_exp = exp[3]
+                    prv_op = ''
             else:
                 crt_exp = exp[3]
                 printit('    [!] Invalid command! Type `help` to see all available commands.', coledt=[1, 49, 91])
 
         # If command is not available
         else:
             crt_exp = exp[3]
@@ -1052,10 +1333,9 @@
     try:
         control_center()
     except KeyboardInterrupt:
         print()
         if not silent_mode:
             printit('[#] Terminating `PH0MBER` framework...', coledt=[1, 49, random.choice([91, 93])], space_down=True, line_down=True, line_up=True, space_up=True)
             exit()
+        else: print()
 
-# if __name__ == '__main__':
-#     main()
```

## phomber/__pycache__/phomber.cpython-39.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Sun May 21 13:03:15 2023 UTC, .py size: 55263 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,2091 +1,2524 @@
-00000000: 610d 0d0a 0000 0000 9316 6a64 dfd7 0000  a.........jd....
+00000000: 610d 0d0a 0000 0000 48ff 7a64 610d 0100  a.......H.zda...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 000b 0000 0040 0000 0073 d000 0000 6400  .....@...s....d.
+00000020: 000b 0000 0040 0000 0073 1c01 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6401 6c03 5a03 6400  d.l.Z.d.d.l.Z.d.
 00000050: 6401 6c04 5a04 6400 6401 6c05 5a05 6400  d.l.Z.d.d.l.Z.d.
 00000060: 6401 6c06 5a06 6400 6401 6c07 5a07 6400  d.l.Z.d.d.l.Z.d.
-00000070: 6401 6c08 5a08 6400 6401 6c09 5a09 6700  d.l.Z.d.d.l.Z.g.
-00000080: 6402 a201 5a0a 6403 610b 6404 610c 6405  d...Z.d.a.d.a.d.
-00000090: 6406 8400 5a0d 6407 6408 8400 5a0e 6409  d...Z.d.d...Z.d.
-000000a0: 640a 8400 5a0f 6403 6404 6404 6404 6404  d...Z.d.d.d.d.d.
-000000b0: 6700 640b a201 6403 6403 6404 6404 6404  g.d...d.d.d.d.d.
-000000c0: 660b 640c 640d 8401 5a10 640e 640f 8400  f.d.d...Z.d.d...
-000000d0: 5a11 6410 6411 8400 5a12 6412 6413 8400  Z.d.d...Z.d.d...
-000000e0: 5a13 6414 6415 8400 5a14 6416 6417 8400  Z.d.d...Z.d.d...
-000000f0: 5a15 6418 6419 8400 5a16 6401 5300 291a  Z.d.d...Z.d.S.).
-00000100: e900 0000 004e 290d da04 6865 6c70 da04  .....N)...help..
-00000110: 6578 6974 da04 7175 6974 da04 646f 726b  exit..quit..dork
-00000120: da03 6578 70da 0563 6865 636b da05 636c  ..exp..check..cl
-00000130: 6561 72da 0473 6176 65da 0573 6865 6c6c  ear..save..shell
-00000140: da04 696e 666f da06 6368 616e 6765 da06  ..info..change..
-00000150: 6e75 6d62 6572 da02 6970 da00 4663 0100  number..ip..Fc..
-00000160: 0000 0000 0000 0000 0000 0100 0000 0600  ................
-00000170: 0000 4300 0000 7328 0000 007a 1474 006a  ..C...s(...z.t.j
-00000180: 017c 0064 0164 028d 0201 0057 0064 0353  .|.d.d.....W.d.S
-00000190: 0001 0001 0001 0059 0064 0453 0030 0064  .......Y.d.S.0.d
-000001a0: 0053 0029 054e e90a 0000 0029 01da 0774  .S.).N.....)...t
-000001b0: 696d 656f 7574 5446 2902 da08 7265 7175  imeoutTF)...requ
-000001c0: 6573 7473 da03 6765 7429 01da 0375 726c  ests..get)...url
-000001d0: a900 7215 0000 00fa 2f62 7569 6c64 2f62  ..r...../build/b
-000001e0: 6469 7374 2e6c 696e 7578 2d78 3836 5f36  dist.linux-x86_6
-000001f0: 342f 6567 672f 7068 6f6d 6265 722f 7068  4/egg/phomber/ph
-00000200: 6f6d 6265 722e 7079 da10 6368 6563 6b5f  omber.py..check_
-00000210: 636f 6e6e 6563 7469 6f6e 3300 0000 730a  connection3...s.
-00000220: 0000 0000 0202 010e 0106 0106 0172 1700  .............r..
-00000230: 0000 6301 0000 0000 0000 0000 0000 0014  ..c.............
-00000240: 0000 0015 0000 0043 0000 0073 3e04 0000  .......C...s>...
-00000250: 6401 6402 6c00 6d01 7d01 0100 6401 6403  d.d.l.m.}...d.d.
-00000260: 6c00 6d02 7d02 0100 6401 6404 6c00 6d03  l.m.}...d.d.l.m.
-00000270: 7d03 0100 6405 6104 7405 6406 7c00 9b00  }...d.a.t.d.|...
-00000280: 6407 9d03 6700 6408 a201 6409 640a 8d03  d...g.d...d.d...
-00000290: 0100 7404 640b 7c00 9b00 640c 9d03 640d  ..t.d.|...d...d.
-000002a0: 1700 3700 6104 7406 a007 640e 7c00 a102  ..7.a.t...d.|...
-000002b0: 737e 7405 640f 6700 6410 a201 6411 8d02  s~t.d.g.d...d...
-000002c0: 0100 7404 6412 3700 6104 6413 5300 7a0e  ..t.d.7.a.d.S.z.
-000002d0: 7400 a008 7c00 a101 7d04 5700 6e30 0400  t...|...}.W.n0..
-000002e0: 7400 6a09 6a0a 79bc 0100 0100 0100 7405  t.j.j.y.......t.
-000002f0: 6414 6700 6410 a201 6411 8d02 0100 7404  d.g.d...d.....t.
-00000300: 6415 3700 6104 5900 6413 5300 3000 740b  d.7.a.Y.d.S.0.t.
-00000310: 7c04 8301 a00c 6416 6417 a102 6417 1900  |.....d.d...d...
-00000320: a00c 6418 6417 a102 6401 1900 a00d a100  ..d.d...d.......
-00000330: 7d05 740b 7c04 8301 a00c 6416 6417 a102  }.t.|.....d.d...
-00000340: 6417 1900 a00c 6418 6417 a102 6417 1900  d.....d.d...d...
-00000350: a00d a100 7d06 7400 a00e 7c04 a101 7d07  ....}.t...|...}.
-00000360: 7400 a00f 7c04 a101 7d08 7c07 9003 72d0  t...|...}.|...r.
-00000370: 7c08 9003 72d0 7400 a008 7c00 6419 a102  |...r.t...|.d...
-00000380: 7d09 7400 a010 7c04 a101 7d0a 7c03 a011  }.t...|...}.|...
-00000390: 7c09 641a a102 7d0b 7400 a008 7c00 641b  |.d...}.t...|.d.
-000003a0: a102 7d0c 7c02 a012 7c0c 641a a102 7d0d  ..}.|...|.d...}.
-000003b0: 740b 7c01 a013 7c04 a101 8301 7d0e 7c0e  t.|...|.....}.|.
-000003c0: a014 641c 6405 a102 a014 641d 6405 a102  ..d.d.....d.d...
-000003d0: a014 641e 6405 a102 a014 641f 6405 a102  ..d.d.....d.d...
-000003e0: a014 6420 6405 a102 a014 6421 6405 a102  ..d d.....d!d...
-000003f0: a014 6422 6405 a102 7d0f 7400 a015 7c04  ..d"d...}.t...|.
-00000400: 7400 6a16 6a17 a102 a014 6423 6405 a102  t.j.j.....d#d...
-00000410: 7d10 740b 7c08 8301 6422 7418 6424 7419  }.t.|...d"t.d$t.
-00000420: 740b 7c08 8301 8301 1800 8301 1400 1700  t.|.............
-00000430: 7d08 740b 7c07 8301 6422 7418 6424 7419  }.t.|...d"t.d$t.
-00000440: 740b 7c07 8301 8301 1800 8301 1400 1700  t.|.............
-00000450: 7d07 740b 7c05 8301 6422 7418 6424 7419  }.t.|...d"t.d$t.
-00000460: 740b 7c05 8301 8301 1800 8301 1400 1700  t.|.............
-00000470: 7d05 740b 7c0b 8301 6422 7418 6424 7419  }.t.|...d"t.d$t.
-00000480: 740b 7c0b 8301 8301 1800 8301 1400 1700  t.|.............
-00000490: 7d0b 740b 7c0a 8301 6422 7418 6424 7419  }.t.|...d"t.d$t.
-000004a0: 740b 7c0a 8301 8301 1800 8301 1400 1700  t.|.............
-000004b0: 7d0a 740b 7c0d 8301 6422 7418 6424 7419  }.t.|...d"t.d$t.
-000004c0: 740b 7c0d 8301 8301 1800 8301 1400 1700  t.|.............
-000004d0: 7d0d 740b 7c0f 8301 6422 7418 6424 7419  }.t.|...d"t.d$t.
-000004e0: 740b 7c0f 8301 8301 1800 8301 1400 1700  t.|.............
-000004f0: 7d0f 740b 7c00 8301 6422 7418 6424 7419  }.t.|...d"t.d$t.
-00000500: 740b 7c00 8301 8301 1800 8301 1400 1700  t.|.............
-00000510: 7d00 740b 7c06 8301 6422 7418 6424 7419  }.t.|...d"t.d$t.
-00000520: 740b 7c06 8301 8301 1800 8301 1400 1700  t.|.............
-00000530: 7d06 740b 7c10 8301 6422 7418 6424 7419  }.t.|...d"t.d$t.
-00000540: 740b 7c10 8301 8301 1800 8301 1400 1700  t.|.............
-00000550: 7d10 6425 7c08 9b00 6426 7c07 9b00 6427  }.d%|...d&|...d'
-00000560: 7c05 9b00 6428 7c0b 9b00 6429 7c0a 9b00  |...d(|...d)|...
-00000570: 642a 7c0d 9b00 642b 7c0f 9b00 642c 7c00  d*|...d+|...d,|.
-00000580: 9b00 642d 7c06 9b00 642e 7c10 9b00 642f  ..d-|...d.|...d/
-00000590: 9d15 7d11 741a 7c11 8301 0100 7404 7c11  ..}.t.|.....t.|.
-000005a0: 640d 1700 3700 6104 6430 7c00 a00d a100  d...7.a.d0|.....
-000005b0: 9b00 6431 7c0a a00d a100 9b00 6432 7c06  ..d1|.......d2|.
-000005c0: a00d a100 9b00 6433 7c0a a00d a100 a01b  ......d3|.......
-000005d0: a100 9b00 6432 7c06 a00d a100 9b00 6434  ....d2|.......d4
-000005e0: 9d0b 7d12 741a 7c12 8301 0100 7404 7c12  ..}.t.|.....t.|.
-000005f0: 640d 1700 3700 6104 6435 7c06 a00d a100  d...7.a.d5|.....
-00000600: 9b00 6434 9d03 7d13 741a 7c13 8301 0100  ..d4..}.t.|.....
-00000610: 7404 7c13 640d 1700 3700 6104 6409 5300  t.|.d...7.a.d.S.
-00000620: 740b 7c08 8301 6422 7418 6424 7419 740b  t.|...d"t.d$t.t.
-00000630: 7c08 8301 8301 1800 8301 1400 1700 7d08  |.............}.
-00000640: 740b 7c07 8301 6422 7418 6424 7419 740b  t.|...d"t.d$t.t.
-00000650: 7c07 8301 8301 1800 8301 1400 1700 7d07  |.............}.
-00000660: 6425 7c08 9b00 6426 7c07 9b00 642f 9d05  d%|...d&|...d/..
-00000670: 7d11 741a 7c11 8301 0100 7404 7c11 640d  }.t.|.....t.|.d.
-00000680: 1700 3700 6104 6413 5300 6400 5300 2936  ..7.a.d.S.d.S.)6
-00000690: 4e72 0100 0000 2901 da08 7469 6d65 7a6f  Nr....)...timezo
-000006a0: 6e65 2901 da07 6361 7272 6965 7229 01da  ne)...carrier)..
-000006b0: 0867 656f 636f 6465 7272 0f00 0000 fa2f  .geocoderr...../
-000006c0: 2020 2020 5b2b 5d20 4772 6174 6865 7269      [+] Gratheri
-000006d0: 6e67 2069 6e66 6f72 6d61 7469 6f6e 2061  ng information a
-000006e0: 626f 7574 201b 5b31 3b34 393b 3936 6dfa  bout .[1;49;96m.
-000006f0: 0d1b 5b31 3b34 393b 3933 6d2e 2e2e a903  ..[1;49;93m.....
-00000700: e901 0000 00e9 3100 0000 e95d 0000 0054  ......1....]...T
-00000710: a902 da06 636f 6c65 6474 da0a 7370 6163  ....coledt..spac
-00000720: 655f 646f 776e 7a3d 0a20 2020 201b 5b31  e_downz=.    .[1
-00000730: 3b34 393b 3933 6d5b 235d 2052 6576 6572  ;49;93m[#] Rever
-00000740: 7365 2070 686f 6e65 206e 756d 6265 7220  se phone number 
-00000750: 6c6f 6f6b 7570 2066 6f72 201b 5b31 3b34  lookup for .[1;4
-00000760: 393b 3936 6dfa 0f1b 5b31 3b34 393b 3933  9;96m...[1;49;93
-00000770: 6d3a 1b5b 306d da01 0a7a 115e 5c2b 5b31  m:.[0m...z.^\+[1
-00000780: 2d39 5d5c 647b 312c 3134 7d24 7a3b 2020  -9]\d{1,14}$z;  
-00000790: 2020 3e20 496e 7661 6c69 6420 7068 6f6e    > Invalid phon
-000007a0: 6520 6e75 6d62 6572 2066 6f72 6d61 7421  e number format!
-000007b0: 2028 4578 616d 706c 653a 202b 3434 7878   (Example: +44xx
-000007c0: 7878 7878 7878 7878 29a9 0372 1e00 0000  xxxxxxxx)..r....
-000007d0: 721f 0000 00e9 5b00 0000 a901 7222 0000  r.....[.....r"..
-000007e0: 007a 3c20 2020 203e 2049 6e76 616c 6964  .z<    > Invalid
-000007f0: 2070 686f 6e65 206e 756d 6265 7220 666f   phone number fo
-00000800: 726d 6174 2120 2845 7861 6d70 6c65 3a20  rmat! (Example: 
-00000810: 2b34 3478 7878 7878 7878 7878 7829 0a46  +44xxxxxxxxxx).F
-00000820: 7a33 2020 2020 3e20 4d69 7373 696e 6720  z3    > Missing 
-00000830: 436f 756e 7472 7920 436f 6465 2120 2845  Country Code! (E
-00000840: 7861 6d70 6c65 3a20 2b39 312c 202b 3434  xample: +91, +44
-00000850: 2c20 2b31 297a 3420 2020 203e 204d 6973  , +1)z4    > Mis
-00000860: 7369 6e67 2043 6f75 6e74 7279 2043 6f64  sing Country Cod
-00000870: 6521 2028 4578 616d 706c 653a 202b 3931  e! (Example: +91
-00000880: 2c20 2b34 342c 202b 3129 0a7a 0d43 6f75  , +44, +1).z.Cou
-00000890: 6e74 7279 2043 6f64 653a 721e 0000 007a  ntry Code:r....z
-000008a0: 104e 6174 696f 6e61 6c20 4e75 6d62 6572  .National Number
-000008b0: 3a5a 0243 48da 0265 6e5a 0252 4ffa 015b  :Z.CH..enZ.RO..[
-000008c0: fa01 5dfa 0127 fa01 28fa 0129 fa01 2cfa  ..]..'..(..)..,.
-000008d0: 0120 7a04 7465 6c3a e91e 0000 0075 5201  . z.tel:.....uR.
-000008e0: 0000 0a20 2020 20e2 948c e294 80e2 9480  ...    .........
-000008f0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00000900: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00000910: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00000920: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00000930: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00000940: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00000950: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00000070: 6401 6c08 5a08 6400 6401 6c09 5a09 6400  d.l.Z.d.d.l.Z.d.
+00000080: 6401 6c0a 5a0a 6400 6401 6c0b 5a0b 6400  d.l.Z.d.d.l.Z.d.
+00000090: 6402 6c0c 6d0d 5a0d 0100 6400 6401 6c0e  d.l.m.Z...d.d.l.
+000000a0: 5a0e 6400 6401 6c0f 5a10 6700 6403 a201  Z.d.d.l.Z.g.d...
+000000b0: 0400 5a11 5a12 6404 6113 6404 6114 6405  ..Z.Z.d.a.d.a.d.
+000000c0: 6115 6406 6407 8400 5a16 6408 6409 8400  a.d.d...Z.d.d...
+000000d0: 5a17 640a 640b 8400 5a18 640c 640d 8400  Z.d.d...Z.d.d...
+000000e0: 5a19 640e 640f 8400 5a1a 6410 6411 8400  Z.d.d...Z.d.d...
+000000f0: 5a1b 6404 6405 6405 6405 6405 6700 6412  Z.d.d.d.d.d.g.d.
+00000100: a201 6404 6404 6405 6405 6405 660b 6413  ..d.d.d.d.d.f.d.
+00000110: 6414 8401 5a1c 6415 6416 8400 5a1d 6417  d...Z.d.d...Z.d.
+00000120: 6418 8400 5a1e 6419 641a 8400 5a1f 641b  d...Z.d.d...Z.d.
+00000130: 641c 8400 5a20 641d 641e 8400 5a21 641f  d...Z d.d...Z!d.
+00000140: 6420 8400 5a22 6401 5300 2921 e900 0000  d ..Z"d.S.)!....
+00000150: 004e 2901 da09 4d61 634c 6f6f 6b75 7029  .N)...MacLookup)
+00000160: 10da 0663 6861 6e67 65da 0563 6865 636b  ...change..check
+00000170: da05 636c 6561 72da 0464 6f72 6bda 0364  ..clear..dork..d
+00000180: 6e73 da04 6578 6974 da03 6578 70da 0468  ns..exit..exp..h
+00000190: 656c 70da 0469 6e66 6fda 0269 70da 036d  elp..info..ip..m
+000001a0: 6163 da06 6e75 6d62 6572 da04 7175 6974  ac..number..quit
+000001b0: da04 7361 7665 da05 7368 656c 6cda 0577  ..save..shell..w
+000001c0: 686f 6973 da00 4663 0000 0000 0000 0000  hois..Fc........
+000001d0: 0000 0000 0100 0000 0600 0000 4300 0000  ............C...
+000001e0: 7336 0000 0064 0164 0267 027d 007a 1a74  s6...d.d.g.}.z.t
+000001f0: 006a 0174 02a0 037c 00a1 0164 0364 048d  .j.t...|...d.d..
+00000200: 0201 0057 0064 0553 0001 0001 0001 0059  ...W.d.S.......Y
+00000210: 0064 0653 0030 0064 0053 0029 074e 7a12  .d.S.0.d.S.).Nz.
+00000220: 6874 7470 733a 2f2f 676f 6f67 6c65 2e63  https://google.c
+00000230: 6f6d 7a10 6874 7470 733a 2f2f 6269 6e67  omz.https://bing
+00000240: 2e63 6f6d e90a 0000 0029 01da 0774 696d  .com.....)...tim
+00000250: 656f 7574 5446 2904 da08 7265 7175 6573  eoutTF)...reques
+00000260: 7473 da03 6765 74da 0672 616e 646f 6dda  ts..get..random.
+00000270: 0663 686f 6963 6529 01da 0475 726c 73a9  .choice)...urls.
+00000280: 0072 1b00 0000 fa2f 6275 696c 642f 6264  .r...../build/bd
+00000290: 6973 742e 6c69 6e75 782d 7838 365f 3634  ist.linux-x86_64
+000002a0: 2f65 6767 2f70 686f 6d62 6572 2f70 686f  /egg/phomber/pho
+000002b0: 6d62 6572 2e70 79da 1063 6865 636b 5f63  mber.py..check_c
+000002c0: 6f6e 6e65 6374 696f 6e3a 0000 0073 0c00  onnection:...s..
+000002d0: 0000 0002 0801 0201 1401 0601 0601 721d  ..............r.
+000002e0: 0000 0063 0100 0000 0000 0000 0000 0000  ...c............
+000002f0: 1400 0000 1700 0000 4300 0000 736c 0400  ........C...sl..
+00000300: 0064 0164 026c 006d 017d 0101 0064 0164  .d.d.l.m.}...d.d
+00000310: 036c 006d 027d 0201 0064 0164 046c 006d  .l.m.}...d.d.l.m
+00000320: 037d 0301 0064 0561 0474 0564 067c 009b  .}...d.a.t.d.|..
+00000330: 0064 079d 0367 0064 08a2 0164 0964 0a8d  .d...g.d...d.d..
+00000340: 0301 0074 0464 0b7c 009b 0064 0c9d 0364  ...t.d.|...d...d
+00000350: 0d17 0037 0061 0474 06a0 0764 0e7c 00a1  ...7.a.t...d.|..
+00000360: 0273 7674 0564 0f67 0064 10a2 0164 118d  .svt.d.g.d...d..
+00000370: 0201 0064 1253 007a 0e74 00a0 087c 00a1  ...d.S.z.t...|..
+00000380: 017d 0457 006e 2804 0074 006a 096a 0a79  .}.W.n(..t.j.j.y
+00000390: ac01 0001 0001 0074 0564 1367 0064 10a2  .......t.d.g.d..
+000003a0: 0164 118d 0201 0059 0064 1253 0030 0074  .d.....Y.d.S.0.t
+000003b0: 0b7c 0483 01a0 0c64 1464 15a1 0264 1519  .|.....d.d...d..
+000003c0: 00a0 0c64 1664 15a1 0264 0119 00a0 0da1  ...d.d...d......
+000003d0: 007d 0574 0b7c 0483 01a0 0c64 1464 15a1  .}.t.|.....d.d..
+000003e0: 0264 1519 00a0 0c64 1664 15a1 0264 1519  .d.....d.d...d..
+000003f0: 00a0 0da1 007d 0674 00a0 0e7c 04a1 017d  .....}.t...|...}
+00000400: 0774 00a0 0f7c 04a1 017d 087c 0790 0372  .t...|...}.|...r
+00000410: d87c 0890 0372 d874 00a0 087c 0064 17a1  .|...r.t...|.d..
+00000420: 027d 0974 00a0 107c 04a1 017d 0a7c 03a0  .}.t...|...}.|..
+00000430: 117c 0964 18a1 027d 0b74 00a0 087c 0064  .|.d...}.t...|.d
+00000440: 19a1 027d 0c7c 02a0 127c 0c64 18a1 027d  ...}.|...|.d...}
+00000450: 0d74 0b7c 01a0 137c 04a1 0183 017d 0e7c  .t.|...|.....}.|
+00000460: 0ea0 1464 1a64 05a1 02a0 1464 1b64 05a1  ...d.d.....d.d..
+00000470: 02a0 1464 1c64 05a1 02a0 1464 1d64 05a1  ...d.d.....d.d..
+00000480: 02a0 1464 1e64 05a1 02a0 1464 1f64 05a1  ...d.d.....d.d..
+00000490: 02a0 1464 2064 05a1 027d 0f74 00a0 157c  ...d d...}.t...|
+000004a0: 0474 006a 166a 17a1 02a0 1464 2164 05a1  .t.j.j.....d!d..
+000004b0: 027d 1074 0b7c 0883 0164 2074 1864 2274  .}.t.|...d t.d"t
+000004c0: 1974 0b7c 0883 0183 0118 0083 0114 0017  .t.|............
+000004d0: 007d 0874 0b7c 0783 0164 2074 1864 2274  .}.t.|...d t.d"t
+000004e0: 1974 0b7c 0783 0183 0118 0083 0114 0017  .t.|............
+000004f0: 007d 0774 0b7c 0583 0164 2074 1864 2274  .}.t.|...d t.d"t
+00000500: 1974 0b7c 0583 0183 0118 0083 0114 0017  .t.|............
+00000510: 007d 0574 0b7c 0b83 0164 2074 1864 2274  .}.t.|...d t.d"t
+00000520: 1974 0b7c 0b83 0183 0118 0083 0114 0017  .t.|............
+00000530: 007d 0b74 0b7c 0a83 0164 2074 1864 2274  .}.t.|...d t.d"t
+00000540: 1974 0b7c 0a83 0183 0118 0083 0114 0017  .t.|............
+00000550: 007d 0a74 0b7c 0d83 0164 2074 1864 2274  .}.t.|...d t.d"t
+00000560: 1974 0b7c 0d83 0183 0118 0083 0114 0017  .t.|............
+00000570: 007d 0d74 0b7c 0f83 0164 2074 1864 2274  .}.t.|...d t.d"t
+00000580: 1974 0b7c 0f83 0183 0118 0083 0114 0017  .t.|............
+00000590: 007d 0f74 0b7c 0083 0164 2074 1864 2274  .}.t.|...d t.d"t
+000005a0: 1974 0b7c 0083 0183 0118 0083 0114 0017  .t.|............
+000005b0: 007d 0074 0b7c 0683 0164 2074 1864 2274  .}.t.|...d t.d"t
+000005c0: 1974 0b7c 0683 0183 0118 0083 0114 0017  .t.|............
+000005d0: 007d 0674 0b7c 1083 0164 2074 1864 2274  .}.t.|...d t.d"t
+000005e0: 1974 0b7c 1083 0183 0118 0083 0114 0017  .t.|............
+000005f0: 007d 1064 237c 009b 0064 247c 089b 0064  .}.d#|...d$|...d
+00000600: 257c 079b 0064 267c 059b 0064 277c 0b9b  %|...d&|...d'|..
+00000610: 0064 287c 0a9b 0064 297c 0d9b 0064 2a7c  .d(|...d)|...d*|
+00000620: 0f9b 0064 2b7c 009b 0064 2c7c 069b 0064  ...d+|...d,|...d
+00000630: 2d7c 109b 0064 2e9d 177d 1174 1a7c 1183  -|...d...}.t.|..
+00000640: 0101 0074 047c 1164 2f17 0037 0061 0464  ...t.|.d/..7.a.d
+00000650: 307c 00a0 0da1 009b 0064 317c 0aa0 0da1  0|.......d1|....
+00000660: 009b 0064 327c 06a0 0da1 009b 0064 337c  ...d2|.......d3|
+00000670: 0aa0 0da1 00a0 1ba1 009b 0064 327c 06a0  ...........d2|..
+00000680: 0da1 009b 0064 349d 0b7d 1274 1a7c 1283  .....d4..}.t.|..
+00000690: 0101 0074 047c 1264 2f17 0037 0061 0464  ...t.|.d/..7.a.d
+000006a0: 357c 06a0 0da1 009b 0064 349d 037d 1374  5|.......d4..}.t
+000006b0: 1a7c 1383 0101 0074 047c 1364 2f17 0037  .|.....t.|.d/..7
+000006c0: 0061 0474 0564 3667 0064 08a2 0164 0964  .a.t.d6g.d...d.d
+000006d0: 0a8d 0301 0064 0953 0074 0b7c 0883 0164  .....d.S.t.|...d
+000006e0: 2074 1864 2274 1974 0b7c 0883 0183 0118   t.d"t.t.|......
+000006f0: 0083 0114 0017 007d 0874 0b7c 0783 0164  .......}.t.|...d
+00000700: 2074 1864 2274 1974 0b7c 0783 0183 0118   t.d"t.t.|......
+00000710: 0083 0114 0017 007d 0774 0b7c 0083 0164  .......}.t.|...d
+00000720: 2074 1864 2274 1974 0b7c 0083 0183 0118   t.d"t.t.|......
+00000730: 0083 0114 0017 007d 0064 237c 009b 0064  .......}.d#|...d
+00000740: 247c 089b 0064 257c 079b 0064 2e9d 077d  $|...d%|...d...}
+00000750: 1174 1a7c 1183 0101 0074 047c 1164 2f17  .t.|.....t.|.d/.
+00000760: 0037 0061 0464 1253 0064 0053 0029 374e  .7.a.d.S.d.S.)7N
+00000770: 7201 0000 0029 01da 0874 696d 657a 6f6e  r....)...timezon
+00000780: 6529 01da 0763 6172 7269 6572 2901 da08  e)...carrier)...
+00000790: 6765 6f63 6f64 6572 7213 0000 00fa 2f20  geocoderr...../ 
+000007a0: 2020 205b 2b5d 2047 7261 7468 6572 696e     [+] Gratherin
+000007b0: 6720 696e 666f 726d 6174 696f 6e20 6162  g information ab
+000007c0: 6f75 7420 1b5b 313b 3439 3b39 366d fa0d  out .[1;49;96m..
+000007d0: 1b5b 313b 3439 3b39 336d 2e2e 2ea9 03e9  .[1;49;93m......
+000007e0: 0100 0000 e931 0000 00e9 5d00 0000 54a9  .....1....]...T.
+000007f0: 02da 0663 6f6c 6564 74da 0a73 7061 6365  ...coledt..space
+00000800: 5f64 6f77 6e7a 3d0a 2020 2020 1b5b 313b  _downz=.    .[1;
+00000810: 3439 3b39 336d 5b23 5d20 5265 7665 7273  49;93m[#] Revers
+00000820: 6520 7068 6f6e 6520 6e75 6d62 6572 206c  e phone number l
+00000830: 6f6f 6b75 7020 666f 7220 1b5b 313b 3439  ookup for .[1;49
+00000840: 3b39 366d fa0f 1b5b 313b 3439 3b39 336d  ;96m...[1;49;93m
+00000850: 3a1b 5b30 6dfa 020a 0a7a 115e 5c2b 5b31  :.[0m....z.^\+[1
+00000860: 2d39 5d5c 647b 312c 3134 7d24 7a3b 2020  -9]\d{1,14}$z;  
+00000870: 2020 3e20 496e 7661 6c69 6420 7068 6f6e    > Invalid phon
+00000880: 6520 6e75 6d62 6572 2066 6f72 6d61 7421  e number format!
+00000890: 2028 4578 616d 706c 653a 202b 3434 7878   (Example: +44xx
+000008a0: 7878 7878 7878 7878 29a9 0372 2400 0000  xxxxxxxx)..r$...
+000008b0: 7225 0000 00e9 5b00 0000 a901 7228 0000  r%....[.....r(..
+000008c0: 0046 7a33 2020 2020 3e20 4d69 7373 696e  .Fz3    > Missin
+000008d0: 6720 436f 756e 7472 7920 436f 6465 2120  g Country Code! 
+000008e0: 2845 7861 6d70 6c65 3a20 2b39 312c 202b  (Example: +91, +
+000008f0: 3434 2c20 2b31 297a 0d43 6f75 6e74 7279  44, +1)z.Country
+00000900: 2043 6f64 653a 7224 0000 007a 104e 6174   Code:r$...z.Nat
+00000910: 696f 6e61 6c20 4e75 6d62 6572 3a5a 0243  ional Number:Z.C
+00000920: 48da 0265 6e5a 0252 4ffa 015b fa01 5dfa  H..enZ.RO..[..].
+00000930: 0127 fa01 28fa 0129 fa01 2cfa 0120 7a04  .'..(..)..,.. z.
+00000940: 7465 6c3a e91e 0000 0075 d400 0000 0a20  tel:.....u..... 
+00000950: 2020 20e2 948c e294 80e2 9480 e294 80e2     .............
 00000960: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
 00000970: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00000980: e294 80e2 9480 e294 80e2 9480 e294 900a  ................
-00000990: 2020 2020 7c20 494e 464f 524d 4154 494f      | INFORMATIO
-000009a0: 4e20 2020 2020 2020 2020 7c20 4445 5343  N         | DESC
-000009b0: 5249 5054 494f 4e20 2020 2020 2020 2020  RIPTION         
-000009c0: 2020 2020 2020 2020 2020 207c 0a20 2020             |.   
-000009d0: 207c 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   |--------------
-000009e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000009f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000a00: 2d2d 2d2d 2d2d 2d2d 7c0a 2020 2020 7c20  --------|.    | 
-00000a10: 1b5b 313b 3439 3b39 376d 506f 7373 6962  .[1;49;97mPossib
-00000a20: 6c65 1b5b 306d 2020 2020 2020 2020 2020  le.[0m          
-00000a30: 2020 7c20 7a2d 207c 0a20 2020 207c 201b    | z- |.    | .
-00000a40: 5b31 3b34 393b 3937 6d56 616c 6964 1b5b  [1;49;97mValid.[
-00000a50: 306d 2020 2020 2020 2020 2020 2020 2020  0m              
-00000a60: 207c 207a 6a20 7c0a 2020 2020 7c2d 2d2d   | zj |.    |---
-00000a70: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000a80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000a90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000aa0: 2d2d 2d7c 0a20 2020 207c 201b 5b31 3b34  ---|.    | .[1;4
-00000ab0: 393b 3937 6d43 6f75 6e74 7279 2043 6f64  9;97mCountry Cod
-00000ac0: 651b 5b30 6d20 2020 2020 2020 207c 207a  e.[0m        | z
-00000ad0: 2d20 7c0a 2020 2020 7c20 1b5b 313b 3439  - |.    | .[1;49
-00000ae0: 3b39 376d 436f 756e 7472 791b 5b30 6d20  ;97mCountry.[0m 
-00000af0: 2020 2020 2020 2020 2020 2020 7c20 fa2d              | .-
-00000b00: 207c 0a20 2020 207c 201b 5b31 3b34 393b   |.    | .[1;49;
-00000b10: 3937 6d52 6567 696f 6e20 436f 6465 1b5b  97mRegion Code.[
-00000b20: 306d 2020 2020 2020 2020 207c 207a 2d20  0m         | z- 
-00000b30: 7c0a 2020 2020 7c20 1b5b 313b 3439 3b39  |.    | .[1;49;9
-00000b40: 376d 5365 7276 6963 6520 5072 6f76 6964  7mService Provid
-00000b50: 6572 1b5b 306d 2020 2020 7c20 fa2d 207c  er.[0m    | .- |
-00000b60: 0a20 2020 207c 201b 5b31 3b34 393b 3937  .    | .[1;49;97
-00000b70: 6d54 696d 657a 6f6e 651b 5b30 6d20 2020  mTimezone.[0m   
-00000b80: 2020 2020 2020 2020 207c 207a 6a20 7c0a           | zj |.
-00000b90: 2020 2020 7c2d 2d2d 2d2d 2d2d 2d2d 2d2d      |-----------
-00000ba0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000bb0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000bc0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d7c 0a20 2020  -----------|.   
-00000bd0: 207c 201b 5b31 3b34 393b 3937 6d49 6e74   | .[1;49;97mInt
-00000be0: 6572 6e61 7469 6f6e 616c 2046 6f72 6d61  ernational Forma
-00000bf0: 741b 5b30 6d7c 207a 2d20 7c0a 2020 2020  t.[0m| z- |.    
-00000c00: 7c20 1b5b 313b 3439 3b39 376d 4e61 7469  | .[1;49;97mNati
-00000c10: 6f6e 616c 2046 6f72 6d61 741b 5b30 6d20  onal Format.[0m 
-00000c20: 2020 2020 7c20 7a2d 207c 0a20 2020 207c      | z- |.    |
-00000c30: 201b 5b31 3b34 393b 3937 6d52 4643 3339   .[1;49;97mRFC39
-00000c40: 3636 2046 6f72 6d61 741b 5b30 6d20 2020  66 Format.[0m   
-00000c50: 2020 207c 2075 b800 0000 207c 0a20 2020     | u.... |.   
-00000c60: 20e2 9494 e294 80e2 9480 e294 80e2 9480   ...............
-00000c70: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00000c80: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00000c90: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00000ca0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00000cb0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00000cc0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00000cd0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00000ce0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00000cf0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00000d00: e294 80e2 9480 e294 980a 2020 2020 2020  ..........      
-00000d10: 2020 7a2b 0a20 2020 201b 5b31 3b34 393b    z+.    .[1;49;
-00000d20: 3933 6d5b 2b5d 2053 6561 7263 6869 6e67  93m[+] Searching
-00000d30: 2066 6f72 201b 5b31 3b34 393b 3936 6d7a   for .[1;49;96mz
-00000d40: 741b 5b31 3b34 393b 3933 6d20 6f6e 2076  t.[1;49;93m on v
-00000d50: 6172 696f 7573 2070 6c61 7466 6f72 6d73  arious platforms
-00000d60: 3a0a 0a20 2020 201b 5b31 3b34 393b 3932  :..    .[1;49;92
-00000d70: 6d3e 2068 7474 7073 3a2f 2f77 7777 2e69  m> https://www.i
-00000d80: 7071 7561 6c69 7479 7363 6f72 652e 636f  pqualityscore.co
-00000d90: 6d2f 7265 7665 7273 652d 7068 6f6e 652d  m/reverse-phone-
-00000da0: 6e75 6d62 6572 2d6c 6f6f 6b75 702f 6c6f  number-lookup/lo
-00000db0: 6f6b 7570 2ffa 012f 7a29 0a20 2020 203e  okup/../z).    >
-00000dc0: 2068 7474 7073 3a2f 2f77 7777 2e74 7275   https://www.tru
-00000dd0: 6563 616c 6c65 722e 636f 6d2f 7365 6172  ecaller.com/sear
-00000de0: 6368 2f7a 090a 2020 2020 1b5b 306d 7a59  ch/z..    .[0mzY
-00000df0: 0a20 2020 201b 5b31 3b34 393b 3933 6d5b  .    .[1;49;93m[
-00000e00: 2b5d 2047 6f6f 676c 6520 446f 726b 2051  +] Google Dork Q
-00000e10: 7565 7269 6573 3a0a 0a20 2020 201b 5b31  ueries:..    .[1
-00000e20: 3b34 393b 3932 6d3e 2068 7474 7073 3a2f  ;49;92m> https:/
-00000e30: 2f77 7777 2e67 6f6f 676c 652e 636f 6d2f  /www.google.com/
-00000e40: 7365 6172 6368 3f71 3d29 1cda 0c70 686f  search?q=)...pho
-00000e50: 6e65 6e75 6d62 6572 7372 1800 0000 7219  nenumbersr....r.
-00000e60: 0000 0072 1a00 0000 da06 7072 765f 6f70  ...r......prv_op
-00000e70: da07 7072 696e 7469 74da 0272 65da 056d  ..printit..re..m
-00000e80: 6174 6368 da05 7061 7273 655a 0f70 686f  atch..parseZ.pho
-00000e90: 6e65 6e75 6d62 6572 7574 696c 5a14 4e75  nenumberutilZ.Nu
-00000ea0: 6d62 6572 5061 7273 6545 7863 6570 7469  mberParseExcepti
-00000eb0: 6f6e da03 7374 72da 0573 706c 6974 da05  on..str..split..
-00000ec0: 7374 7269 705a 0f69 735f 7661 6c69 645f  stripZ.is_valid_
-00000ed0: 6e75 6d62 6572 5a12 6973 5f70 6f73 7369  numberZ.is_possi
-00000ee0: 626c 655f 6e75 6d62 6572 5a16 7265 6769  ble_numberZ.regi
-00000ef0: 6f6e 5f63 6f64 655f 666f 725f 6e75 6d62  on_code_for_numb
-00000f00: 6572 5a16 6465 7363 7269 7074 696f 6e5f  erZ.description_
-00000f10: 666f 725f 6e75 6d62 6572 5a0f 6e61 6d65  for_numberZ.name
-00000f20: 5f66 6f72 5f6e 756d 6265 725a 1574 696d  _for_numberZ.tim
-00000f30: 655f 7a6f 6e65 735f 666f 725f 6e75 6d62  e_zones_for_numb
-00000f40: 6572 da07 7265 706c 6163 655a 0d66 6f72  er..replaceZ.for
-00000f50: 6d61 745f 6e75 6d62 6572 5a11 5068 6f6e  mat_numberZ.Phon
-00000f60: 654e 756d 6265 7246 6f72 6d61 745a 0752  eNumberFormatZ.R
-00000f70: 4643 3339 3636 da03 696e 74da 036c 656e  FC3966..int..len
-00000f80: da05 7072 696e 74da 056c 6f77 6572 2914  ..print..lower).
-00000f90: 5a0c 7068 6f6e 655f 6e75 6d62 6572 7218  Z.phone_numberr.
-00000fa0: 0000 0072 1900 0000 721a 0000 005a 1470  ...r....r....Z.p
-00000fb0: 686f 6e65 5f6e 756d 6265 725f 6465 7461  hone_number_deta
-00000fc0: 696c 73da 0c63 6f75 6e74 7279 5f63 6f64  ils..country_cod
-00000fd0: 655a 0b6f 6e6c 795f 6e75 6d62 6572 5a05  eZ.only_numberZ.
-00000fe0: 7661 6c69 64da 0870 6f73 7369 626c 655a  valid..possibleZ
-00000ff0: 0e63 6f75 6e72 7479 5f6e 756d 6265 72da  .counrty_number.
-00001000: 0b72 6567 696f 6e5f 636f 6465 da07 636f  .region_code..co
-00001010: 756e 7472 795a 0e73 6572 7669 6365 5f6e  untryZ.service_n
-00001020: 756d 6265 725a 1073 6572 7669 6365 5f70  umberZ.service_p
-00001030: 726f 7669 6465 725a 1b74 696d 657a 6f6e  roviderZ.timezon
-00001040: 655f 6465 7461 696c 735f 756e 6669 6c74  e_details_unfilt
-00001050: 6572 6564 5a10 7469 6d65 7a6f 6e65 5f64  eredZ.timezone_d
-00001060: 6574 6169 6c73 5a08 725f 666f 726d 6174  etailsZ.r_format
-00001070: da0c 6669 6e61 6c5f 6f75 7470 7574 5a12  ..final_outputZ.
-00001080: 6f6e 6c69 6e65 5f66 7265 655f 6c6f 6f6b  online_free_look
-00001090: 7570 5a13 676f 6f67 6c65 5f64 6f72 6b5f  upZ.google_dork_
-000010a0: 7175 6572 6965 7372 1500 0000 7215 0000  queriesr....r...
-000010b0: 0072 1600 0000 da0d 6e75 6d62 6572 5f6c  .r......number_l
-000010c0: 6f6f 6b75 703c 0000 0073 b600 0000 0002  ookup<...s......
-000010d0: 0c01 0c01 0c04 0403 1a01 1403 0c01 1001  ................
-000010e0: 0801 0403 0202 0e01 1001 1001 0801 0803  ................
-000010f0: 2401 2403 0a03 0a02 0c02 0c03 0a03 0c03  $.$.............
-00001100: 0c03 0c03 0e01 3c03 1803 2001 2001 2001  ......<... . . .
-00001110: 2001 2001 2001 2001 2001 2001 2003 0204   . . . . . . ...
-00001120: 02fc 0405 02fb 0407 02f9 0408 02f8 0409  ................
-00001130: 02f7 040a 02f6 040b 02f5 040d 02f3 040e  ................
-00001140: 02f2 040f 02f1 0812 0801 0c03 0201 06ff  ................
-00001150: 0403 06fd 0403 06fd 0404 0afc 0403 06fd  ................
-00001160: 0806 0801 0c03 0203 06fd 0805 0801 0c02  ................
-00001170: 0404 2001 2002 0204 02fc 0405 02fb 0808  .. . ...........
-00001180: 0801 0c01 7248 0000 0063 0100 0000 0000  ....rH...c......
-00001190: 0000 0000 0000 3600 0000 3700 0000 4300  ......6...7...C.
-000011a0: 0000 7328 0f00 0064 0161 0074 0164 0267  ..s(...d.a.t.d.g
-000011b0: 0064 03a2 0164 0464 058d 0301 0074 0264  .d...d.d.....t.d
-000011c0: 0683 0173 3c74 0164 0767 0064 08a2 0164  ...s<t.d.g.d...d
-000011d0: 0464 058d 0301 0074 0064 0937 0061 0064  .d.....t.d.7.a.d
-000011e0: 0a53 0074 0164 0b7c 009b 0064 0c9d 0367  .S.t.d.|...d...g
-000011f0: 0064 03a2 0164 0464 058d 0301 0074 0064  .d...d.d.....t.d
-00001200: 0d7c 009b 0064 0e9d 0364 0f17 0037 0061  .|...d...d...7.a
-00001210: 0074 03a0 0464 107c 00a1 0273 9274 0164  .t...d.|...s.t.d
-00001220: 1167 0064 08a2 0164 128d 0201 0074 0064  .g.d...d.....t.d
-00001230: 1337 0061 0064 0053 0064 147c 009b 009d  .7.a.d.S.d.|....
-00001240: 0264 157c 009b 0064 169d 0364 177c 009b  .d.|...d...d.|..
-00001250: 009d 0267 037d 0174 057c 0083 0164 1874  ...g.}.t.|...d.t
-00001260: 0664 1974 0774 057c 0083 0183 0118 0083  .d.t.t.|........
-00001270: 0114 0017 007d 0064 1a64 1b69 017d 0274  .....}.d.d.i.}.t
-00001280: 08a0 0967 0064 1ca2 01a1 017d 037c 0364  ...g.d.....}.|.d
-00001290: 1d6b 0290 0372 cc90 027a 8674 0a6a 0b7c  .k...r...z.t.j.|
-000012a0: 0164 1d19 0064 1e7c 0264 1f8d 037d 047c  .d...d.|.d...}.|
-000012b0: 04a0 0ca1 007d 057c 046a 0d64 206b 0290  .....}.|.j.d k..
-000012c0: 0172 8c7c 0564 2119 0064 226b 0290 0172  .r.|.d!..d"k...r
-000012d0: 8c7c 0564 2319 007d 067c 0564 2419 007d  .|.d#..}.|.d$..}
-000012e0: 077c 0564 2519 007d 087c 0564 2619 007d  .|.d%..}.|.d&..}
-000012f0: 097c 0564 2719 007d 0a7c 0564 2819 007d  .|.d'..}.|.d(..}
-00001300: 0b7c 0564 2919 007d 0c7c 0564 2a19 007d  .|.d)..}.|.d*..}
-00001310: 0d7c 0564 2b19 007d 0e7c 0564 2c19 007d  .|.d+..}.|.d,..}
-00001320: 0f7c 0564 2d19 007d 107c 0564 2e19 007d  .|.d-..}.|.d...}
-00001330: 116e 0874 0e64 2f83 0182 0174 057c 0683  .n.t.d/....t.|..
-00001340: 0164 1874 0664 1974 0774 057c 0683 0183  .d.t.d.t.t.|....
-00001350: 0118 0083 0114 0017 007d 0674 057c 0783  .........}.t.|..
-00001360: 0164 1874 0664 1974 0774 057c 0783 0183  .d.t.d.t.t.|....
-00001370: 0118 0083 0114 0017 007d 0774 057c 0883  .........}.t.|..
-00001380: 0164 1874 0664 1974 0774 057c 0883 0183  .d.t.d.t.t.|....
-00001390: 0118 0083 0114 0017 007d 0874 057c 0983  .........}.t.|..
-000013a0: 0164 1874 0664 1974 0774 057c 0983 0183  .d.t.d.t.t.|....
-000013b0: 0118 0083 0114 0017 007d 0974 057c 0a83  .........}.t.|..
-000013c0: 0164 1874 0664 1974 0774 057c 0a83 0183  .d.t.d.t.t.|....
-000013d0: 0118 0083 0114 0017 007d 0a74 057c 0b83  .........}.t.|..
-000013e0: 0164 1874 0664 1974 0774 057c 0b83 0183  .d.t.d.t.t.|....
-000013f0: 0118 0083 0114 0017 007d 0b74 057c 0c83  .........}.t.|..
-00001400: 0164 1874 0664 1974 0774 057c 0c83 0183  .d.t.d.t.t.|....
-00001410: 0118 0083 0114 0017 007d 0c74 057c 0d83  .........}.t.|..
-00001420: 0164 1874 0664 1974 0774 057c 0d83 0183  .d.t.d.t.t.|....
-00001430: 0118 0083 0114 0017 007d 0d74 057c 0e83  .........}.t.|..
-00001440: 0164 1874 0664 1974 0774 057c 0e83 0183  .d.t.d.t.t.|....
-00001450: 0118 0083 0114 0017 007d 0e74 057c 0f83  .........}.t.|..
-00001460: 0164 1874 0664 1974 0774 057c 0f83 0183  .d.t.d.t.t.|....
-00001470: 0118 0083 0114 0017 007d 0f74 057c 1083  .........}.t.|..
-00001480: 0164 1874 0664 1974 0774 057c 1083 0183  .d.t.d.t.t.|....
-00001490: 0118 0083 0114 0017 007d 1074 057c 1183  .........}.t.|..
-000014a0: 0164 1874 0664 1974 0774 057c 1183 0183  .d.t.d.t.t.|....
-000014b0: 0118 0083 0114 0017 007d 1164 307c 009b  .........}.d0|..
-000014c0: 0064 317c 069b 0064 327c 079b 0064 337c  .d1|...d2|...d3|
-000014d0: 089b 0064 347c 099b 0064 357c 0a9b 0064  ...d4|...d5|...d
-000014e0: 367c 0e9b 0064 377c 0d9b 0064 387c 0f9b  6|...d7|...d8|..
-000014f0: 0064 397c 109b 0064 3a7c 0b9b 0064 3b7c  .d9|...d:|...d;|
-00001500: 0c9b 0064 3c9d 197d 1274 0f7c 1283 0101  ...d<..}.t.|....
-00001510: 0074 007c 1264 0f17 0037 0061 0057 006e  .t.|.d...7.a.W.n
-00001520: 4e04 0074 0e90 0379 c601 007d 1301 007a  N..t...y...}...z
-00001530: 3474 0f7c 1383 0101 0064 307c 009b 0064  4t.|.....d0|...d
-00001540: 3d9d 037d 1274 0f7c 1283 0101 0074 007c  =..}.t.|.....t.|
-00001550: 1264 0f17 0037 0061 0057 0059 0064 007d  .d...7.a.W.Y.d.}
-00001560: 137e 136e 0a64 007d 137e 1330 0030 0090  .~.n.d.}.~.0.0..
-00001570: 0b6e 587c 0364 3e6b 0290 0972 3490 057a  .nX|.d>k...r4..z
-00001580: 2a74 0a6a 0b7c 0164 3e19 0064 1e7c 0264  *t.j.|.d>..d.|.d
-00001590: 1f8d 037d 047c 04a0 0ca1 007d 057c 046a  ...}.|.....}.|.j
-000015a0: 0d64 206b 0290 0472 dc7c 0564 3f19 007d  .d k...r.|.d?..}
-000015b0: 117c 0564 4019 007d 147c 0564 4119 007d  .|.d@..}.|.dA..}
-000015c0: 157c 0564 2719 007d 0a7c 0564 2619 007d  .|.d'..}.|.d&..}
-000015d0: 087c 0564 4219 007d 167c 0564 4319 007d  .|.dB..}.|.dC..}
-000015e0: 067c 0564 4319 007d 177c 0564 4419 007d  .|.dC..}.|.dD..}
-000015f0: 187c 0564 4519 007d 197c 0564 4619 007d  .|.dE..}.|.dF..}
-00001600: 1a7c 0564 4719 007d 1b7c 0564 4819 007d  .|.dG..}.|.dH..}
-00001610: 1c7c 0564 4919 007d 1d7c 0564 4a19 007d  .|.dI..}.|.dJ..}
-00001620: 0e7c 0564 4b19 007d 0f7c 0564 4c19 007d  .|.dK..}.|.dL..}
-00001630: 107c 0564 2a19 007d 0d7c 0564 4d19 007d  .|.d*..}.|.dM..}
-00001640: 1e7c 0564 4e19 007d 1f7c 0564 4f19 007d  .|.dN..}.|.dO..}
-00001650: 207c 0564 5019 007d 217c 0564 5119 007d   |.dP..}!|.dQ..}
-00001660: 227c 0564 5219 007d 237c 0564 5319 007d  "|.dR..}#|.dS..}
-00001670: 247c 0564 5419 007d 257c 0564 2919 007d  $|.dT..}%|.d)..}
-00001680: 0c6e 0874 0e64 5583 0182 0174 057c 1183  .n.t.dU....t.|..
-00001690: 0164 1874 0664 1974 0774 057c 1183 0183  .d.t.d.t.t.|....
-000016a0: 0118 0083 0114 0017 007d 1174 057c 1483  .........}.t.|..
-000016b0: 0164 1874 0664 1974 0774 057c 1483 0183  .d.t.d.t.t.|....
-000016c0: 0118 0083 0114 0017 007d 1474 057c 1583  .........}.t.|..
-000016d0: 0164 1874 0664 1974 0774 057c 1583 0183  .d.t.d.t.t.|....
-000016e0: 0118 0083 0114 0017 007d 1574 057c 0a83  .........}.t.|..
-000016f0: 0164 1874 0664 1974 0774 057c 0a83 0183  .d.t.d.t.t.|....
-00001700: 0118 0083 0114 0017 007d 0a74 057c 0883  .........}.t.|..
-00001710: 0164 1874 0664 1974 0774 057c 0883 0183  .d.t.d.t.t.|....
-00001720: 0118 0083 0114 0017 007d 0874 057c 1683  .........}.t.|..
-00001730: 0164 1874 0664 1974 0774 057c 1683 0183  .d.t.d.t.t.|....
-00001740: 0118 0083 0114 0017 007d 1674 057c 0683  .........}.t.|..
-00001750: 0164 1874 0664 1974 0774 057c 0683 0183  .d.t.d.t.t.|....
-00001760: 0118 0083 0114 0017 007d 0674 057c 1783  .........}.t.|..
-00001770: 0164 1874 0664 1974 0774 057c 1783 0183  .d.t.d.t.t.|....
-00001780: 0118 0083 0114 0017 007d 1774 057c 1883  .........}.t.|..
-00001790: 0164 1874 0664 1974 0774 057c 1883 0183  .d.t.d.t.t.|....
-000017a0: 0118 0083 0114 0017 007d 1874 057c 1983  .........}.t.|..
-000017b0: 0164 1874 0664 1974 0774 057c 1983 0183  .d.t.d.t.t.|....
-000017c0: 0118 0083 0114 0017 007d 1974 057c 1a83  .........}.t.|..
-000017d0: 0164 1874 0664 1974 0774 057c 1a83 0183  .d.t.d.t.t.|....
-000017e0: 0118 0083 0114 0017 007d 1a74 057c 1b83  .........}.t.|..
-000017f0: 0164 1874 0664 1974 0774 057c 1b83 0183  .d.t.d.t.t.|....
-00001800: 0118 0083 0114 0017 007d 1b74 057c 1c83  .........}.t.|..
-00001810: 0164 1874 0664 1974 0774 057c 1c83 0183  .d.t.d.t.t.|....
-00001820: 0118 0083 0114 0017 007d 1c74 057c 1d83  .........}.t.|..
-00001830: 0164 1874 0664 1974 0774 057c 1d83 0183  .d.t.d.t.t.|....
-00001840: 0118 0083 0114 0017 007d 1d74 057c 0e83  .........}.t.|..
-00001850: 0164 1874 0664 1974 0774 057c 0e83 0183  .d.t.d.t.t.|....
-00001860: 0118 0083 0114 0017 007d 0e74 057c 0f83  .........}.t.|..
-00001870: 0164 1874 0664 1974 0774 057c 0f83 0183  .d.t.d.t.t.|....
-00001880: 0118 0083 0114 0017 007d 0f74 057c 1083  .........}.t.|..
-00001890: 0164 1874 0664 1974 0774 057c 1083 0183  .d.t.d.t.t.|....
-000018a0: 0118 0083 0114 0017 007d 1074 057c 0d83  .........}.t.|..
-000018b0: 0164 1874 0664 1974 0774 057c 0d83 0183  .d.t.d.t.t.|....
-000018c0: 0118 0083 0114 0017 007d 0d74 057c 1e83  .........}.t.|..
-000018d0: 0164 1874 0664 1974 0774 057c 1e83 0183  .d.t.d.t.t.|....
-000018e0: 0118 0083 0114 0017 007d 1e74 057c 1f83  .........}.t.|..
-000018f0: 0164 1874 0664 1974 0774 057c 1f83 0183  .d.t.d.t.t.|....
-00001900: 0118 0083 0114 0017 007d 1f74 057c 2083  .........}.t.| .
-00001910: 0164 1874 0664 1974 0774 057c 2083 0183  .d.t.d.t.t.| ...
-00001920: 0118 0083 0114 0017 007d 2074 057c 2183  .........} t.|!.
-00001930: 0164 1874 0664 1974 0774 057c 2183 0183  .d.t.d.t.t.|!...
-00001940: 0118 0083 0114 0017 007d 2174 057c 2283  .........}!t.|".
-00001950: 0164 1874 0664 1974 0774 057c 2283 0183  .d.t.d.t.t.|"...
-00001960: 0118 0083 0114 0017 007d 2274 057c 2383  .........}"t.|#.
-00001970: 0164 1874 0664 1974 0774 057c 2383 0183  .d.t.d.t.t.|#...
-00001980: 0118 0083 0114 0017 007d 2374 057c 2483  .........}#t.|$.
-00001990: 0164 1874 0664 1974 0774 057c 2483 0183  .d.t.d.t.t.|$...
-000019a0: 0118 0083 0114 0017 007d 2474 057c 2583  .........}$t.|%.
-000019b0: 0164 1874 0664 1974 0774 057c 2583 0183  .d.t.d.t.t.|%...
-000019c0: 0118 0083 0114 0017 007d 2574 057c 0c83  .........}%t.|..
-000019d0: 0164 1874 0664 1974 0774 057c 0c83 0183  .d.t.d.t.t.|....
-000019e0: 0118 0083 0114 0017 007d 0c64 307c 009b  .........}.d0|..
-000019f0: 0064 567c 159b 0064 577c 149b 0064 587c  .dV|...dW|...dX|
-00001a00: 069b 0064 597c 179b 0064 327c 189b 0064  ...dY|...d2|...d
-00001a10: 5a7c 199b 0064 5b7c 1a9b 0064 337c 089b  Z|...d[|...d3|..
-00001a20: 0064 347c 169b 0064 357c 0a9b 0064 5c7c  .d4|...d5|...d\|
-00001a30: 1b9b 0064 5d7c 1f9b 0064 5e7c 1c9b 0064  ...d]|...d^|...d
-00001a40: 5f7c 1d9b 0064 607c 239b 0064 617c 249b  _|...d`|#..da|$.
-00001a50: 0064 627c 229b 0064 637c 209b 0064 647c  .db|"..dc| ..dd|
-00001a60: 219b 0064 367c 0e9b 0064 387c 0f9b 0064  !..d6|...d8|...d
-00001a70: 397c 109b 0064 377c 0d9b 0064 657c 1e9b  9|...d7|...de|..
-00001a80: 0064 667c 259b 0064 677c 0c9b 0064 3c9d  .df|%..dg|...d<.
-00001a90: 377d 1274 0f7c 1283 0101 0074 007c 1264  7}.t.|.....t.|.d
-00001aa0: 0f17 0037 0061 0057 006e 2c01 0001 0001  ...7.a.W.n,.....
-00001ab0: 0064 307c 009b 0064 689d 037d 1274 0f7c  .d0|...dh..}.t.|
-00001ac0: 1283 0101 0074 007c 1264 0f17 0037 0061  .....t.|.d...7.a
-00001ad0: 0059 006e 0230 0090 056e f07c 0364 696b  .Y.n.0...n.|.dik
-00001ae0: 0290 0f72 2490 057a b674 0a6a 0b7c 0164  ...r$..z.t.j.|.d
-00001af0: 6919 0064 1e7c 0264 1f8d 037d 047c 04a0  i..d.|.d...}.|..
-00001b00: 0ca1 007d 057c 046a 0d64 206b 0290 0a72  ...}.|.j.d k...r
-00001b10: 967c 0564 2219 0064 046b 0290 0a72 967c  .|.d"..d.k...r.|
-00001b20: 0564 3f19 007d 117c 0564 6a19 007d 267c  .d?..}.|.dj..}&|
-00001b30: 0564 6b19 007d 277c 0564 4819 007d 1c7c  .dk..}'|.dH..}.|
-00001b40: 0564 2319 007d 067c 0564 4419 007d 187c  .d#..}.|.dD..}.|
-00001b50: 0564 2619 007d 087c 0564 4219 007d 167c  .d&..}.|.dB..}.|
-00001b60: 0564 2719 007d 0a7c 0564 4b19 007d 0f7c  .d'..}.|.dK..}.|
-00001b70: 0564 4c19 007d 107c 0564 6c19 007d 287c  .dL..}.|.dl..}(|
-00001b80: 0564 4a19 007d 0e7c 0564 6d19 007d 297c  .dJ..}.|.dm..})|
-00001b90: 0564 6e19 007d 2a7c 0564 6f19 007d 2b7c  .dn..}*|.do..}+|
-00001ba0: 0564 7019 0064 7119 007d 2c7c 0564 7019  .dp..dq..},|.dp.
-00001bb0: 0064 7219 007d 2d7c 0564 7019 0064 7319  .dr..}-|.dp..ds.
-00001bc0: 007d 2e7c 0564 7419 0064 5419 007d 257c  .}.|.dt..dT..}%|
-00001bd0: 0564 7419 0064 2919 007d 0c7c 0564 7419  .dt..d)..}.|.dt.
-00001be0: 0064 2819 007d 0b7c 0564 7419 0064 7519  .d(..}.|.dt..du.
-00001bf0: 007d 2f7c 0564 2a19 0064 7619 007d 307c  .}/|.d*..dv..}0|
-00001c00: 0564 2a19 0064 7719 007d 317c 0564 2a19  .d*..dw..}1|.d*.
-00001c10: 0064 7819 007d 327c 0564 2a19 0064 7919  .dx..}2|.d*..dy.
-00001c20: 007d 337c 0564 2a19 0064 7a19 007d 347c  .}3|.d*..dz..}4|
-00001c30: 0564 2a19 0064 7b19 007d 356e 0874 0e64  .d*..d{..}5n.t.d
-00001c40: 7c83 0182 0174 057c 1183 0164 1874 0664  |....t.|...d.t.d
-00001c50: 1974 0774 057c 1183 0183 0118 0083 0114  .t.t.|..........
-00001c60: 0017 007d 1174 057c 2683 0164 1874 0664  ...}.t.|&..d.t.d
-00001c70: 1974 0774 057c 2683 0183 0118 0083 0114  .t.t.|&.........
-00001c80: 0017 007d 2674 057c 2783 0164 1874 0664  ...}&t.|'..d.t.d
-00001c90: 1974 0774 057c 2783 0183 0118 0083 0114  .t.t.|'.........
-00001ca0: 0017 007d 2774 057c 1c83 0164 1874 0664  ...}'t.|...d.t.d
-00001cb0: 1974 0774 057c 1c83 0183 0118 0083 0114  .t.t.|..........
-00001cc0: 0017 007d 1c74 057c 0683 0164 1874 0664  ...}.t.|...d.t.d
-00001cd0: 1974 0774 057c 0683 0183 0118 0083 0114  .t.t.|..........
-00001ce0: 0017 007d 0674 057c 1883 0164 1874 0664  ...}.t.|...d.t.d
-00001cf0: 1974 0774 057c 1883 0183 0118 0083 0114  .t.t.|..........
-00001d00: 0017 007d 1874 057c 0883 0164 1874 0664  ...}.t.|...d.t.d
-00001d10: 1974 0774 057c 0883 0183 0118 0083 0114  .t.t.|..........
-00001d20: 0017 007d 0874 057c 1683 0164 1874 0664  ...}.t.|...d.t.d
-00001d30: 1974 0774 057c 1683 0183 0118 0083 0114  .t.t.|..........
-00001d40: 0017 007d 1674 057c 0a83 0164 1874 0664  ...}.t.|...d.t.d
-00001d50: 1974 0774 057c 0a83 0183 0118 0083 0114  .t.t.|..........
-00001d60: 0017 007d 0a74 057c 0f83 0164 1874 0664  ...}.t.|...d.t.d
-00001d70: 1974 0774 057c 0f83 0183 0118 0083 0114  .t.t.|..........
-00001d80: 0017 007d 0f74 057c 1083 0164 1874 0664  ...}.t.|...d.t.d
-00001d90: 1974 0774 057c 1083 0183 0118 0083 0114  .t.t.|..........
-00001da0: 0017 007d 1074 057c 2883 0164 1874 0664  ...}.t.|(..d.t.d
-00001db0: 1974 0774 057c 2883 0183 0118 0083 0114  .t.t.|(.........
-00001dc0: 0017 007d 2874 057c 0e83 0164 1874 0664  ...}(t.|...d.t.d
-00001dd0: 1974 0774 057c 0e83 0183 0118 0083 0114  .t.t.|..........
-00001de0: 0017 007d 0e74 057c 2983 0164 1874 0664  ...}.t.|)..d.t.d
-00001df0: 1974 0774 057c 2983 0183 0118 0083 0114  .t.t.|).........
-00001e00: 0017 007d 2974 057c 2a83 0164 1874 0664  ...})t.|*..d.t.d
-00001e10: 1974 0774 057c 2a83 0183 0118 0083 0114  .t.t.|*.........
-00001e20: 0017 007d 2a74 057c 2b83 0164 1874 0664  ...}*t.|+..d.t.d
-00001e30: 1974 0774 057c 2b83 0183 0118 0083 0114  .t.t.|+.........
-00001e40: 0017 007d 2b74 057c 2c83 0164 1874 0664  ...}+t.|,..d.t.d
-00001e50: 1974 0774 057c 2c83 0183 0118 0083 0114  .t.t.|,.........
-00001e60: 0017 007d 2c74 057c 2d83 0164 1874 0664  ...},t.|-..d.t.d
-00001e70: 1974 0774 057c 2d83 0183 0118 0083 0114  .t.t.|-.........
-00001e80: 0017 007d 2d74 057c 2e83 0164 1874 0664  ...}-t.|...d.t.d
-00001e90: 1974 0774 057c 2e83 0183 0118 0083 0114  .t.t.|..........
-00001ea0: 0017 007d 2e74 057c 2583 0164 1874 0664  ...}.t.|%..d.t.d
-00001eb0: 1974 0774 057c 2583 0183 0118 0083 0114  .t.t.|%.........
-00001ec0: 0017 007d 2574 057c 0c83 0164 1874 0664  ...}%t.|...d.t.d
-00001ed0: 1974 0774 057c 0c83 0183 0118 0083 0114  .t.t.|..........
-00001ee0: 0017 007d 0c74 057c 0b83 0164 1874 0664  ...}.t.|...d.t.d
-00001ef0: 1974 0774 057c 0b83 0183 0118 0083 0114  .t.t.|..........
-00001f00: 0017 007d 0b74 057c 2f83 0164 1874 0664  ...}.t.|/..d.t.d
-00001f10: 1974 0774 057c 2f83 0183 0118 0083 0114  .t.t.|/.........
-00001f20: 0017 007d 2f74 057c 3083 0164 1874 0664  ...}/t.|0..d.t.d
-00001f30: 1974 0774 057c 3083 0183 0118 0083 0114  .t.t.|0.........
-00001f40: 0017 007d 3074 057c 3183 0164 1874 0664  ...}0t.|1..d.t.d
-00001f50: 1974 0774 057c 3183 0183 0118 0083 0114  .t.t.|1.........
-00001f60: 0017 007d 3174 057c 3283 0164 1874 0664  ...}1t.|2..d.t.d
-00001f70: 1974 0774 057c 3283 0183 0118 0083 0114  .t.t.|2.........
-00001f80: 0017 007d 3274 057c 3383 0164 1874 0664  ...}2t.|3..d.t.d
-00001f90: 1974 0774 057c 3383 0183 0118 0083 0114  .t.t.|3.........
-00001fa0: 0017 007d 3374 057c 3483 0164 1874 0664  ...}3t.|4..d.t.d
-00001fb0: 1974 0774 057c 3483 0183 0118 0083 0114  .t.t.|4.........
-00001fc0: 0017 007d 3474 057c 3583 0164 1874 0664  ...}4t.|5..d.t.d
-00001fd0: 1974 0774 057c 3583 0183 0118 0083 0114  .t.t.|5.........
-00001fe0: 0017 007d 3564 307c 009b 0064 7d7c 269b  ...}5d0|...d}|&.
-00001ff0: 0064 587c 069b 0064 327c 189b 0064 337c  .dX|...d2|...d3|
-00002000: 089b 0064 347c 169b 0064 357c 0a9b 0064  ...d4|...d5|...d
-00002010: 7e7c 2a9b 0064 7f7c 279b 0064 5e7c 1c9b  ~|*..d.|'..d^|..
-00002020: 0064 5f7c 289b 0064 807c 2b9b 0064 817c  .d_|(..d.|+..d.|
-00002030: 2e9b 0064 367c 0e9b 0064 5d7c 299b 0064  ...d6|...d]|)..d
-00002040: 387c 0f9b 0064 397c 109b 0064 827c 309b  8|...d9|...d.|0.
-00002050: 0064 837c 319b 0064 847c 329b 0064 857c  .d.|1..d.|2..d.|
-00002060: 339b 0064 867c 349b 0064 877c 359b 0064  3..d.|4..d.|5..d
-00002070: 667c 259b 0064 677c 0b9b 0064 887c 2f9b  f|%..dg|...d.|/.
-00002080: 0064 3c9d 357d 1274 0f7c 1283 0101 0074  .d<.5}.t.|.....t
-00002090: 007c 1264 0f17 0037 0061 0057 006e 2c01  .|.d...7.a.W.n,.
-000020a0: 0001 0001 0064 307c 009b 0064 899d 037d  .....d0|...d...}
-000020b0: 1274 0f7c 1283 0101 0074 007c 1264 0f17  .t.|.....t.|.d..
-000020c0: 0037 0061 0059 006e 0230 0064 0453 0029  .7.a.Y.n.0.d.S.)
-000020d0: 8a4e 720f 0000 007a 2820 2020 205b 2b5d  .Nr....z(    [+]
-000020e0: 2056 6572 6966 7969 6e67 2069 6e74 6572   Verifying inter
-000020f0: 6e65 7420 636f 6e6e 6563 7469 6f6e 2e2e  net connection..
-00002100: 2e72 1d00 0000 5472 2100 0000 7a16 6874  .r....Tr!...z.ht
-00002110: 7470 733a 2f2f 7777 772e 676f 6f67 6c65  tps://www.google
-00002120: 2e63 6f6d 7a28 2020 2020 3e20 496e 7465  .comz(    > Inte
-00002130: 726e 6574 2063 6f6e 6e65 6374 696f 6e20  rnet connection 
-00002140: 6e6f 7420 6176 6169 6c61 626c 6521 7226  not available!r&
-00002150: 0000 007a 380a 2020 2020 1b5b 313b 3439  ...z8.    .[1;49
-00002160: 3b39 316d 3e20 496e 7465 726e 6574 2063  ;91m> Internet c
-00002170: 6f6e 6e65 6374 696f 6e20 6e6f 7420 6176  onnection not av
-00002180: 6169 6c61 626c 6521 1b5b 306d 0a46 721b  ailable!.[0m.Fr.
-00002190: 0000 0072 1c00 0000 7a3a 2020 2020 1b5b  ...r....z:    .[
-000021a0: 313b 3439 3b39 336d 5b23 5d20 5265 7665  1;49;93m[#] Reve
-000021b0: 7273 6520 6970 2061 6464 7265 7373 206c  rse ip address l
-000021c0: 6f6f 6b75 7020 666f 7220 1b5b 313b 3439  ookup for .[1;49
-000021d0: 3b39 366d 7224 0000 0072 2500 0000 7a24  ;96mr$...r%...z$
-000021e0: 5e5c 647b 312c 337d 5c2e 5c64 7b31 2c33  ^\d{1,3}\.\d{1,3
-000021f0: 7d5c 2e5c 647b 312c 337d 5c2e 5c64 7b31  }\.\d{1,3}\.\d{1
-00002200: 2c33 7d24 7a33 2020 2020 3e20 496e 7661  ,3}$z3    > Inva
-00002210: 6c69 6420 6970 2061 6464 7265 7373 2066  lid ip address f
-00002220: 6f72 6d61 7421 2028 4578 616d 706c 653a  ormat! (Example:
-00002230: 2038 2e38 2e38 2e38 2972 2800 0000 7a41   8.8.8.8)r(...zA
-00002240: 2020 201b 5b31 3b34 393b 3931 6d3e 2049     .[1;49;91m> I
-00002250: 6e76 616c 6964 2069 7020 6164 6472 6573  nvalid ip addres
-00002260: 7320 666f 726d 6174 2120 2845 7861 6d70  s format! (Examp
-00002270: 6c65 3a20 382e 382e 382e 3829 1b5b 306d  le: 8.8.8.8).[0m
-00002280: 0a7a 1768 7474 703a 2f2f 6970 2d61 7069  .z.http://ip-api
-00002290: 2e63 6f6d 2f6a 736f 6e2f 7a11 6874 7470  .com/json/z.http
-000022a0: 733a 2f2f 6970 6170 692e 636f 2f7a 062f  s://ipapi.co/z./
-000022b0: 6a73 6f6e 2f7a 1068 7474 703a 2f2f 6970  json/z.http://ip
-000022c0: 7768 6f2e 6973 2f72 3000 0000 7231 0000  who.is/r0...r1..
-000022d0: 00fa 0a55 7365 722d 4167 656e 747a 444d  ...User-AgentzDM
-000022e0: 6f7a 696c 6c61 2f35 2e30 2028 5831 313b  ozilla/5.0 (X11;
-000022f0: 204c 696e 7578 2078 3836 5f36 343b 2072   Linux x86_64; r
-00002300: 763a 3839 2e30 2920 4765 636b 6f2f 3230  v:89.0) Gecko/20
-00002310: 3130 3031 3031 2046 6972 6566 6f78 2f38  100101 Firefox/8
-00002320: 392e 3029 0372 0100 0000 721e 0000 00e9  9.0).r....r.....
-00002330: 0200 0000 7201 0000 0072 1000 0000 2902  ....r....r....).
-00002340: 7211 0000 00da 0768 6561 6465 7273 e9c8  r......headers..
-00002350: 0000 00da 0673 7461 7475 73da 0773 7563  .....status..suc
-00002360: 6365 7373 7246 0000 00da 0b63 6f75 6e74  cessrF.....count
-00002370: 7279 436f 6465 5a0a 7265 6769 6f6e 4e61  ryCodeZ.regionNa
-00002380: 6d65 da06 7265 6769 6f6e da04 6369 7479  me..region..city
-00002390: da03 6973 70da 036f 7267 7218 0000 00da  ..isp..orgr.....
-000023a0: 037a 6970 5a03 6c61 745a 036c 6f6e da05  .zipZ.latZ.lon..
-000023b0: 7175 6572 797a 2072 6576 6572 7365 2d69  queryz reverse-i
-000023c0: 702d 6c6f 6f6b 7570 2d73 6572 7665 722d  p-lookup-server-
-000023d0: 312d 6572 726f 7275 d200 0000 0a20 2020  1-erroru.....   
-000023e0: 20e2 948c e294 80e2 9480 e294 80e2 9480   ...............
-000023f0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00002400: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00002410: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00002420: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00002430: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00002440: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00000980: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00000990: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+000009a0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+000009b0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+000009c0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+000009d0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+000009e0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+000009f0: 9480 e294 80e2 9480 e294 900a 2020 2020  ............    
+00000a00: 7c20 5363 616e 6e65 6420 5068 6f6e 6520  | Scanned Phone 
+00000a10: 4e75 6d62 6572 3a20 1b5b 313b 3439 3b39  Number: .[1;49;9
+00000a20: 366d 7ae8 1b5b 306d 207c 0a20 2020 207c  6mz..[0m |.    |
+00000a30: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000a40: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000a50: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000a60: 2d2d 2d2d 2d2d 7c0a 2020 2020 7c20 494e  ------|.    | IN
+00000a70: 464f 524d 4154 494f 4e20 2020 2020 2020  FORMATION       
+00000a80: 2020 7c20 4445 5343 5249 5054 494f 4e20    | DESCRIPTION 
+00000a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000aa0: 2020 207c 0a20 2020 207c 2d2d 2d2d 2d2d     |.    |------
+00000ab0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000ac0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000ad0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000ae0: 7c0a 2020 2020 7c20 1b5b 313b 3439 3b39  |.    | .[1;49;9
+00000af0: 376d 506f 7373 6962 6c65 1b5b 306d 2020  7mPossible.[0m  
+00000b00: 2020 2020 2020 2020 2020 7c20 7a2d 207c            | z- |
+00000b10: 0a20 2020 207c 201b 5b31 3b34 393b 3937  .    | .[1;49;97
+00000b20: 6d56 616c 6964 1b5b 306d 2020 2020 2020  mValid.[0m      
+00000b30: 2020 2020 2020 2020 207c 207a 6a20 7c0a           | zj |.
+00000b40: 2020 2020 7c2d 2d2d 2d2d 2d2d 2d2d 2d2d      |-----------
+00000b50: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000b60: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000b70: 2d2d 2d2d 2d2d 2d2d 2d2d 2d7c 0a20 2020  -----------|.   
+00000b80: 207c 201b 5b31 3b34 393b 3937 6d43 6f75   | .[1;49;97mCou
+00000b90: 6e74 7279 2043 6f64 651b 5b30 6d20 2020  ntry Code.[0m   
+00000ba0: 2020 2020 207c 207a 2d20 7c0a 2020 2020       | z- |.    
+00000bb0: 7c20 1b5b 313b 3439 3b39 376d 436f 756e  | .[1;49;97mCoun
+00000bc0: 7472 791b 5b30 6d20 2020 2020 2020 2020  try.[0m         
+00000bd0: 2020 2020 7c20 fa2d 207c 0a20 2020 207c      | .- |.    |
+00000be0: 201b 5b31 3b34 393b 3937 6d52 6567 696f   .[1;49;97mRegio
+00000bf0: 6e20 436f 6465 1b5b 306d 2020 2020 2020  n Code.[0m      
+00000c00: 2020 207c 207a 2d20 7c0a 2020 2020 7c20     | z- |.    | 
+00000c10: 1b5b 313b 3439 3b39 376d 5365 7276 6963  .[1;49;97mServic
+00000c20: 6520 5072 6f76 6964 6572 1b5b 306d 2020  e Provider.[0m  
+00000c30: 2020 7c20 fa2d 207c 0a20 2020 207c 201b    | .- |.    | .
+00000c40: 5b31 3b34 393b 3937 6d54 696d 657a 6f6e  [1;49;97mTimezon
+00000c50: 651b 5b30 6d20 2020 2020 2020 2020 2020  e.[0m           
+00000c60: 207c 207a 6a20 7c0a 2020 2020 7c2d 2d2d   | zj |.    |---
+00000c70: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000c80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000c90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000ca0: 2d2d 2d7c 0a20 2020 207c 201b 5b31 3b34  ---|.    | .[1;4
+00000cb0: 393b 3937 6d49 6e74 6572 6e61 7469 6f6e  9;97mInternation
+00000cc0: 616c 2046 6f72 6d61 741b 5b30 6d7c 207a  al Format.[0m| z
+00000cd0: 2d20 7c0a 2020 2020 7c20 1b5b 313b 3439  - |.    | .[1;49
+00000ce0: 3b39 376d 4e61 7469 6f6e 616c 2046 6f72  ;97mNational For
+00000cf0: 6d61 741b 5b30 6d20 2020 2020 7c20 7a2d  mat.[0m     | z-
+00000d00: 207c 0a20 2020 207c 201b 5b31 3b34 393b   |.    | .[1;49;
+00000d10: 3937 6d52 4643 3339 3636 2046 6f72 6d61  97mRFC3966 Forma
+00000d20: 741b 5b30 6d20 2020 2020 207c 2075 b800  t.[0m      | u..
+00000d30: 0000 207c 0a20 2020 20e2 9494 e294 80e2  .. |.    .......
+00000d40: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00000d50: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00000d60: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00000d70: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00000d80: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00000d90: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00000da0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00000db0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00000dc0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00000dd0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00000de0: 980a 2020 2020 2020 2020 da01 0a7a 2b0a  ..        ...z+.
+00000df0: 2020 2020 1b5b 313b 3439 3b39 336d 5b2b      .[1;49;93m[+
+00000e00: 5d20 5365 6172 6368 696e 6720 666f 7220  ] Searching for 
+00000e10: 1b5b 313b 3439 3b39 366d 7a74 1b5b 313b  .[1;49;96mzt.[1;
+00000e20: 3439 3b39 336d 206f 6e20 7661 7269 6f75  49;93m on variou
+00000e30: 7320 706c 6174 666f 726d 733a 0a0a 2020  s platforms:..  
+00000e40: 2020 1b5b 313b 3439 3b39 326d 3e20 6874    .[1;49;92m> ht
+00000e50: 7470 733a 2f2f 7777 772e 6970 7175 616c  tps://www.ipqual
+00000e60: 6974 7973 636f 7265 2e63 6f6d 2f72 6576  ityscore.com/rev
+00000e70: 6572 7365 2d70 686f 6e65 2d6e 756d 6265  erse-phone-numbe
+00000e80: 722d 6c6f 6f6b 7570 2f6c 6f6f 6b75 702f  r-lookup/lookup/
+00000e90: fa01 2f7a 290a 2020 2020 3e20 6874 7470  ../z).    > http
+00000ea0: 733a 2f2f 7777 772e 7472 7565 6361 6c6c  s://www.truecall
+00000eb0: 6572 2e63 6f6d 2f73 6561 7263 682f 7a09  er.com/search/z.
+00000ec0: 0a20 2020 201b 5b30 6d7a 590a 2020 2020  .    .[0mzY.    
+00000ed0: 1b5b 313b 3439 3b39 336d 5b2b 5d20 476f  .[1;49;93m[+] Go
+00000ee0: 6f67 6c65 2044 6f72 6b20 5175 6572 6965  ogle Dork Querie
+00000ef0: 733a 0a0a 2020 2020 1b5b 313b 3439 3b39  s:..    .[1;49;9
+00000f00: 326d 3e20 6874 7470 733a 2f2f 7777 772e  2m> https://www.
+00000f10: 676f 6f67 6c65 2e63 6f6d 2f73 6561 7263  google.com/searc
+00000f20: 683f 713d 7a28 2020 2020 5b2b 5d20 5363  h?q=z(    [+] Sc
+00000f30: 616e 6e69 6e67 2073 6f63 6961 6c20 6d65  anning social me
+00000f40: 6469 6120 706c 6174 666f 726d 733a 291c  dia platforms:).
+00000f50: da0c 7068 6f6e 656e 756d 6265 7273 721e  ..phonenumbersr.
+00000f60: 0000 0072 1f00 0000 7220 0000 00da 0670  ...r....r .....p
+00000f70: 7276 5f6f 70da 0770 7269 6e74 6974 da02  rv_op..printit..
+00000f80: 7265 da05 6d61 7463 68da 0570 6172 7365  re..match..parse
+00000f90: 5a0f 7068 6f6e 656e 756d 6265 7275 7469  Z.phonenumberuti
+00000fa0: 6c5a 144e 756d 6265 7250 6172 7365 4578  lZ.NumberParseEx
+00000fb0: 6365 7074 696f 6eda 0373 7472 da05 7370  ception..str..sp
+00000fc0: 6c69 74da 0573 7472 6970 5a0f 6973 5f76  lit..stripZ.is_v
+00000fd0: 616c 6964 5f6e 756d 6265 725a 1269 735f  alid_numberZ.is_
+00000fe0: 706f 7373 6962 6c65 5f6e 756d 6265 725a  possible_numberZ
+00000ff0: 1672 6567 696f 6e5f 636f 6465 5f66 6f72  .region_code_for
+00001000: 5f6e 756d 6265 725a 1664 6573 6372 6970  _numberZ.descrip
+00001010: 7469 6f6e 5f66 6f72 5f6e 756d 6265 725a  tion_for_numberZ
+00001020: 0f6e 616d 655f 666f 725f 6e75 6d62 6572  .name_for_number
+00001030: 5a15 7469 6d65 5f7a 6f6e 6573 5f66 6f72  Z.time_zones_for
+00001040: 5f6e 756d 6265 72da 0772 6570 6c61 6365  _number..replace
+00001050: 5a0d 666f 726d 6174 5f6e 756d 6265 725a  Z.format_numberZ
+00001060: 1150 686f 6e65 4e75 6d62 6572 466f 726d  .PhoneNumberForm
+00001070: 6174 5a07 5246 4333 3936 36da 0369 6e74  atZ.RFC3966..int
+00001080: da03 6c65 6eda 0570 7269 6e74 da05 6c6f  ..len..print..lo
+00001090: 7765 7229 145a 0c70 686f 6e65 5f6e 756d  wer).Z.phone_num
+000010a0: 6265 7272 1e00 0000 721f 0000 0072 2000  berr....r....r .
+000010b0: 0000 5a14 7068 6f6e 655f 6e75 6d62 6572  ..Z.phone_number
+000010c0: 5f64 6574 6169 6c73 da0c 636f 756e 7472  _details..countr
+000010d0: 795f 636f 6465 5a0b 6f6e 6c79 5f6e 756d  y_codeZ.only_num
+000010e0: 6265 725a 0576 616c 6964 da08 706f 7373  berZ.valid..poss
+000010f0: 6962 6c65 5a0e 636f 756e 7274 795f 6e75  ibleZ.counrty_nu
+00001100: 6d62 6572 da0b 7265 6769 6f6e 5f63 6f64  mber..region_cod
+00001110: 65da 0763 6f75 6e74 7279 5a0e 7365 7276  e..countryZ.serv
+00001120: 6963 655f 6e75 6d62 6572 5a10 7365 7276  ice_numberZ.serv
+00001130: 6963 655f 7072 6f76 6964 6572 5a1b 7469  ice_providerZ.ti
+00001140: 6d65 7a6f 6e65 5f64 6574 6169 6c73 5f75  mezone_details_u
+00001150: 6e66 696c 7465 7265 645a 1074 696d 657a  nfilteredZ.timez
+00001160: 6f6e 655f 6465 7461 696c 735a 0872 5f66  one_detailsZ.r_f
+00001170: 6f72 6d61 74da 0c66 696e 616c 5f6f 7574  ormat..final_out
+00001180: 7075 745a 126f 6e6c 696e 655f 6672 6565  putZ.online_free
+00001190: 5f6c 6f6f 6b75 705a 1367 6f6f 676c 655f  _lookupZ.google_
+000011a0: 646f 726b 5f71 7565 7269 6573 721b 0000  dork_queriesr...
+000011b0: 0072 1b00 0000 721c 0000 00da 0d6e 756d  .r....r......num
+000011c0: 6265 725f 6c6f 6f6b 7570 4400 0000 73be  ber_lookupD...s.
+000011d0: 0000 0000 020c 010c 010c 0404 031a 0114  ................
+000011e0: 030c 0110 0104 0302 020e 0110 0110 0108  ................
+000011f0: 0324 0124 030a 030a 020c 020c 030a 030c  .$.$............
+00001200: 030c 030c 030e 013c 0318 0320 0120 0120  .......<... . . 
+00001210: 0120 0120 0120 0120 0120 0120 0120 0302  . . . . . . . ..
+00001220: 0202 fe04 0602 fa04 0702 f904 0902 f704  ................
+00001230: 0a02 f604 0b02 f504 0c02 f404 0d02 f304  ................
+00001240: 0202 fe04 1002 f004 1102 ef08 1408 010c  ................
+00001250: 0302 0106 ff04 0306 fd04 0306 fd04 040a  ................
+00001260: fc04 0306 fd08 0608 010c 0302 0306 fd08  ................
+00001270: 0508 010c 0312 0204 0420 0120 0120 0202  ......... . . ..
+00001280: 0202 fe04 0602 fa04 0702 f908 0a08 010c  ................
+00001290: 0172 4f00 0000 6301 0000 0000 0000 0000  .rO...c.........
+000012a0: 0000 0036 0000 0037 0000 0043 0000 0073  ...6...7...C...s
+000012b0: 160f 0000 6401 6100 7401 6402 6700 6403  ....d.a.t.d.g.d.
+000012c0: a201 6404 6405 8d03 0100 7402 8300 7332  ..d.d.....t...s2
+000012d0: 7401 6406 6700 6407 a201 6404 6405 8d03  t.d.g.d...d.d...
+000012e0: 0100 6408 5300 7401 6409 7c00 9b00 640a  ..d.S.t.d.|...d.
+000012f0: 9d03 6700 6403 a201 6404 6405 8d03 0100  ..g.d...d.d.....
+00001300: 7400 640b 7c00 9b00 640c 9d03 640d 1700  t.d.|...d...d...
+00001310: 3700 6100 7403 a004 640e 7c00 a102 7380  7.a.t...d.|...s.
+00001320: 7401 640f 6700 6407 a201 6410 8d02 0100  t.d.g.d...d.....
+00001330: 6408 5300 6411 7c00 9b00 9d02 6412 7c00  d.S.d.|.....d.|.
+00001340: 9b00 6413 9d03 6414 7c00 9b00 9d02 6703  ..d...d.|.....g.
+00001350: 7d01 7405 7c00 8301 6415 7406 6416 7407  }.t.|...d.t.d.t.
+00001360: 7405 7c00 8301 8301 1800 8301 1400 1700  t.|.............
+00001370: 7d00 6417 6418 6901 7d02 7408 a009 6700  }.d.d.i.}.t...g.
+00001380: 6419 a201 a101 7d03 7c03 641a 6b02 9003  d.....}.|.d.k...
+00001390: 72ba 9002 7a86 740a 6a0b 7c01 641a 1900  r...z.t.j.|.d...
+000013a0: 641b 7c02 641c 8d03 7d04 7c04 a00c a100  d.|.d...}.|.....
+000013b0: 7d05 7c04 6a0d 641d 6b02 9001 727a 7c05  }.|.j.d.k...rz|.
+000013c0: 641e 1900 641f 6b02 9001 727a 7c05 6420  d...d.k...rz|.d 
+000013d0: 1900 7d06 7c05 6421 1900 7d07 7c05 6422  ..}.|.d!..}.|.d"
+000013e0: 1900 7d08 7c05 6423 1900 7d09 7c05 6424  ..}.|.d#..}.|.d$
+000013f0: 1900 7d0a 7c05 6425 1900 7d0b 7c05 6426  ..}.|.d%..}.|.d&
+00001400: 1900 7d0c 7c05 6427 1900 7d0d 7c05 6428  ..}.|.d'..}.|.d(
+00001410: 1900 7d0e 7c05 6429 1900 7d0f 7c05 642a  ..}.|.d)..}.|.d*
+00001420: 1900 7d10 7c05 642b 1900 7d11 6e08 740e  ..}.|.d+..}.n.t.
+00001430: 642c 8301 8201 7405 7c06 8301 6415 7406  d,....t.|...d.t.
+00001440: 6416 7407 7405 7c06 8301 8301 1800 8301  d.t.t.|.........
+00001450: 1400 1700 7d06 7405 7c07 8301 6415 7406  ....}.t.|...d.t.
+00001460: 6416 7407 7405 7c07 8301 8301 1800 8301  d.t.t.|.........
+00001470: 1400 1700 7d07 7405 7c08 8301 6415 7406  ....}.t.|...d.t.
+00001480: 6416 7407 7405 7c08 8301 8301 1800 8301  d.t.t.|.........
+00001490: 1400 1700 7d08 7405 7c09 8301 6415 7406  ....}.t.|...d.t.
+000014a0: 6416 7407 7405 7c09 8301 8301 1800 8301  d.t.t.|.........
+000014b0: 1400 1700 7d09 7405 7c0a 8301 6415 7406  ....}.t.|...d.t.
+000014c0: 6416 7407 7405 7c0a 8301 8301 1800 8301  d.t.t.|.........
+000014d0: 1400 1700 7d0a 7405 7c0b 8301 6415 7406  ....}.t.|...d.t.
+000014e0: 6416 7407 7405 7c0b 8301 8301 1800 8301  d.t.t.|.........
+000014f0: 1400 1700 7d0b 7405 7c0c 8301 6415 7406  ....}.t.|...d.t.
+00001500: 6416 7407 7405 7c0c 8301 8301 1800 8301  d.t.t.|.........
+00001510: 1400 1700 7d0c 7405 7c0d 8301 6415 7406  ....}.t.|...d.t.
+00001520: 6416 7407 7405 7c0d 8301 8301 1800 8301  d.t.t.|.........
+00001530: 1400 1700 7d0d 7405 7c0e 8301 6415 7406  ....}.t.|...d.t.
+00001540: 6416 7407 7405 7c0e 8301 8301 1800 8301  d.t.t.|.........
+00001550: 1400 1700 7d0e 7405 7c0f 8301 6415 7406  ....}.t.|...d.t.
+00001560: 6416 7407 7405 7c0f 8301 8301 1800 8301  d.t.t.|.........
+00001570: 1400 1700 7d0f 7405 7c10 8301 6415 7406  ....}.t.|...d.t.
+00001580: 6416 7407 7405 7c10 8301 8301 1800 8301  d.t.t.|.........
+00001590: 1400 1700 7d10 7405 7c11 8301 6415 7406  ....}.t.|...d.t.
+000015a0: 6416 7407 7405 7c11 8301 8301 1800 8301  d.t.t.|.........
+000015b0: 1400 1700 7d11 642d 7c00 9b00 642e 7c06  ....}.d-|...d.|.
+000015c0: 9b00 642f 7c07 9b00 6430 7c08 9b00 6431  ..d/|...d0|...d1
+000015d0: 7c09 9b00 6432 7c0a 9b00 6433 7c0e 9b00  |...d2|...d3|...
+000015e0: 6434 7c0d 9b00 6435 7c0f 9b00 6436 7c10  d4|...d5|...d6|.
+000015f0: 9b00 6437 7c0b 9b00 6438 7c0c 9b00 6439  ..d7|...d8|...d9
+00001600: 9d19 7d12 740f 7c12 8301 0100 7400 7c12  ..}.t.|.....t.|.
+00001610: 643a 1700 3700 6100 5700 6e4e 0400 740e  d:..7.a.W.nN..t.
+00001620: 9003 79b4 0100 7d13 0100 7a34 740f 7c13  ..y...}...z4t.|.
+00001630: 8301 0100 642d 7c00 9b00 643b 9d03 7d12  ....d-|...d;..}.
+00001640: 740f 7c12 8301 0100 7400 7c12 643a 1700  t.|.....t.|.d:..
+00001650: 3700 6100 5700 5900 6400 7d13 7e13 6e0a  7.a.W.Y.d.}.~.n.
+00001660: 6400 7d13 7e13 3000 3000 900b 6e58 7c03  d.}.~.0.0...nX|.
+00001670: 643c 6b02 9009 7222 9005 7a2a 740a 6a0b  d<k...r"..z*t.j.
+00001680: 7c01 643c 1900 641b 7c02 641c 8d03 7d04  |.d<..d.|.d...}.
+00001690: 7c04 a00c a100 7d05 7c04 6a0d 641d 6b02  |.....}.|.j.d.k.
+000016a0: 9004 72ca 7c05 643d 1900 7d11 7c05 643e  ..r.|.d=..}.|.d>
+000016b0: 1900 7d14 7c05 643f 1900 7d15 7c05 6424  ..}.|.d?..}.|.d$
+000016c0: 1900 7d0a 7c05 6423 1900 7d08 7c05 6440  ..}.|.d#..}.|.d@
+000016d0: 1900 7d16 7c05 6441 1900 7d06 7c05 6441  ..}.|.dA..}.|.dA
+000016e0: 1900 7d17 7c05 6442 1900 7d18 7c05 6443  ..}.|.dB..}.|.dC
+000016f0: 1900 7d19 7c05 6444 1900 7d1a 7c05 6445  ..}.|.dD..}.|.dE
+00001700: 1900 7d1b 7c05 6446 1900 7d1c 7c05 6447  ..}.|.dF..}.|.dG
+00001710: 1900 7d1d 7c05 6448 1900 7d0e 7c05 6449  ..}.|.dH..}.|.dI
+00001720: 1900 7d0f 7c05 644a 1900 7d10 7c05 6427  ..}.|.dJ..}.|.d'
+00001730: 1900 7d0d 7c05 644b 1900 7d1e 7c05 644c  ..}.|.dK..}.|.dL
+00001740: 1900 7d1f 7c05 644d 1900 7d20 7c05 644e  ..}.|.dM..} |.dN
+00001750: 1900 7d21 7c05 644f 1900 7d22 7c05 6450  ..}!|.dO..}"|.dP
+00001760: 1900 7d23 7c05 6451 1900 7d24 7c05 6452  ..}#|.dQ..}$|.dR
+00001770: 1900 7d25 7c05 6426 1900 7d0c 6e08 740e  ..}%|.d&..}.n.t.
+00001780: 6453 8301 8201 7405 7c11 8301 6415 7406  dS....t.|...d.t.
+00001790: 6416 7407 7405 7c11 8301 8301 1800 8301  d.t.t.|.........
+000017a0: 1400 1700 7d11 7405 7c14 8301 6415 7406  ....}.t.|...d.t.
+000017b0: 6416 7407 7405 7c14 8301 8301 1800 8301  d.t.t.|.........
+000017c0: 1400 1700 7d14 7405 7c15 8301 6415 7406  ....}.t.|...d.t.
+000017d0: 6416 7407 7405 7c15 8301 8301 1800 8301  d.t.t.|.........
+000017e0: 1400 1700 7d15 7405 7c0a 8301 6415 7406  ....}.t.|...d.t.
+000017f0: 6416 7407 7405 7c0a 8301 8301 1800 8301  d.t.t.|.........
+00001800: 1400 1700 7d0a 7405 7c08 8301 6415 7406  ....}.t.|...d.t.
+00001810: 6416 7407 7405 7c08 8301 8301 1800 8301  d.t.t.|.........
+00001820: 1400 1700 7d08 7405 7c16 8301 6415 7406  ....}.t.|...d.t.
+00001830: 6416 7407 7405 7c16 8301 8301 1800 8301  d.t.t.|.........
+00001840: 1400 1700 7d16 7405 7c06 8301 6415 7406  ....}.t.|...d.t.
+00001850: 6416 7407 7405 7c06 8301 8301 1800 8301  d.t.t.|.........
+00001860: 1400 1700 7d06 7405 7c17 8301 6415 7406  ....}.t.|...d.t.
+00001870: 6416 7407 7405 7c17 8301 8301 1800 8301  d.t.t.|.........
+00001880: 1400 1700 7d17 7405 7c18 8301 6415 7406  ....}.t.|...d.t.
+00001890: 6416 7407 7405 7c18 8301 8301 1800 8301  d.t.t.|.........
+000018a0: 1400 1700 7d18 7405 7c19 8301 6415 7406  ....}.t.|...d.t.
+000018b0: 6416 7407 7405 7c19 8301 8301 1800 8301  d.t.t.|.........
+000018c0: 1400 1700 7d19 7405 7c1a 8301 6415 7406  ....}.t.|...d.t.
+000018d0: 6416 7407 7405 7c1a 8301 8301 1800 8301  d.t.t.|.........
+000018e0: 1400 1700 7d1a 7405 7c1b 8301 6415 7406  ....}.t.|...d.t.
+000018f0: 6416 7407 7405 7c1b 8301 8301 1800 8301  d.t.t.|.........
+00001900: 1400 1700 7d1b 7405 7c1c 8301 6415 7406  ....}.t.|...d.t.
+00001910: 6416 7407 7405 7c1c 8301 8301 1800 8301  d.t.t.|.........
+00001920: 1400 1700 7d1c 7405 7c1d 8301 6415 7406  ....}.t.|...d.t.
+00001930: 6416 7407 7405 7c1d 8301 8301 1800 8301  d.t.t.|.........
+00001940: 1400 1700 7d1d 7405 7c0e 8301 6415 7406  ....}.t.|...d.t.
+00001950: 6416 7407 7405 7c0e 8301 8301 1800 8301  d.t.t.|.........
+00001960: 1400 1700 7d0e 7405 7c0f 8301 6415 7406  ....}.t.|...d.t.
+00001970: 6416 7407 7405 7c0f 8301 8301 1800 8301  d.t.t.|.........
+00001980: 1400 1700 7d0f 7405 7c10 8301 6415 7406  ....}.t.|...d.t.
+00001990: 6416 7407 7405 7c10 8301 8301 1800 8301  d.t.t.|.........
+000019a0: 1400 1700 7d10 7405 7c0d 8301 6415 7406  ....}.t.|...d.t.
+000019b0: 6416 7407 7405 7c0d 8301 8301 1800 8301  d.t.t.|.........
+000019c0: 1400 1700 7d0d 7405 7c1e 8301 6415 7406  ....}.t.|...d.t.
+000019d0: 6416 7407 7405 7c1e 8301 8301 1800 8301  d.t.t.|.........
+000019e0: 1400 1700 7d1e 7405 7c1f 8301 6415 7406  ....}.t.|...d.t.
+000019f0: 6416 7407 7405 7c1f 8301 8301 1800 8301  d.t.t.|.........
+00001a00: 1400 1700 7d1f 7405 7c20 8301 6415 7406  ....}.t.| ..d.t.
+00001a10: 6416 7407 7405 7c20 8301 8301 1800 8301  d.t.t.| ........
+00001a20: 1400 1700 7d20 7405 7c21 8301 6415 7406  ....} t.|!..d.t.
+00001a30: 6416 7407 7405 7c21 8301 8301 1800 8301  d.t.t.|!........
+00001a40: 1400 1700 7d21 7405 7c22 8301 6415 7406  ....}!t.|"..d.t.
+00001a50: 6416 7407 7405 7c22 8301 8301 1800 8301  d.t.t.|"........
+00001a60: 1400 1700 7d22 7405 7c23 8301 6415 7406  ....}"t.|#..d.t.
+00001a70: 6416 7407 7405 7c23 8301 8301 1800 8301  d.t.t.|#........
+00001a80: 1400 1700 7d23 7405 7c24 8301 6415 7406  ....}#t.|$..d.t.
+00001a90: 6416 7407 7405 7c24 8301 8301 1800 8301  d.t.t.|$........
+00001aa0: 1400 1700 7d24 7405 7c25 8301 6415 7406  ....}$t.|%..d.t.
+00001ab0: 6416 7407 7405 7c25 8301 8301 1800 8301  d.t.t.|%........
+00001ac0: 1400 1700 7d25 7405 7c0c 8301 6415 7406  ....}%t.|...d.t.
+00001ad0: 6416 7407 7405 7c0c 8301 8301 1800 8301  d.t.t.|.........
+00001ae0: 1400 1700 7d0c 642d 7c00 9b00 6454 7c15  ....}.d-|...dT|.
+00001af0: 9b00 6455 7c14 9b00 6456 7c06 9b00 6457  ..dU|...dV|...dW
+00001b00: 7c17 9b00 642f 7c18 9b00 6458 7c19 9b00  |...d/|...dX|...
+00001b10: 6459 7c1a 9b00 6430 7c08 9b00 6431 7c16  dY|...d0|...d1|.
+00001b20: 9b00 6432 7c0a 9b00 645a 7c1b 9b00 645b  ..d2|...dZ|...d[
+00001b30: 7c1f 9b00 645c 7c1c 9b00 645d 7c1d 9b00  |...d\|...d]|...
+00001b40: 645e 7c23 9b00 645f 7c24 9b00 6460 7c22  d^|#..d_|$..d`|"
+00001b50: 9b00 6461 7c20 9b00 6462 7c21 9b00 6433  ..da| ..db|!..d3
+00001b60: 7c0e 9b00 6435 7c0f 9b00 6436 7c10 9b00  |...d5|...d6|...
+00001b70: 6434 7c0d 9b00 6463 7c1e 9b00 6464 7c25  d4|...dc|...dd|%
+00001b80: 9b00 6465 7c0c 9b00 6439 9d37 7d12 740f  ..de|...d9.7}.t.
+00001b90: 7c12 8301 0100 7400 7c12 643a 1700 3700  |.....t.|.d:..7.
+00001ba0: 6100 5700 6e2c 0100 0100 0100 642d 7c00  a.W.n,......d-|.
+00001bb0: 9b00 643b 9d03 7d12 740f 7c12 8301 0100  ..d;..}.t.|.....
+00001bc0: 7400 7c12 643a 1700 3700 6100 5900 6e02  t.|.d:..7.a.Y.n.
+00001bd0: 3000 9005 6ef0 7c03 6466 6b02 900f 7212  0...n.|.dfk...r.
+00001be0: 9005 7ab6 740a 6a0b 7c01 6466 1900 641b  ..z.t.j.|.df..d.
+00001bf0: 7c02 641c 8d03 7d04 7c04 a00c a100 7d05  |.d...}.|.....}.
+00001c00: 7c04 6a0d 641d 6b02 900a 7284 7c05 641f  |.j.d.k...r.|.d.
+00001c10: 1900 6404 6b02 900a 7284 7c05 643d 1900  ..d.k...r.|.d=..
+00001c20: 7d11 7c05 6467 1900 7d26 7c05 6468 1900  }.|.dg..}&|.dh..
+00001c30: 7d27 7c05 6446 1900 7d1c 7c05 6420 1900  }'|.dF..}.|.d ..
+00001c40: 7d06 7c05 6442 1900 7d18 7c05 6423 1900  }.|.dB..}.|.d#..
+00001c50: 7d08 7c05 6440 1900 7d16 7c05 6424 1900  }.|.d@..}.|.d$..
+00001c60: 7d0a 7c05 6449 1900 7d0f 7c05 644a 1900  }.|.dI..}.|.dJ..
+00001c70: 7d10 7c05 6469 1900 7d28 7c05 6448 1900  }.|.di..}(|.dH..
+00001c80: 7d0e 7c05 646a 1900 7d29 7c05 646b 1900  }.|.dj..})|.dk..
+00001c90: 7d2a 7c05 646c 1900 7d2b 7c05 646d 1900  }*|.dl..}+|.dm..
+00001ca0: 646e 1900 7d2c 7c05 646d 1900 646f 1900  dn..},|.dm..do..
+00001cb0: 7d2d 7c05 646d 1900 6470 1900 7d2e 7c05  }-|.dm..dp..}.|.
+00001cc0: 6471 1900 6452 1900 7d25 7c05 6471 1900  dq..dR..}%|.dq..
+00001cd0: 6426 1900 7d0c 7c05 6471 1900 6425 1900  d&..}.|.dq..d%..
+00001ce0: 7d0b 7c05 6471 1900 6472 1900 7d2f 7c05  }.|.dq..dr..}/|.
+00001cf0: 6427 1900 6473 1900 7d30 7c05 6427 1900  d'..ds..}0|.d'..
+00001d00: 6474 1900 7d31 7c05 6427 1900 6475 1900  dt..}1|.d'..du..
+00001d10: 7d32 7c05 6427 1900 6476 1900 7d33 7c05  }2|.d'..dv..}3|.
+00001d20: 6427 1900 6477 1900 7d34 7c05 6427 1900  d'..dw..}4|.d'..
+00001d30: 6478 1900 7d35 6e08 740e 6479 8301 8201  dx..}5n.t.dy....
+00001d40: 7405 7c11 8301 6415 7406 6416 7407 7405  t.|...d.t.d.t.t.
+00001d50: 7c11 8301 8301 1800 8301 1400 1700 7d11  |.............}.
+00001d60: 7405 7c26 8301 6415 7406 6416 7407 7405  t.|&..d.t.d.t.t.
+00001d70: 7c26 8301 8301 1800 8301 1400 1700 7d26  |&............}&
+00001d80: 7405 7c27 8301 6415 7406 6416 7407 7405  t.|'..d.t.d.t.t.
+00001d90: 7c27 8301 8301 1800 8301 1400 1700 7d27  |'............}'
+00001da0: 7405 7c1c 8301 6415 7406 6416 7407 7405  t.|...d.t.d.t.t.
+00001db0: 7c1c 8301 8301 1800 8301 1400 1700 7d1c  |.............}.
+00001dc0: 7405 7c06 8301 6415 7406 6416 7407 7405  t.|...d.t.d.t.t.
+00001dd0: 7c06 8301 8301 1800 8301 1400 1700 7d06  |.............}.
+00001de0: 7405 7c18 8301 6415 7406 6416 7407 7405  t.|...d.t.d.t.t.
+00001df0: 7c18 8301 8301 1800 8301 1400 1700 7d18  |.............}.
+00001e00: 7405 7c08 8301 6415 7406 6416 7407 7405  t.|...d.t.d.t.t.
+00001e10: 7c08 8301 8301 1800 8301 1400 1700 7d08  |.............}.
+00001e20: 7405 7c16 8301 6415 7406 6416 7407 7405  t.|...d.t.d.t.t.
+00001e30: 7c16 8301 8301 1800 8301 1400 1700 7d16  |.............}.
+00001e40: 7405 7c0a 8301 6415 7406 6416 7407 7405  t.|...d.t.d.t.t.
+00001e50: 7c0a 8301 8301 1800 8301 1400 1700 7d0a  |.............}.
+00001e60: 7405 7c0f 8301 6415 7406 6416 7407 7405  t.|...d.t.d.t.t.
+00001e70: 7c0f 8301 8301 1800 8301 1400 1700 7d0f  |.............}.
+00001e80: 7405 7c10 8301 6415 7406 6416 7407 7405  t.|...d.t.d.t.t.
+00001e90: 7c10 8301 8301 1800 8301 1400 1700 7d10  |.............}.
+00001ea0: 7405 7c28 8301 6415 7406 6416 7407 7405  t.|(..d.t.d.t.t.
+00001eb0: 7c28 8301 8301 1800 8301 1400 1700 7d28  |(............}(
+00001ec0: 7405 7c0e 8301 6415 7406 6416 7407 7405  t.|...d.t.d.t.t.
+00001ed0: 7c0e 8301 8301 1800 8301 1400 1700 7d0e  |.............}.
+00001ee0: 7405 7c29 8301 6415 7406 6416 7407 7405  t.|)..d.t.d.t.t.
+00001ef0: 7c29 8301 8301 1800 8301 1400 1700 7d29  |)............})
+00001f00: 7405 7c2a 8301 6415 7406 6416 7407 7405  t.|*..d.t.d.t.t.
+00001f10: 7c2a 8301 8301 1800 8301 1400 1700 7d2a  |*............}*
+00001f20: 7405 7c2b 8301 6415 7406 6416 7407 7405  t.|+..d.t.d.t.t.
+00001f30: 7c2b 8301 8301 1800 8301 1400 1700 7d2b  |+............}+
+00001f40: 7405 7c2c 8301 6415 7406 6416 7407 7405  t.|,..d.t.d.t.t.
+00001f50: 7c2c 8301 8301 1800 8301 1400 1700 7d2c  |,............},
+00001f60: 7405 7c2d 8301 6415 7406 6416 7407 7405  t.|-..d.t.d.t.t.
+00001f70: 7c2d 8301 8301 1800 8301 1400 1700 7d2d  |-............}-
+00001f80: 7405 7c2e 8301 6415 7406 6416 7407 7405  t.|...d.t.d.t.t.
+00001f90: 7c2e 8301 8301 1800 8301 1400 1700 7d2e  |.............}.
+00001fa0: 7405 7c25 8301 6415 7406 6416 7407 7405  t.|%..d.t.d.t.t.
+00001fb0: 7c25 8301 8301 1800 8301 1400 1700 7d25  |%............}%
+00001fc0: 7405 7c0c 8301 6415 7406 6416 7407 7405  t.|...d.t.d.t.t.
+00001fd0: 7c0c 8301 8301 1800 8301 1400 1700 7d0c  |.............}.
+00001fe0: 7405 7c0b 8301 6415 7406 6416 7407 7405  t.|...d.t.d.t.t.
+00001ff0: 7c0b 8301 8301 1800 8301 1400 1700 7d0b  |.............}.
+00002000: 7405 7c2f 8301 6415 7406 6416 7407 7405  t.|/..d.t.d.t.t.
+00002010: 7c2f 8301 8301 1800 8301 1400 1700 7d2f  |/............}/
+00002020: 7405 7c30 8301 6415 7406 6416 7407 7405  t.|0..d.t.d.t.t.
+00002030: 7c30 8301 8301 1800 8301 1400 1700 7d30  |0............}0
+00002040: 7405 7c31 8301 6415 7406 6416 7407 7405  t.|1..d.t.d.t.t.
+00002050: 7c31 8301 8301 1800 8301 1400 1700 7d31  |1............}1
+00002060: 7405 7c32 8301 6415 7406 6416 7407 7405  t.|2..d.t.d.t.t.
+00002070: 7c32 8301 8301 1800 8301 1400 1700 7d32  |2............}2
+00002080: 7405 7c33 8301 6415 7406 6416 7407 7405  t.|3..d.t.d.t.t.
+00002090: 7c33 8301 8301 1800 8301 1400 1700 7d33  |3............}3
+000020a0: 7405 7c34 8301 6415 7406 6416 7407 7405  t.|4..d.t.d.t.t.
+000020b0: 7c34 8301 8301 1800 8301 1400 1700 7d34  |4............}4
+000020c0: 7405 7c35 8301 6415 7406 6416 7407 7405  t.|5..d.t.d.t.t.
+000020d0: 7c35 8301 8301 1800 8301 1400 1700 7d35  |5............}5
+000020e0: 642d 7c00 9b00 6454 7c26 9b00 6456 7c06  d-|...dT|&..dV|.
+000020f0: 9b00 642f 7c18 9b00 6430 7c08 9b00 6431  ..d/|...d0|...d1
+00002100: 7c16 9b00 6432 7c0a 9b00 647a 7c2a 9b00  |...d2|...dz|*..
+00002110: 647b 7c27 9b00 645c 7c1c 9b00 645d 7c28  d{|'..d\|...d]|(
+00002120: 9b00 647c 7c2b 9b00 647d 7c2e 9b00 6433  ..d||+..d}|...d3
+00002130: 7c0e 9b00 645b 7c29 9b00 6435 7c0f 9b00  |...d[|)..d5|...
+00002140: 6436 7c10 9b00 647e 7c30 9b00 647f 7c31  d6|...d~|0..d.|1
+00002150: 9b00 6480 7c32 9b00 6481 7c33 9b00 6482  ..d.|2..d.|3..d.
+00002160: 7c34 9b00 6483 7c35 9b00 6464 7c25 9b00  |4..d.|5..dd|%..
+00002170: 6465 7c0b 9b00 6484 7c2f 9b00 6439 9d35  de|...d.|/..d9.5
+00002180: 7d12 740f 7c12 8301 0100 7400 7c12 643a  }.t.|.....t.|.d:
+00002190: 1700 3700 6100 5700 6e2c 0100 0100 0100  ..7.a.W.n,......
+000021a0: 642d 7c00 9b00 643b 9d03 7d12 740f 7c12  d-|...d;..}.t.|.
+000021b0: 8301 0100 7400 7c12 643a 1700 3700 6100  ....t.|.d:..7.a.
+000021c0: 5900 6e02 3000 6404 5300 2985 4e72 1300  Y.n.0.d.S.).Nr..
+000021d0: 0000 fa28 2020 2020 5b2b 5d20 5665 7269  ...(    [+] Veri
+000021e0: 6679 696e 6720 696e 7465 726e 6574 2063  fying internet c
+000021f0: 6f6e 6e65 6374 696f 6e2e 2e2e 7223 0000  onnection...r#..
+00002200: 0054 7227 0000 00fa 2820 2020 203e 2049  .Tr'....(    > I
+00002210: 6e74 6572 6e65 7420 636f 6e6e 6563 7469  nternet connecti
+00002220: 6f6e 206e 6f74 2061 7661 696c 6162 6c65  on not available
+00002230: 2172 2c00 0000 4672 2100 0000 7222 0000  !r,...Fr!...r"..
+00002240: 007a 3a20 2020 201b 5b31 3b34 393b 3933  .z:    .[1;49;93
+00002250: 6d5b 235d 2052 6576 6572 7365 2069 7020  m[#] Reverse ip 
+00002260: 6164 6472 6573 7320 6c6f 6f6b 7570 2066  address lookup f
+00002270: 6f72 201b 5b31 3b34 393b 3936 6d72 2a00  or .[1;49;96mr*.
+00002280: 0000 722b 0000 007a 245e 5c64 7b31 2c33  ..r+...z$^\d{1,3
+00002290: 7d5c 2e5c 647b 312c 337d 5c2e 5c64 7b31  }\.\d{1,3}\.\d{1
+000022a0: 2c33 7d5c 2e5c 647b 312c 337d 247a 3320  ,3}\.\d{1,3}$z3 
+000022b0: 2020 203e 2049 6e76 616c 6964 2069 7020     > Invalid ip 
+000022c0: 6164 6472 6573 7320 666f 726d 6174 2120  address format! 
+000022d0: 2845 7861 6d70 6c65 3a20 382e 382e 382e  (Example: 8.8.8.
+000022e0: 3829 722e 0000 007a 1768 7474 703a 2f2f  8)r....z.http://
+000022f0: 6970 2d61 7069 2e63 6f6d 2f6a 736f 6e2f  ip-api.com/json/
+00002300: 7a11 6874 7470 733a 2f2f 6970 6170 692e  z.https://ipapi.
+00002310: 636f 2f7a 062f 6a73 6f6e 2f7a 1068 7474  co/z./json/z.htt
+00002320: 703a 2f2f 6970 7768 6f2e 6973 2f72 3600  p://ipwho.is/r6.
+00002330: 0000 7237 0000 00fa 0a55 7365 722d 4167  ..r7.....User-Ag
+00002340: 656e 747a 444d 6f7a 696c 6c61 2f35 2e30  entzDMozilla/5.0
+00002350: 2028 5831 313b 204c 696e 7578 2078 3836   (X11; Linux x86
+00002360: 5f36 343b 2072 763a 3839 2e30 2920 4765  _64; rv:89.0) Ge
+00002370: 636b 6f2f 3230 3130 3031 3031 2046 6972  cko/20100101 Fir
+00002380: 6566 6f78 2f38 392e 3029 0372 0100 0000  efox/89.0).r....
+00002390: 7224 0000 00e9 0200 0000 7201 0000 0072  r$........r....r
+000023a0: 1400 0000 2902 7215 0000 00da 0768 6561  ....).r......hea
+000023b0: 6465 7273 e9c8 0000 00da 0673 7461 7475  ders.......statu
+000023c0: 73da 0773 7563 6365 7373 724d 0000 00da  s..successrM....
+000023d0: 0b63 6f75 6e74 7279 436f 6465 5a0a 7265  .countryCodeZ.re
+000023e0: 6769 6f6e 4e61 6d65 da06 7265 6769 6f6e  gionName..region
+000023f0: da04 6369 7479 da03 6973 70da 036f 7267  ..city..isp..org
+00002400: 721e 0000 00da 037a 6970 5a03 6c61 745a  r......zipZ.latZ
+00002410: 036c 6f6e da05 7175 6572 797a 2072 6576  .lon..queryz rev
+00002420: 6572 7365 2d69 702d 6c6f 6f6b 7570 2d73  erse-ip-lookup-s
+00002430: 6572 7665 722d 312d 6572 726f 7275 d200  erver-1-erroru..
+00002440: 0000 0a20 2020 20e2 948c e294 80e2 9480  ...    .........
 00002450: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
 00002460: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
 00002470: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00002480: e294 80e2 9480 e294 900a 2020 2020 7c20  ..........    | 
-00002490: 5363 616e 6e65 6420 4950 2041 6464 7265  Scanned IP Addre
-000024a0: 7373 3a20 1b5b 313b 3439 3b39 366d 6135  ss: .[1;49;96ma5
-000024b0: 0100 001b 5b30 6d20 2020 7c0a 2020 2020  ....[0m   |.    
-000024c0: 7c20 5365 7276 6572 2063 6f64 6520 6e61  | Server code na
-000024d0: 6d65 2020 3a20 1b5b 313b 3439 3b39 366d  me  : .[1;49;96m
-000024e0: 7265 7665 7273 652d 6970 2d6c 6f6f 6b75  reverse-ip-looku
-000024f0: 702d 7365 7276 6572 2d31 1b5b 306d 2020  p-server-1.[0m  
-00002500: 2020 2020 207c 0a20 2020 207c 2d2d 2d2d       |.    |----
-00002510: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00002520: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00002480: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00002490: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+000024a0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+000024b0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+000024c0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+000024d0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+000024e0: e294 80e2 9480 e294 80e2 9480 e294 900a  ................
+000024f0: 2020 2020 7c20 5363 616e 6e65 6420 4950      | Scanned IP
+00002500: 2041 6464 7265 7373 3a20 1b5b 313b 3439   Address: .[1;49
+00002510: 3b39 366d 7aea 1b5b 306d 2020 207c 0a20  ;96mz..[0m   |. 
+00002520: 2020 207c 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d     |------------
 00002530: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00002540: 2d2d 7c0a 2020 2020 7c20 494e 464f 524d  --|.    | INFORM
-00002550: 4154 494f 4e20 2020 2020 2020 2020 7c20  ATION         | 
-00002560: 4445 5343 5249 5054 494f 4e20 2020 2020  DESCRIPTION     
-00002570: 2020 2020 2020 2020 2020 2020 2020 207c                 |
-00002580: 0a20 2020 207c 2d2d 2d2d 2d2d 2d2d 2d2d  .    |----------
-00002590: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00002540: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00002550: 2d2d 2d2d 2d2d 2d2d 2d2d 7c0a 2020 2020  ----------|.    
+00002560: 7c20 494e 464f 524d 4154 494f 4e20 2020  | INFORMATION   
+00002570: 2020 2020 2020 7c20 4445 5343 5249 5054        | DESCRIPT
+00002580: 494f 4e20 2020 2020 2020 2020 2020 2020  ION             
+00002590: 2020 2020 2020 207c 0a20 2020 207c 2d2d         |.    |--
 000025a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000025b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 7c0a 2020  ------------|.  
-000025c0: 2020 7c20 1b5b 313b 3439 3b39 376d 436f    | .[1;49;97mCo
-000025d0: 756e 7472 791b 5b30 6d20 2020 2020 2020  untry.[0m       
-000025e0: 2020 2020 2020 7c20 7a2d 207c 0a20 2020        | z- |.   
-000025f0: 207c 201b 5b31 3b34 393b 3937 6d43 6f75   | .[1;49;97mCou
-00002600: 6e74 7279 2043 6f64 651b 5b30 6d20 2020  ntry Code.[0m   
-00002610: 2020 2020 207c 207a 2d20 7c0a 2020 2020       | z- |.    
-00002620: 7c20 1b5b 313b 3439 3b39 376d 5265 6769  | .[1;49;97mRegi
-00002630: 6f6e 1b5b 306d 2020 2020 2020 2020 2020  on.[0m          
-00002640: 2020 2020 7c20 7232 0000 007a 2d20 7c0a      | r2...z- |.
-00002650: 2020 2020 7c20 1b5b 313b 3439 3b39 376d      | .[1;49;97m
-00002660: 4369 7479 1b5b 306d 2020 2020 2020 2020  City.[0m        
-00002670: 2020 2020 2020 2020 7c20 7a6a 207c 0a20          | zj |. 
-00002680: 2020 207c 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d     |------------
-00002690: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000025b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000025c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000025d0: 2d2d 2d2d 7c0a 2020 2020 7c20 1b5b 313b  ----|.    | .[1;
+000025e0: 3439 3b39 376d 436f 756e 7472 791b 5b30  49;97mCountry.[0
+000025f0: 6d20 2020 2020 2020 2020 2020 2020 7c20  m             | 
+00002600: 7a2d 207c 0a20 2020 207c 201b 5b31 3b34  z- |.    | .[1;4
+00002610: 393b 3937 6d43 6f75 6e74 7279 2043 6f64  9;97mCountry Cod
+00002620: 651b 5b30 6d20 2020 2020 2020 207c 207a  e.[0m        | z
+00002630: 2d20 7c0a 2020 2020 7c20 1b5b 313b 3439  - |.    | .[1;49
+00002640: 3b39 376d 5265 6769 6f6e 1b5b 306d 2020  ;97mRegion.[0m  
+00002650: 2020 2020 2020 2020 2020 2020 7c20 7238              | r8
+00002660: 0000 007a 2d20 7c0a 2020 2020 7c20 1b5b  ...z- |.    | .[
+00002670: 313b 3439 3b39 376d 4369 7479 1b5b 306d  1;49;97mCity.[0m
+00002680: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002690: 7c20 7a6a 207c 0a20 2020 207c 2d2d 2d2d  | zj |.    |----
 000026a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000026b0: 2d2d 2d2d 2d2d 2d2d 2d2d 7c0a 2020 2020  ----------|.    
-000026c0: 7c20 1b5b 313b 3439 3b39 376d 506f 7374  | .[1;49;97mPost
-000026d0: 616c 2043 6f64 651b 5b30 6d20 2020 2020  al Code.[0m     
-000026e0: 2020 2020 7c20 7233 0000 007a 2d20 7c0a      | r3...z- |.
-000026f0: 2020 2020 7c20 1b5b 313b 3439 3b39 376d      | .[1;49;97m
-00002700: 4c61 7469 7475 6465 1b5b 306d 2020 2020  Latitude.[0m    
-00002710: 2020 2020 2020 2020 7c20 7a2d 207c 0a20          | z- |. 
-00002720: 2020 207c 201b 5b31 3b34 393b 3937 6d4c     | .[1;49;97mL
-00002730: 6f6e 6769 7475 6465 1b5b 306d 2020 2020  ongitude.[0m    
-00002740: 2020 2020 2020 207c 207a 6a20 7c0a 2020         | zj |.  
-00002750: 2020 7c2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d    |-------------
-00002760: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000026b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000026c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000026d0: 2d2d 7c0a 2020 2020 7c20 1b5b 313b 3439  --|.    | .[1;49
+000026e0: 3b39 376d 506f 7374 616c 2043 6f64 651b  ;97mPostal Code.
+000026f0: 5b30 6d20 2020 2020 2020 2020 7c20 7239  [0m         | r9
+00002700: 0000 007a 2d20 7c0a 2020 2020 7c20 1b5b  ...z- |.    | .[
+00002710: 313b 3439 3b39 376d 4c61 7469 7475 6465  1;49;97mLatitude
+00002720: 1b5b 306d 2020 2020 2020 2020 2020 2020  .[0m            
+00002730: 7c20 7a2d 207c 0a20 2020 207c 201b 5b31  | z- |.    | .[1
+00002740: 3b34 393b 3937 6d4c 6f6e 6769 7475 6465  ;49;97mLongitude
+00002750: 1b5b 306d 2020 2020 2020 2020 2020 207c  .[0m           |
+00002760: 207a 6a20 7c0a 2020 2020 7c2d 2d2d 2d2d   zj |.    |-----
 00002770: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00002780: 2d2d 2d2d 2d2d 2d2d 2d7c 0a20 2020 207c  ---------|.    |
-00002790: 201b 5b31 3b34 393b 3937 6d49 5350 1b5b   .[1;49;97mISP.[
-000027a0: 306d 2020 2020 2020 2020 2020 2020 2020  0m              
-000027b0: 2020 207c 207a 2d20 7c0a 2020 2020 7c20     | z- |.    | 
-000027c0: 1b5b 313b 3439 3b39 376d 4f72 671b 5b30  .[1;49;97mOrg.[0
-000027d0: 6d20 2020 2020 2020 2020 2020 2020 2020  m               
-000027e0: 2020 7c20 75b4 0000 0020 7c0a 2020 2020    | u.... |.    
-000027f0: e294 94e2 9480 e294 80e2 9480 e294 80e2  ................
-00002800: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00002780: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00002790: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000027a0: 2d7c 0a20 2020 207c 201b 5b31 3b34 393b  -|.    | .[1;49;
+000027b0: 3937 6d49 5350 1b5b 306d 2020 2020 2020  97mISP.[0m      
+000027c0: 2020 2020 2020 2020 2020 207c 207a 2d20             | z- 
+000027d0: 7c0a 2020 2020 7c20 1b5b 313b 3439 3b39  |.    | .[1;49;9
+000027e0: 376d 4f72 671b 5b30 6d20 2020 2020 2020  7mOrg.[0m       
+000027f0: 2020 2020 2020 2020 2020 7c20 f5b4 0000            | ....
+00002800: 0020 7c0a 2020 2020 e294 94e2 9480 e294  . |.    ........
 00002810: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
 00002820: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
 00002830: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
 00002840: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
 00002850: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
 00002860: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
 00002870: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
 00002880: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00002890: 9480 e294 80e2 9498 0a20 2020 2075 8d01  .........    u..
-000028a0: 0000 1b5b 306d 2020 207c 0a20 2020 207c  ...[0m   |.    |
-000028b0: 2053 6572 7665 7220 636f 6465 206e 616d   Server code nam
-000028c0: 6520 203a 201b 5b31 3b34 393b 3936 6d72  e  : .[1;49;96mr
-000028d0: 6576 6572 7365 2d69 702d 6c6f 6f6b 7570  everse-ip-lookup
-000028e0: 2d73 6572 7665 722d 311b 5b30 6d20 2020  -server-1.[0m   
-000028f0: 2020 2020 7c0a 2020 2020 7c2d 2d2d 2d2d      |.    |-----
-00002900: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00002910: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00002920: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00002930: 2d7c 0a20 2020 207c 201b 5b31 3b34 393b  -|.    | .[1;49;
-00002940: 3931 6d46 6169 6c65 6420 746f 2046 6574  91mFailed to Fet
-00002950: 6368 2069 6e66 6f72 6d61 7469 6f6e 2066  ch information f
-00002960: 726f 6d20 7468 6973 2073 6572 7665 7221  rom this server!
-00002970: 1b5b 306d 2020 2020 2020 2020 7c0a 2020  .[0m        |.  
-00002980: 2020 e294 94e2 9480 e294 80e2 9480 e294    ..............
-00002990: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-000029a0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-000029b0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-000029c0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-000029d0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-000029e0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-000029f0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00002a00: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00002a10: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00002a20: 80e2 9480 e294 80e2 9498 0a20 2020 2072  ...........    r
-00002a30: 1e00 0000 720e 0000 00da 076e 6574 776f  ....r......netwo
-00002a40: 726b da07 7665 7273 696f 6e72 4500 0000  rk..versionrE...
-00002a50: da0c 636f 756e 7472 795f 6e61 6d65 7243  ..country_namerC
-00002a60: 0000 00da 1163 6f75 6e74 7279 5f63 6f64  .....country_cod
-00002a70: 655f 6973 6f33 da0f 636f 756e 7472 795f  e_iso3..country_
-00002a80: 6361 7069 7461 6cda 0b63 6f75 6e74 7279  capital..country
-00002a90: 5f74 6c64 da0e 636f 6e74 696e 656e 745f  _tld..continent_
-00002aa0: 636f 6465 da05 696e 5f65 75da 0670 6f73  code..in_eu..pos
-00002ab0: 7461 6cda 086c 6174 6974 7564 65da 096c  tal..latitude..l
-00002ac0: 6f6e 6769 7475 6465 da0a 7574 635f 6f66  ongitude..utc_of
-00002ad0: 6673 6574 da14 636f 756e 7472 795f 6361  fset..country_ca
-00002ae0: 6c6c 696e 675f 636f 6465 da08 6375 7272  lling_code..curr
-00002af0: 656e 6379 da0d 6375 7272 656e 6379 5f6e  ency..currency_n
-00002b00: 616d 65da 096c 616e 6775 6167 6573 da0c  ame..languages..
-00002b10: 636f 756e 7472 795f 6172 6561 da12 636f  country_area..co
-00002b20: 756e 7472 795f 706f 7075 6c61 7469 6f6e  untry_population
-00002b30: da03 6173 6e7a 2072 6576 6572 7365 2d69  ..asnz reverse-i
-00002b40: 702d 6c6f 6f6b 7570 2d73 6572 7665 722d  p-lookup-server-
-00002b50: 322d 6572 726f 7261 3501 0000 1b5b 306d  2-errora5....[0m
-00002b60: 2020 207c 0a20 2020 207c 2053 6572 7665     |.    | Serve
-00002b70: 7220 636f 6465 206e 616d 6520 203a 201b  r code name  : .
-00002b80: 5b31 3b34 393b 3936 6d72 6576 6572 7365  [1;49;96mreverse
-00002b90: 2d69 702d 6c6f 6f6b 7570 2d73 6572 7665  -ip-lookup-serve
-00002ba0: 722d 321b 5b30 6d20 2020 2020 2020 7c0a  r-2.[0m       |.
-00002bb0: 2020 2020 7c2d 2d2d 2d2d 2d2d 2d2d 2d2d      |-----------
+00002890: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+000028a0: 80e2 9480 e294 80e2 9480 e294 80e2 9498  ................
+000028b0: 0a20 2020 2072 3a00 0000 7542 0100 001b  .    r:...uB....
+000028c0: 5b30 6d20 2020 7c0a 2020 2020 7c2d 2d2d  [0m   |.    |---
+000028d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000028e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000028f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00002900: 2d2d 2d7c 0a20 2020 207c 201b 5b31 3b34  ---|.    | .[1;4
+00002910: 393b 3931 6d46 6169 6c65 6420 746f 2046  9;91mFailed to F
+00002920: 6574 6368 2069 6e66 6f72 6d61 7469 6f6e  etch information
+00002930: 2066 726f 6d20 7468 6973 2073 6572 7665   from this serve
+00002940: 7221 1b5b 306d 2020 2020 2020 2020 7c0a  r!.[0m        |.
+00002950: 2020 2020 e294 94e2 9480 e294 80e2 9480      ............
+00002960: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00002970: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00002980: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00002990: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+000029a0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+000029b0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+000029c0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+000029d0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+000029e0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+000029f0: e294 80e2 9480 e294 80e2 9498 0a20 2020  .............   
+00002a00: 2072 2400 0000 720c 0000 00da 076e 6574   r$...r......net
+00002a10: 776f 726b da07 7665 7273 696f 6e72 4c00  work..versionrL.
+00002a20: 0000 da0c 636f 756e 7472 795f 6e61 6d65  ....country_name
+00002a30: 724a 0000 00da 1163 6f75 6e74 7279 5f63  rJ.....country_c
+00002a40: 6f64 655f 6973 6f33 da0f 636f 756e 7472  ode_iso3..countr
+00002a50: 795f 6361 7069 7461 6cda 0b63 6f75 6e74  y_capital..count
+00002a60: 7279 5f74 6c64 da0e 636f 6e74 696e 656e  ry_tld..continen
+00002a70: 745f 636f 6465 da05 696e 5f65 75da 0670  t_code..in_eu..p
+00002a80: 6f73 7461 6cda 086c 6174 6974 7564 65da  ostal..latitude.
+00002a90: 096c 6f6e 6769 7475 6465 da0a 7574 635f  .longitude..utc_
+00002aa0: 6f66 6673 6574 da14 636f 756e 7472 795f  offset..country_
+00002ab0: 6361 6c6c 696e 675f 636f 6465 da08 6375  calling_code..cu
+00002ac0: 7272 656e 6379 da0d 6375 7272 656e 6379  rrency..currency
+00002ad0: 5f6e 616d 65da 096c 616e 6775 6167 6573  _name..languages
+00002ae0: da0c 636f 756e 7472 795f 6172 6561 da12  ..country_area..
+00002af0: 636f 756e 7472 795f 706f 7075 6c61 7469  country_populati
+00002b00: 6f6e da03 6173 6e7a 2072 6576 6572 7365  on..asnz reverse
+00002b10: 2d69 702d 6c6f 6f6b 7570 2d73 6572 7665  -ip-lookup-serve
+00002b20: 722d 322d 6572 726f 727a ea1b 5b30 6d20  r-2-errorz..[0m 
+00002b30: 2020 7c0a 2020 2020 7c2d 2d2d 2d2d 2d2d    |.    |-------
+00002b40: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00002b50: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00002b60: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d7c  ---------------|
+00002b70: 0a20 2020 207c 2049 4e46 4f52 4d41 5449  .    | INFORMATI
+00002b80: 4f4e 2020 2020 2020 2020 207c 2044 4553  ON         | DES
+00002b90: 4352 4950 5449 4f4e 2020 2020 2020 2020  CRIPTION        
+00002ba0: 2020 2020 2020 2020 2020 2020 7c0a 2020              |.  
+00002bb0: 2020 7c2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d    |-------------
 00002bc0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00002bd0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00002be0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d7c 0a20 2020  -----------|.   
-00002bf0: 207c 2049 4e46 4f52 4d41 5449 4f4e 2020   | INFORMATION  
-00002c00: 2020 2020 2020 207c 2044 4553 4352 4950         | DESCRIP
-00002c10: 5449 4f4e 2020 2020 2020 2020 2020 2020  TION            
-00002c20: 2020 2020 2020 2020 7c0a 2020 2020 7c2d          |.    |-
-00002c30: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00002c40: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00002be0: 2d2d 2d2d 2d2d 2d2d 2d7c 0a20 2020 207c  ---------|.    |
+00002bf0: 201b 5b31 3b34 393b 3937 6d49 5020 5479   .[1;49;97mIP Ty
+00002c00: 7065 1b5b 306d 2020 2020 2020 2020 2020  pe.[0m          
+00002c10: 2020 207c 207a 2d20 7c0a 2020 2020 7c20     | z- |.    | 
+00002c20: 1b5b 313b 3439 3b39 376d 4e65 7477 6f72  .[1;49;97mNetwor
+00002c30: 6b1b 5b30 6d20 2020 2020 2020 2020 2020  k.[0m           
+00002c40: 2020 7c20 7a6a 207c 0a20 2020 207c 2d2d    | zj |.    |--
 00002c50: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00002c60: 2d2d 2d2d 2d7c 0a20 2020 207c 201b 5b31  -----|.    | .[1
-00002c70: 3b34 393b 3937 6d49 5020 5479 7065 1b5b  ;49;97mIP Type.[
-00002c80: 306d 2020 2020 2020 2020 2020 2020 207c  0m             |
-00002c90: 207a 2d20 7c0a 2020 2020 7c20 1b5b 313b   z- |.    | .[1;
-00002ca0: 3439 3b39 376d 4e65 7477 6f72 6b1b 5b30  49;97mNetwork.[0
-00002cb0: 6d20 2020 2020 2020 2020 2020 2020 7c20  m             | 
-00002cc0: 7a6a 207c 0a20 2020 207c 2d2d 2d2d 2d2d  zj |.    |------
-00002cd0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00002ce0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00002cf0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00002d00: 7c0a 2020 2020 7c20 1b5b 313b 3439 3b39  |.    | .[1;49;9
-00002d10: 376d 436f 756e 7472 791b 5b30 6d20 2020  7mCountry.[0m   
-00002d20: 2020 2020 2020 2020 2020 7c20 7a2d 207c            | z- |
-00002d30: 0a20 2020 207c 201b 5b31 3b34 393b 3937  .    | .[1;49;97
-00002d40: 6d43 6f75 6e74 7279 204e 616d 651b 5b30  mCountry Name.[0
-00002d50: 6d20 2020 2020 2020 207c 207a 2d20 7c0a  m        | z- |.
-00002d60: 2020 2020 7c20 1b5b 313b 3439 3b39 376d      | .[1;49;97m
-00002d70: 436f 756e 7472 7920 436f 6465 2049 534f  Country Code ISO
-00002d80: 331b 5b30 6d20 2020 7c20 7a2d 207c 0a20  3.[0m   | z- |. 
-00002d90: 2020 207c 201b 5b31 3b34 393b 3937 6d43     | .[1;49;97mC
-00002da0: 6f75 6e74 7279 2043 6170 6974 616c 1b5b  ountry Capital.[
-00002db0: 306d 2020 2020 207c 207a 6a20 7c0a 2020  0m     | zj |.  
-00002dc0: 2020 7c2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d    |-------------
-00002dd0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00002de0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00002df0: 2d2d 2d2d 2d2d 2d2d 2d7c 0a20 2020 207c  ---------|.    |
-00002e00: 201b 5b31 3b34 393b 3937 6d43 6f75 6e74   .[1;49;97mCount
-00002e10: 7279 2054 4c44 1b5b 306d 2020 2020 2020  ry TLD.[0m      
-00002e20: 2020 207c 207a 2d20 7c0a 2020 2020 7c20     | z- |.    | 
-00002e30: 1b5b 313b 3439 3b39 376d 4361 6c6c 696e  .[1;49;97mCallin
-00002e40: 6720 5072 6566 6978 1b5b 306d 2020 2020  g Prefix.[0m    
-00002e50: 2020 7c20 7a2d 207c 0a20 2020 207c 201b    | z- |.    | .
-00002e60: 5b31 3b34 393b 3937 6d43 6f6e 7469 6e65  [1;49;97mContine
-00002e70: 6e74 2043 6f64 651b 5b30 6d20 2020 2020  nt Code.[0m     
-00002e80: 207c 207a 2d20 7c0a 2020 2020 7c20 1b5b   | z- |.    | .[
-00002e90: 313b 3439 3b39 376d 496e 2045 551b 5b30  1;49;97mIn EU.[0
-00002ea0: 6d20 2020 2020 2020 2020 2020 2020 2020  m               
-00002eb0: 7c20 7a2d 207c 0a20 2020 207c 201b 5b31  | z- |.    | .[1
-00002ec0: 3b34 393b 3937 6d41 7070 726f 782e 2041  ;49;97mApprox. A
-00002ed0: 7265 611b 5b30 6d20 2020 2020 2020 207c  rea.[0m        |
-00002ee0: 207a 2d20 7c0a 2020 2020 7c20 1b5b 313b   z- |.    | .[1;
-00002ef0: 3439 3b39 376d 4170 7072 6f78 2e20 506f  49;97mApprox. Po
-00002f00: 7075 6c61 7469 6f6e 1b5b 306d 2020 7c20  pulation.[0m  | 
-00002f10: 7a2d 207c 0a20 2020 207c 201b 5b31 3b34  z- |.    | .[1;4
-00002f20: 393b 3937 6d4c 616e 6775 6167 6573 2053  9;97mLanguages S
-00002f30: 706f 6b65 6e1b 5b30 6d20 2020 207c 207a  poken.[0m    | z
-00002f40: 2d20 7c0a 2020 2020 7c20 1b5b 313b 3439  - |.    | .[1;49
-00002f50: 3b39 376d 4375 7272 656e 6379 1b5b 306d  ;97mCurrency.[0m
-00002f60: 2020 2020 2020 2020 2020 2020 7c20 7a2d              | z-
-00002f70: 207c 0a20 2020 207c 201b 5b31 3b34 393b   |.    | .[1;49;
-00002f80: 3937 6d43 7572 7265 6e63 7920 4e61 6d65  97mCurrency Name
-00002f90: 1b5b 306d 2020 2020 2020 207c 207a 2d20  .[0m       | z- 
-00002fa0: 7c0a 2020 2020 7c20 1b5b 313b 3439 3b39  |.    | .[1;49;9
-00002fb0: 376d 5554 4320 4f66 6673 6574 1b5b 306d  7mUTC Offset.[0m
-00002fc0: 2020 2020 2020 2020 2020 7c20 7a6a 207c            | zj |
-00002fd0: 0a20 2020 207c 2d2d 2d2d 2d2d 2d2d 2d2d  .    |----------
-00002fe0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00002ff0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00003000: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 7c0a 2020  ------------|.  
-00003010: 2020 7c20 1b5b 313b 3439 3b39 376d 4153    | .[1;49;97mAS
-00003020: 4e1b 5b30 6d20 2020 2020 2020 2020 2020  N.[0m           
-00003030: 2020 2020 2020 7c20 7a2d 207c 0a20 2020        | z- |.   
-00003040: 207c 201b 5b31 3b34 393b 3937 6d49 5350   | .[1;49;97mISP
-00003050: 1b5b 306d 2020 2020 2020 2020 2020 2020  .[0m            
-00003060: 2020 2020 207c 2075 8d01 0000 1b5b 306d       | u.....[0m
-00003070: 2020 207c 0a20 2020 207c 2053 6572 7665     |.    | Serve
-00003080: 7220 636f 6465 206e 616d 6520 203a 201b  r code name  : .
-00003090: 5b31 3b34 393b 3936 6d72 6576 6572 7365  [1;49;96mreverse
-000030a0: 2d69 702d 6c6f 6f6b 7570 2d73 6572 7665  -ip-lookup-serve
-000030b0: 722d 321b 5b30 6d20 2020 2020 2020 7c0a  r-2.[0m       |.
-000030c0: 2020 2020 7c2d 2d2d 2d2d 2d2d 2d2d 2d2d      |-----------
+00002c60: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00002c70: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00002c80: 2d2d 2d2d 7c0a 2020 2020 7c20 1b5b 313b  ----|.    | .[1;
+00002c90: 3439 3b39 376d 436f 756e 7472 791b 5b30  49;97mCountry.[0
+00002ca0: 6d20 2020 2020 2020 2020 2020 2020 7c20  m             | 
+00002cb0: 7a2d 207c 0a20 2020 207c 201b 5b31 3b34  z- |.    | .[1;4
+00002cc0: 393b 3937 6d43 6f75 6e74 7279 204e 616d  9;97mCountry Nam
+00002cd0: 651b 5b30 6d20 2020 2020 2020 207c 207a  e.[0m        | z
+00002ce0: 2d20 7c0a 2020 2020 7c20 1b5b 313b 3439  - |.    | .[1;49
+00002cf0: 3b39 376d 436f 756e 7472 7920 436f 6465  ;97mCountry Code
+00002d00: 2049 534f 331b 5b30 6d20 2020 7c20 7a2d   ISO3.[0m   | z-
+00002d10: 207c 0a20 2020 207c 201b 5b31 3b34 393b   |.    | .[1;49;
+00002d20: 3937 6d43 6f75 6e74 7279 2043 6170 6974  97mCountry Capit
+00002d30: 616c 1b5b 306d 2020 2020 207c 207a 6a20  al.[0m     | zj 
+00002d40: 7c0a 2020 2020 7c2d 2d2d 2d2d 2d2d 2d2d  |.    |---------
+00002d50: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00002d60: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00002d70: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d7c 0a20  -------------|. 
+00002d80: 2020 207c 201b 5b31 3b34 393b 3937 6d43     | .[1;49;97mC
+00002d90: 6f75 6e74 7279 2054 4c44 1b5b 306d 2020  ountry TLD.[0m  
+00002da0: 2020 2020 2020 207c 207a 2d20 7c0a 2020         | z- |.  
+00002db0: 2020 7c20 1b5b 313b 3439 3b39 376d 4361    | .[1;49;97mCa
+00002dc0: 6c6c 696e 6720 5072 6566 6978 1b5b 306d  lling Prefix.[0m
+00002dd0: 2020 2020 2020 7c20 7a2d 207c 0a20 2020        | z- |.   
+00002de0: 207c 201b 5b31 3b34 393b 3937 6d43 6f6e   | .[1;49;97mCon
+00002df0: 7469 6e65 6e74 2043 6f64 651b 5b30 6d20  tinent Code.[0m 
+00002e00: 2020 2020 207c 207a 2d20 7c0a 2020 2020       | z- |.    
+00002e10: 7c20 1b5b 313b 3439 3b39 376d 496e 2045  | .[1;49;97mIn E
+00002e20: 551b 5b30 6d20 2020 2020 2020 2020 2020  U.[0m           
+00002e30: 2020 2020 7c20 7a2d 207c 0a20 2020 207c      | z- |.    |
+00002e40: 201b 5b31 3b34 393b 3937 6d41 7070 726f   .[1;49;97mAppro
+00002e50: 782e 2041 7265 611b 5b30 6d20 2020 2020  x. Area.[0m     
+00002e60: 2020 207c 207a 2d20 7c0a 2020 2020 7c20     | z- |.    | 
+00002e70: 1b5b 313b 3439 3b39 376d 4170 7072 6f78  .[1;49;97mApprox
+00002e80: 2e20 506f 7075 6c61 7469 6f6e 1b5b 306d  . Population.[0m
+00002e90: 2020 7c20 7a2d 207c 0a20 2020 207c 201b    | z- |.    | .
+00002ea0: 5b31 3b34 393b 3937 6d4c 616e 6775 6167  [1;49;97mLanguag
+00002eb0: 6573 2053 706f 6b65 6e1b 5b30 6d20 2020  es Spoken.[0m   
+00002ec0: 207c 207a 2d20 7c0a 2020 2020 7c20 1b5b   | z- |.    | .[
+00002ed0: 313b 3439 3b39 376d 4375 7272 656e 6379  1;49;97mCurrency
+00002ee0: 1b5b 306d 2020 2020 2020 2020 2020 2020  .[0m            
+00002ef0: 7c20 7a2d 207c 0a20 2020 207c 201b 5b31  | z- |.    | .[1
+00002f00: 3b34 393b 3937 6d43 7572 7265 6e63 7920  ;49;97mCurrency 
+00002f10: 4e61 6d65 1b5b 306d 2020 2020 2020 207c  Name.[0m       |
+00002f20: 207a 2d20 7c0a 2020 2020 7c20 1b5b 313b   z- |.    | .[1;
+00002f30: 3439 3b39 376d 5554 4320 4f66 6673 6574  49;97mUTC Offset
+00002f40: 1b5b 306d 2020 2020 2020 2020 2020 7c20  .[0m          | 
+00002f50: 7a6a 207c 0a20 2020 207c 2d2d 2d2d 2d2d  zj |.    |------
+00002f60: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00002f70: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00002f80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00002f90: 7c0a 2020 2020 7c20 1b5b 313b 3439 3b39  |.    | .[1;49;9
+00002fa0: 376d 4153 4e1b 5b30 6d20 2020 2020 2020  7mASN.[0m       
+00002fb0: 2020 2020 2020 2020 2020 7c20 7a2d 207c            | z- |
+00002fc0: 0a20 2020 207c 201b 5b31 3b34 393b 3937  .    | .[1;49;97
+00002fd0: 6d49 5350 1b5b 306d 2020 2020 2020 2020  mISP.[0m        
+00002fe0: 2020 2020 2020 2020 207c 2072 5300 0000           | rS...
+00002ff0: da04 7479 7065 da09 636f 6e74 696e 656e  ..type..continen
+00003000: 74da 0569 735f 6575 da0c 6361 6c6c 696e  t..is_eu..callin
+00003010: 675f 636f 6465 da07 6361 7069 7461 6cda  g_code..capital.
+00003020: 0762 6f72 6465 7273 da04 666c 6167 5a03  .borders..flagZ.
+00003030: 696d 675a 0565 6d6f 6a69 5a0d 656d 6f6a  imgZ.emojiZ.emoj
+00003040: 695f 756e 6963 6f64 65da 0a63 6f6e 6e65  i_unicode..conne
+00003050: 6374 696f 6eda 0664 6f6d 6169 6eda 0269  ction..domain..i
+00003060: 645a 0461 6262 725a 0669 735f 6473 74da  dZ.abbrZ.is_dst.
+00003070: 066f 6666 7365 74da 0375 7463 5a0c 6375  .offset..utcZ.cu
+00003080: 7272 656e 745f 7469 6d65 7a20 7265 7665  rrent_timez reve
+00003090: 7273 652d 6970 2d6c 6f6f 6b75 702d 7365  rse-ip-lookup-se
+000030a0: 7276 6572 2d33 2d65 7272 6f72 7a6a 207c  rver-3-errorzj |
+000030b0: 0a20 2020 207c 2d2d 2d2d 2d2d 2d2d 2d2d  .    |----------
+000030c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 000030d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000030e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000030f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d7c 0a20 2020  -----------|.   
-00003100: 207c 201b 5b31 3b34 393b 3931 6d46 6169   | .[1;49;91mFai
-00003110: 6c65 6420 746f 2046 6574 6368 2069 6e66  led to Fetch inf
-00003120: 6f72 6d61 7469 6f6e 2066 726f 6d20 7468  ormation from th
-00003130: 6973 2073 6572 7665 7221 1b5b 306d 2020  is server!.[0m  
-00003140: 2020 2020 2020 7c0a 2020 2020 e294 94e2        |.    ....
-00003150: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00003160: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00003170: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00003180: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00003190: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-000031a0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-000031b0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-000031c0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-000031d0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-000031e0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-000031f0: 80e2 9498 0a20 2020 2072 4a00 0000 da04  .....    rJ.....
-00003200: 7479 7065 da09 636f 6e74 696e 656e 74da  type..continent.
-00003210: 0569 735f 6575 da0c 6361 6c6c 696e 675f  .is_eu..calling_
-00003220: 636f 6465 da07 6361 7069 7461 6cda 0762  code..capital..b
-00003230: 6f72 6465 7273 da04 666c 6167 5a03 696d  orders..flagZ.im
-00003240: 675a 0565 6d6f 6a69 5a0d 656d 6f6a 695f  gZ.emojiZ.emoji_
-00003250: 756e 6963 6f64 65da 0a63 6f6e 6e65 6374  unicode..connect
-00003260: 696f 6eda 0664 6f6d 6169 6eda 0269 645a  ion..domain..idZ
-00003270: 0461 6262 725a 0669 735f 6473 74da 066f  .abbrZ.is_dst..o
-00003280: 6666 7365 74da 0375 7463 5a0c 6375 7272  ffset..utcZ.curr
-00003290: 656e 745f 7469 6d65 7a20 7265 7665 7273  ent_timez revers
-000032a0: 652d 6970 2d6c 6f6f 6b75 702d 7365 7276  e-ip-lookup-serv
-000032b0: 6572 2d33 2d65 7272 6f72 6135 0100 001b  er-3-errora5....
-000032c0: 5b30 6d20 2020 7c0a 2020 2020 7c20 5365  [0m   |.    | Se
-000032d0: 7276 6572 2063 6f64 6520 6e61 6d65 2020  rver code name  
-000032e0: 3a20 1b5b 313b 3439 3b39 366d 7265 7665  : .[1;49;96mreve
-000032f0: 7273 652d 6970 2d6c 6f6f 6b75 702d 7365  rse-ip-lookup-se
-00003300: 7276 6572 2d33 1b5b 306d 2020 2020 2020  rver-3.[0m      
-00003310: 207c 0a20 2020 207c 2d2d 2d2d 2d2d 2d2d   |.    |--------
-00003320: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00003330: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00003340: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 7c0a  --------------|.
-00003350: 2020 2020 7c20 494e 464f 524d 4154 494f      | INFORMATIO
-00003360: 4e20 2020 2020 2020 2020 7c20 4445 5343  N         | DESC
-00003370: 5249 5054 494f 4e20 2020 2020 2020 2020  RIPTION         
-00003380: 2020 2020 2020 2020 2020 207c 0a20 2020             |.   
-00003390: 207c 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   |--------------
-000033a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000033b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000033c0: 2d2d 2d2d 2d2d 2d2d 7c0a 2020 2020 7c20  --------|.    | 
-000033d0: 1b5b 313b 3439 3b39 376d 4950 2054 7970  .[1;49;97mIP Typ
-000033e0: 651b 5b30 6d20 2020 2020 2020 2020 2020  e.[0m           
-000033f0: 2020 7c20 7a6a 207c 0a20 2020 207c 2d2d    | zj |.    |--
-00003400: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00003410: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00003420: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00003430: 2d2d 2d2d 7c0a 2020 2020 7c20 1b5b 313b  ----|.    | .[1;
-00003440: 3439 3b39 376d 436f 756e 7472 7920 4361  49;97mCountry Ca
-00003450: 7069 7461 6c1b 5b30 6d20 2020 2020 7c20  pital.[0m     | 
-00003460: 7a2d 207c 0a20 2020 207c 201b 5b31 3b34  z- |.    | .[1;4
-00003470: 393b 3937 6d43 6f6e 7469 6e65 6e74 1b5b  9;97mContinent.[
-00003480: 306d 2020 2020 2020 2020 2020 207c 207a  0m           | z
-00003490: 2d20 7c0a 2020 2020 7c20 1b5b 313b 3439  - |.    | .[1;49
-000034a0: 3b39 376d 5368 6172 696e 6720 426f 7264  ;97mSharing Bord
-000034b0: 6572 2077 6974 681b 5b30 6d20 7c20 7a2d  er with.[0m | z-
-000034c0: 207c 0a20 2020 207c 201b 5b31 3b34 393b   |.    | .[1;49;
-000034d0: 3937 6d46 6c61 6720 456d 6f6a 691b 5b30  97mFlag Emoji.[0
-000034e0: 6d20 2020 2020 2020 2020 207c 207a 6a20  m          | zj 
-000034f0: 7c0a 2020 2020 7c2d 2d2d 2d2d 2d2d 2d2d  |.    |---------
-00003500: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00003510: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00003520: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d7c 0a20  -------------|. 
-00003530: 2020 207c 201b 5b31 3b34 393b 3937 6d54     | .[1;49;97mT
-00003540: 696d 657a 6f6e 651b 5b30 6d20 2020 2020  imezone.[0m     
-00003550: 2020 2020 2020 207c 207a 2d20 7c0a 2020         | z- |.  
-00003560: 2020 7c20 1b5b 313b 3439 3b39 376d 5469    | .[1;49;97mTi
-00003570: 6d65 7a6f 6e65 2041 6262 721b 5b30 6d20  mezone Abbr.[0m 
-00003580: 2020 2020 2020 7c20 7a2d 207c 0a20 2020        | z- |.   
-00003590: 207c 201b 5b31 3b34 393b 3937 6d54 696d   | .[1;49;97mTim
-000035a0: 657a 6f6e 6520 6973 2044 5354 1b5b 306d  ezone is DST.[0m
-000035b0: 2020 2020 207c 207a 2d20 7c0a 2020 2020       | z- |.    
-000035c0: 7c20 1b5b 313b 3439 3b39 376d 5469 6d65  | .[1;49;97mTime
-000035d0: 7a6f 6e65 204f 6666 7365 741b 5b30 6d20  zone Offset.[0m 
-000035e0: 2020 2020 7c20 7a2d 207c 0a20 2020 207c      | z- |.    |
-000035f0: 201b 5b31 3b34 393b 3937 6d54 696d 657a   .[1;49;97mTimez
-00003600: 6f6e 6520 5554 431b 5b30 6d20 2020 2020  one UTC.[0m     
-00003610: 2020 207c 207a 2d20 7c0a 2020 2020 7c20     | z- |.    | 
-00003620: 1b5b 313b 3439 3b39 376d 4375 7272 656e  .[1;49;97mCurren
-00003630: 7420 5469 6d65 1b5b 306d 2020 2020 2020  t Time.[0m      
-00003640: 2020 7c20 7a2d 207c 0a20 2020 207c 201b    | z- |.    | .
-00003650: 5b31 3b34 393b 3937 6d44 6f6d 6169 6e1b  [1;49;97mDomain.
-00003660: 5b30 6d20 2020 2020 2020 2020 2020 2020  [0m             
-00003670: 207c 2075 8d01 0000 1b5b 306d 2020 207c   | u.....[0m   |
-00003680: 0a20 2020 207c 2053 6572 7665 7220 636f  .    | Server co
-00003690: 6465 206e 616d 6520 203a 201b 5b31 3b34  de name  : .[1;4
-000036a0: 393b 3936 6d72 6576 6572 7365 2d69 702d  9;96mreverse-ip-
-000036b0: 6c6f 6f6b 7570 2d73 6572 7665 722d 331b  lookup-server-3.
-000036c0: 5b30 6d20 2020 2020 2020 7c0a 2020 2020  [0m       |.    
-000036d0: 7c2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  |---------------
-000036e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000036f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00003700: 2d2d 2d2d 2d2d 2d7c 0a20 2020 207c 201b  -------|.    | .
-00003710: 5b31 3b34 393b 3931 6d46 6169 6c65 6420  [1;49;91mFailed 
-00003720: 746f 2046 6574 6368 2069 6e66 6f72 6d61  to Fetch informa
-00003730: 7469 6f6e 2066 726f 6d20 7468 6973 2073  tion from this s
-00003740: 6572 7665 7221 1b5b 306d 2020 2020 2020  erver!.[0m      
-00003750: 2020 7c0a 2020 2020 e294 94e2 9480 e294    |.    ........
-00003760: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00003770: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00003780: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00003790: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-000037a0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-000037b0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-000037c0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-000037d0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-000037e0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-000037f0: 80e2 9480 e294 80e2 9480 e294 80e2 9498  ................
-00003800: 0a20 2020 2029 1072 3600 0000 7237 0000  .    ).r6...r7..
-00003810: 0072 1700 0000 7238 0000 0072 3900 0000  .r....r8...r9...
-00003820: 723b 0000 0072 3f00 0000 7240 0000 00da  r;...r?...r@....
-00003830: 0672 616e 646f 6dda 0663 686f 6963 6572  .random..choicer
-00003840: 1200 0000 7213 0000 00da 046a 736f 6eda  ....r......json.
-00003850: 0b73 7461 7475 735f 636f 6465 da09 4578  .status_code..Ex
-00003860: 6365 7074 696f 6e72 4100 0000 2936 5a0a  ceptionrA...)6Z.
-00003870: 6970 5f61 6464 7265 7373 5a0c 6970 5f61  ip_addressZ.ip_a
-00003880: 6464 7265 7373 6573 724b 0000 005a 0a72  ddressesrK...Z.r
-00003890: 616e 646f 6d5f 6170 69da 0872 6573 706f  andom_api..respo
-000038a0: 6e73 655a 0d72 6573 706f 6e73 655f 6a73  nseZ.response_js
-000038b0: 6f6e 7246 0000 0072 4f00 0000 7250 0000  onrF...rO...rP..
-000038c0: 005a 0a72 6567 696f 6e43 6f64 6572 5100  .Z.regionCoderQ.
-000038d0: 0000 7252 0000 0072 5300 0000 7218 0000  ..rR...rS...r...
-000038e0: 0072 5e00 0000 725f 0000 0072 6000 0000  .r^...r_...r`...
-000038f0: 720e 0000 0072 4700 0000 da01 6572 5600  r....rG.....erV.
-00003900: 0000 7257 0000 0072 4500 0000 7258 0000  ..rW...rE...rX..
-00003910: 0072 4300 0000 7259 0000 0072 5a00 0000  .rC...rY...rZ...
-00003920: 725b 0000 0072 5c00 0000 725d 0000 0072  r[...r\...r]...r
-00003930: 6100 0000 7262 0000 0072 6300 0000 7264  a...rb...rc...rd
-00003940: 0000 0072 6500 0000 7266 0000 0072 6700  ...re...rf...rg.
-00003950: 0000 7268 0000 005a 0769 705f 7479 7065  ..rh...Z.ip_type
-00003960: 726a 0000 0072 6b00 0000 726c 0000 0072  rj...rk...rl...r
-00003970: 6d00 0000 726e 0000 005a 0866 6c61 675f  m...rn...Z.flag_
-00003980: 696d 675a 0a66 6c61 675f 656d 6f6a 695a  imgZ.flag_emojiZ
-00003990: 1266 6c61 675f 656d 6f6a 695f 756e 6963  .flag_emoji_unic
-000039a0: 6f64 6572 7100 0000 5a0b 7469 6d65 7a6f  oderq...Z.timezo
-000039b0: 6e65 5f69 645a 0d74 696d 657a 6f6e 655f  ne_idZ.timezone_
-000039c0: 6162 6272 5a0f 7469 6d65 7a6f 6e65 5f69  abbrZ.timezone_i
-000039d0: 735f 6473 745a 0f74 696d 657a 6f6e 655f  s_dstZ.timezone_
-000039e0: 6f66 6673 6574 5a0c 7469 6d65 7a6f 6e65  offsetZ.timezone
-000039f0: 5f75 7463 5a15 7469 6d65 7a6f 6e65 5f63  _utcZ.timezone_c
-00003a00: 7572 7265 6e74 5f74 696d 6572 1500 0000  urrent_timer....
-00003a10: 7215 0000 0072 1600 0000 da09 6970 5f6c  r....r......ip_l
-00003a20: 6f6f 6b75 70c3 0000 0073 9402 0000 0003  ookup....s......
-00003a30: 0403 1201 0801 1201 0801 0403 1a01 1403  ................
-00003a40: 0c01 1001 0801 0403 1e01 2004 04ff 0405  .......... .....
-00003a50: 0e03 0a01 0402 1401 0803 1a01 0801 0801  ................
-00003a60: 0801 0801 0801 0801 0801 0801 0801 0801  ................
-00003a70: 0801 0a02 0803 2001 2001 2001 2001 2001  ...... . . . . .
-00003a80: 2001 2001 2001 2001 2001 2001 2003 0202   . . . . . . ...
-00003a90: 02fe 0407 02f9 0408 02f8 0409 02f7 040a  ................
-00003aa0: 02f6 040b 02f5 040d 02f3 040e 02f2 040f  ................
-00003ab0: 02f1 0410 02f0 0412 02ee 0413 02ed 0816  ................
-00003ac0: 0801 1002 1001 0801 0202 02fe 0808 0801  ................
-00003ad0: 2603 0a01 0402 1401 0803 0c01 0801 0801  &...............
-00003ae0: 0801 0801 0801 0801 0801 0801 0801 0801  ................
-00003af0: 0801 0801 0801 0801 0801 0801 0801 0801  ................
-00003b00: 0801 0801 0801 0801 0801 0801 0801 0801  ................
-00003b10: 0a02 0803 2001 2001 2001 2001 2001 2001  .... . . . . . .
-00003b20: 2001 2001 2001 2001 2001 2001 2001 2001   . . . . . . . .
-00003b30: 2001 2001 2001 2001 2001 2001 2001 2001   . . . . . . . .
-00003b40: 2001 2001 2001 2001 2003 0202 02fe 0407   . . . . .......
-00003b50: 02f9 0408 02f8 040a 02f6 040b 02f5 040c  ................
-00003b60: 02f4 040d 02f3 040e 02f2 040f 02f1 0410  ................
-00003b70: 02f0 0411 02ef 0413 02ed 0414 02ec 0415  ................
-00003b80: 02eb 0416 02ea 0417 02e9 0418 02e8 0419  ................
-00003b90: 02e7 041a 02e6 041b 02e5 041d 02e3 041e  ................
-00003ba0: 02e2 041f 02e1 0420 02e0 0421 02df 0423  ....... ...!...#
-00003bb0: 02dd 0424 02dc 0827 0801 1002 0601 0202  ...$...'........
-00003bc0: 02fe 0808 0801 1603 0a01 0402 1401 0803  ................
-00003bd0: 1a01 0801 0801 0801 0801 0801 0801 0801  ................
-00003be0: 0801 0801 0801 0801 0801 0801 0801 0801  ................
-00003bf0: 0801 0c01 0c01 0c01 0c01 0c01 0c01 0c01  ................
-00003c00: 0c01 0c01 0c01 0c01 0c01 0e02 0803 2001  .............. .
-00003c10: 2001 2001 2001 2001 2001 2001 2001 2001   . . . . . . . .
-00003c20: 2001 2001 2001 2001 2001 2001 2001 2001   . . . . . . . .
-00003c30: 2001 2001 2001 2001 2001 2001 2001 2001   . . . . . . . .
-00003c40: 2001 2001 2001 2003 0202 02fe 0407 02f9   . . . .........
-00003c50: 0409 02f7 040a 02f6 040b 02f5 040c 02f4  ................
-00003c60: 040d 02f3 040f 02f1 0410 02f0 0411 02ef  ................
-00003c70: 0412 02ee 0413 02ed 0414 02ec 0416 02ea  ................
-00003c80: 0417 02e9 0418 02e8 0419 02e7 041b 02e5  ................
-00003c90: 041c 02e4 041d 02e3 041e 02e2 041f 02e1  ................
-00003ca0: 0420 02e0 0422 02de 0423 02dd 0424 02dc  . ..."...#...$..
-00003cb0: 0827 0801 1002 0601 0202 02fe 0808 0801  .'..............
-00003cc0: 1202 727c 0000 0029 0372 0100 0000 7201  ..r|...).r....r.
-00003cd0: 0000 0072 0100 0000 630c 0000 0000 0000  ...r....c.......
-00003ce0: 0000 0000 000f 0000 0008 0000 0043 0000  .............C..
-00003cf0: 0073 fc00 0000 7c09 7208 7c0a 72f8 7400  .s....|.r.|.r.t.
-00003d00: a001 a100 6a02 7d0c 7c04 721c 7403 8300  ....j.}.|.r.t...
-00003d10: 0100 7c02 722c 7403 6401 7c0c 1400 8301  ..|.r,t.d.|.....
-00003d20: 0100 7403 7c07 6402 6403 8d02 0100 7404  ..t.|.d.d.....t.
-00003d30: 7c00 8301 7c0c 6b00 72ca 7405 7c0c 7404  |...|.k.r.t.|.t.
-00003d40: 7c00 8301 1800 6404 1b00 8301 7d0d 7403  |.....d.....}.t.
-00003d50: 7c01 7c0d 1400 6402 6403 8d02 0100 7403  |.|...d.d.....t.
-00003d60: 6405 7c06 6406 1900 9b00 6407 7c06 6408  d.|.d.....d.|.d.
-00003d70: 1900 9b00 6407 7c06 6404 1900 9b00 6409  ....d.|.d.....d.
-00003d80: 9d07 6402 6403 8d02 0100 7c0b 72a2 7406  ..d.d.....|.r.t.
-00003d90: 7c00 8301 7d0e 6e10 7403 7407 7c00 8301  |...}.n.t.t.|...
-00003da0: 6402 6403 8d02 0100 7403 640a 6402 6403  d.d.....t.d.d.d.
-00003db0: 8d02 0100 7403 7c01 7c0d 1400 8301 0100  ....t.|.|.......
-00003dc0: 7403 7c08 6402 6403 8d02 0100 7c03 72e6  t.|.d.d.....|.r.
-00003dd0: 7403 6401 7c0c 1400 8301 0100 7c05 72f0  t.d.|.......|.r.
-00003de0: 7403 8300 0100 7c0b 72f8 7c0e 5300 6400  t.....|.r.|.S.d.
-00003df0: 5300 290b 4e75 0300 0000 e2b8 ba72 0f00  S.).Nu.......r..
-00003e00: 0000 2901 da03 656e 6472 4a00 0000 7a02  ..)...endrJ...z.
-00003e10: 1b5b 7201 0000 00fa 013b 721e 0000 00da  .[r......;r.....
-00003e20: 016d fa04 1b5b 306d 2908 da02 6f73 da11  .m...[0m)...os..
-00003e30: 6765 745f 7465 726d 696e 616c 5f73 697a  get_terminal_siz
-00003e40: 65da 0763 6f6c 756d 6e73 7241 0000 0072  e..columnsrA...r
-00003e50: 4000 0000 723f 0000 00da 0569 6e70 7574  @...r?.....input
-00003e60: 723b 0000 0029 0fda 0474 6578 74da 0663  r;...)...text..c
-00003e70: 656e 7465 72da 076c 696e 655f 7570 da09  enter..line_up..
-00003e80: 6c69 6e65 5f64 6f77 6eda 0873 7061 6365  line_down..space
-00003e90: 5f75 7072 2300 0000 7222 0000 00da 0f6e  _upr#...r".....n
-00003ea0: 6f72 6d61 6c74 7874 5f73 7461 7274 5a0d  ormaltxt_startZ.
-00003eb0: 6e6f 726d 616c 7478 745f 656e 645a 0468  normaltxt_endZ.h
-00003ec0: 6964 655a 0c76 6572 626f 7365 5f6d 6f64  ideZ.verbose_mod
-00003ed0: 65da 0a69 6e70 7574 5f6d 6f64 65da 0577  e..input_mode..w
-00003ee0: 6964 7468 5a09 6e65 775f 7769 6474 685a  idthZ.new_widthZ
-00003ef0: 0969 6e70 7574 5f76 6172 7215 0000 0072  .input_varr....r
-00003f00: 1500 0000 7216 0000 0072 3700 0000 3102  ....r....r7...1.
-00003f10: 0000 7322 0000 0000 0108 020a 030a 0110  ..s"............
-00003f20: 020c 020c 0114 0110 012c 010e 0110 010c  .........,......
-00003f30: 010c 020c 0210 010a 0272 3700 0000 6301  .........r7...c.
-00003f40: 0000 0000 0000 0000 0000 0008 0000 0008  ................
-00003f50: 0000 0043 0000 0073 fa00 0000 7ad4 7c00  ...C...s....z.|.
-00003f60: 6401 1700 7400 7401 a002 6402 a101 8301  d...t.t...d.....
-00003f70: 1700 6403 1700 7d01 7403 a004 a100 7d02  ..d...}.t.....}.
-00003f80: 7403 a005 a100 7d03 7c02 6404 1700 7c01  t.....}.|.d...|.
-00003f90: 1700 7d04 6405 7c01 9b00 6406 7c04 9b00  ..}.d.|...d.|...
-00003fa0: 6407 9d05 7d05 7406 7c05 8301 0100 7407  d...}.t.|.....t.
-00003fb0: 7c04 6408 8302 8f1a 7d06 7c06 a008 7409  |.d.....}.|...t.
-00003fc0: a101 0100 5700 6400 0400 0400 8303 0100  ....W.d.........
-00003fd0: 6e10 3100 737c 3000 0100 0100 0100 5900  n.1.s|0.......Y.
-00003fe0: 0100 740a 6409 6700 640a a201 640b 640b  ..t.d.g.d...d.d.
-00003ff0: 640c 8d04 0100 7c03 640d 6b02 72b6 640e  d.....|.d.k.r.d.
-00004000: 7c04 9b00 640f 7c04 9b00 6410 9d05 7d07  |...d.|...d...}.
-00004010: 6e12 6411 7c04 9b00 6412 7c04 9b00 6410  n.d.|...d.|...d.
-00004020: 9d05 7d07 7406 7c07 8301 0100 5700 640b  ..}.t.|.....W.d.
-00004030: 5300 0100 0100 0100 740a 6413 6700 6414  S.......t.d.g.d.
-00004040: a201 640b 6415 8d03 0100 5900 6416 5300  ..d.d.....Y.d.S.
-00004050: 3000 6400 5300 2917 4eda 015f 7a11 2564  0.d.S.).N.._z.%d
-00004060: 2d25 6d2d 2559 5f25 482d 254d 2d25 537a  -%m-%Y_%H-%M-%Sz
-00004070: 042e 7478 7472 3400 0000 7a2f 0a20 2020  ..txtr4...z/.   
-00004080: 201b 5b31 3b34 393b 3933 6d5b 235d 204f   .[1;49;93m[#] O
-00004090: 7574 7075 7420 4669 6c65 204e 616d 653a  utput File Name:
-000040a0: 201b 5b31 3b34 393b 3937 6d7a 331b 5b30   .[1;49;97mz3.[0
-000040b0: 6d0a 2020 2020 1b5b 313b 3439 3b39 336d  m.    .[1;49;93m
-000040c0: 5b23 5d20 4f75 7470 7574 2046 696c 6520  [#] Output File 
-000040d0: 5061 7468 3a20 1b5b 313b 3439 3b39 376d  Path: .[1;49;97m
-000040e0: 7a0d 1b5b 306d 0a20 2020 2020 2020 20da  z..[0m.        .
-000040f0: 0177 7a31 2020 2020 5b2b 5d20 4578 6375  .wz1    [+] Excu
-00004100: 7465 2066 6f6c 6c6f 7769 6e67 2063 6f6d  te following com
-00004110: 6d61 6e64 7320 746f 2076 6965 7720 6f75  mands to view ou
-00004120: 7470 7574 3a72 1d00 0000 5429 0372 2200  tput:r....T).r".
-00004130: 0000 7223 0000 0072 8900 0000 da02 6e74  ..r#...r......nt
-00004140: 7a1b 2020 2020 1b5b 313b 3439 3b39 326d  z.    .[1;49;92m
-00004150: 3e20 7368 656c 6c20 6d6f 7265 207a 201b  > shell more z .
-00004160: 5b30 6d0a 2020 2020 1b5b 313b 3439 3b39  [0m.    .[1;49;9
-00004170: 326d 3e20 7368 656c 6c20 7479 7065 2072  2m> shell type r
-00004180: 8000 0000 7a1a 2020 2020 1b5b 313b 3439  ....z.    .[1;49
-00004190: 3b39 326d 3e20 7368 656c 6c20 6361 7420  ;92m> shell cat 
-000041a0: 7a20 1b5b 306d 0a20 2020 201b 5b31 3b34  z .[0m.    .[1;4
-000041b0: 393b 3932 6d3e 2073 6865 6c6c 206c 6573  9;92m> shell les
-000041c0: 7320 7a22 2020 2020 5b21 5d20 4f75 7470  s z"    [!] Outp
-000041d0: 7574 2063 6f75 6c64 206e 6f74 2062 6520  ut could not be 
-000041e0: 7361 7665 6421 7226 0000 0072 2100 0000  saved!r&...r!...
-000041f0: 4629 0b72 3b00 0000 da04 7469 6d65 da08  F).r;.....time..
-00004200: 7374 7266 7469 6d65 7281 0000 00da 0667  strftimer......g
-00004210: 6574 6377 64da 0575 6e61 6d65 7241 0000  etcwd..unamerA..
-00004220: 00da 046f 7065 6eda 0577 7269 7465 7236  ...open..writer6
-00004230: 0000 0072 3700 0000 2908 da07 7072 765f  ...r7...)...prv_
-00004240: 636d 64da 0866 696c 656e 616d 65da 0370  cmd..filename..p
-00004250: 7764 da07 6f73 5f6e 616d 65da 0470 6174  wd..os_name..pat
-00004260: 685a 0e66 696c 655f 7361 7665 5f69 6e66  hZ.file_save_inf
-00004270: 6fda 0166 5a07 6578 655f 636d 6472 1500  o..fZ.exe_cmdr..
-00004280: 0000 7215 0000 0072 1600 0000 da0b 7361  ..r....r......sa
-00004290: 7665 5f6f 7574 7075 744c 0200 0073 2c00  ve_outputL...s,.
-000042a0: 0000 0001 0201 1a01 0801 0801 0c02 0201  ................
-000042b0: 02ff 0402 02fe 0804 0802 0c01 2802 1402  ............(...
-000042c0: 0801 1403 1202 0802 0601 0601 1201 729c  ..............r.
-000042d0: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
-000042e0: 0500 0000 0700 0000 4300 0000 7380 0000  ........C...s...
-000042f0: 007a 6064 0164 0269 017d 0074 006a 0164  .z`d.d.i.}.t.j.d
-00004300: 0374 0274 03a0 0464 0464 05a1 0283 0117  .t.t...d.d......
-00004310: 007c 0064 068d 027d 017c 016a 0564 076b  .|.d...}.|.j.d.k
-00004320: 0272 5e74 06a0 077c 016a 0864 08a1 027d  .r^t...|.j.d...}
-00004330: 027c 026a 0964 0964 0a64 0b69 0164 0c8d  .|.j.d.d.d.i.d..
-00004340: 026a 08a0 0aa1 007d 037c 0357 0053 0057  .j.....}.|.W.S.W
-00004350: 006e 0c01 0001 0001 0059 006e 0230 0067  .n.......Y.n.0.g
-00004360: 0064 0da2 017d 0474 03a0 0b7c 04a1 0153  .d...}.t...|...S
-00004370: 0029 0e4e 7249 0000 007a 444d 6f7a 696c  .).NrI...zDMozil
-00004380: 6c61 2f35 2e30 2028 5831 313b 204c 696e  la/5.0 (X11; Lin
-00004390: 7578 2078 3836 5f36 343b 2072 763a 3930  ux x86_64; rv:90
-000043a0: 2e30 2920 4765 636b 6f2f 3230 3130 3031  .0) Gecko/201001
-000043b0: 3031 2046 6972 6566 6f78 2f39 302e 307a  01 Firefox/90.0z
-000043c0: 2068 7474 7073 3a2f 2f77 7777 2e65 7870   https://www.exp
-000043d0: 6c6f 6974 2d64 622e 636f 6d2f 6768 6462  loit-db.com/ghdb
-000043e0: 2f69 e803 0000 6940 1f00 0029 0172 4b00  /i....i@...).rK.
-000043f0: 0000 724c 0000 007a 0b68 746d 6c2e 7061  ..rL...z.html.pa
-00004400: 7273 6572 5a02 6831 da05 636c 6173 737a  rserZ.h1..classz
-00004410: 0a63 6172 642d 7469 746c 6529 01da 0561  .card-title)...a
-00004420: 7474 7273 2916 7a1d 7369 7465 3a64 6f6d  ttrs).z.site:dom
-00004430: 6169 6e2e 636f 6d20 6669 6c65 7479 7065  ain.com filetype
-00004440: 3a20 7064 667a 0f69 6e75 726c 3a20 7061  : pdfz.inurl: pa
-00004450: 7373 776f 7264 7515 0000 0069 6e74 6578  sswordu....intex
-00004460: 743a e280 9d75 7365 726e 616d 65e2 809d  t:...username...
-00004470: 7a0c 6669 6c65 7479 7065 3a78 6c73 751b  z.filetype:xlsu.
-00004480: 0000 0066 696c 6574 7970 653a 7478 7420  ...filetype:txt 
-00004490: e280 9c75 7365 726e 616d 65e2 809d 7548  ...username...uH
-000044a0: 0000 0066 696c 6574 7970 653a 6c6f 6720  ...filetype:log 
-000044b0: e280 9c50 4850 2050 6172 7365 2065 7272  ...PHP Parse err
-000044c0: 6f72 e280 9d20 7c20 e280 9c50 4850 2057  or... | ...PHP W
-000044d0: 6172 6e69 6e67 e280 9d20 7c20 e280 9c50  arning... | ...P
-000044e0: 4850 2045 7272 6f72 e280 9d75 1700 0000  HP Error...u....
-000044f0: 696e 7469 746c 653a 20e2 809c 696e 6465  intitle: ...inde
-00004500: 7820 6f66 e280 9d75 2200 0000 696e 7469  x of...u"...inti
-00004510: 746c 653a 20e2 809c 696e 6465 7820 6f66  tle: ...index of
-00004520: e280 9d20 e280 9c2e 6769 74e2 809d 7522  ... ....git...u"
-00004530: 0000 0069 6e74 6974 6c65 3a20 e280 9c69  ...intitle: ...i
-00004540: 6e64 6578 206f 66e2 809d 20e2 809c 2e73  ndex of... ....s
-00004550: 766e e280 9d75 1900 0000 696e 7572 6c3a  vn...u....inurl:
-00004560: e280 9d76 6965 7765 7266 7261 6d65 3f6d  ...viewerframe?m
-00004570: 6f64 6575 2800 0000 696e 7572 6c3a e280  odeu(...inurl:..
-00004580: 9d4d 756c 7469 4361 6d65 7261 4672 616d  .MultiCameraFram
-00004590: 653f 4d6f 6465 3d4d 6f74 696f 6ee2 809d  e?Mode=Motion...
-000045a0: 752b 0000 0069 6e74 6974 6c65 3a20 e280  u+...intitle: ..
-000045b0: 9c69 6e64 6578 206f 66e2 809d 20e2 809c  .index of... ...
-000045c0: 2e62 6173 685f 6869 7374 6f72 79e2 809d  .bash_history...
-000045d0: 751b 0000 0069 6e74 6578 743a 20e2 809c  u....intext: ...
-000045e0: 4c61 7374 206d 6f64 6966 6965 64e2 809d  Last modified...
-000045f0: 7518 0000 0069 6e74 6578 743a 20e2 809c  u....intext: ...
-00004600: 496e 6465 7820 6f66 202f e280 9d75 1e00  Index of /...u..
-00004610: 0000 696e 7465 7874 3a20 e280 9c50 6172  ..intext: ...Par
-00004620: 656e 7420 4469 7265 6374 6f72 79e2 809d  ent Directory...
-00004630: 7512 0000 0069 6e75 726c 3a20 e280 9c61  u....inurl: ...a
-00004640: 646d 696e e280 9d75 1200 0000 696e 7572  dmin...u....inur
-00004650: 6c3a 20e2 809c 6c6f 6769 6ee2 809d 751e  l: ...login...u.
-00004660: 0000 0069 6e75 726c 3a20 e280 9c6c 6f67  ...inurl: ...log
-00004670: 696e e280 9d20 e280 9c61 646d 696e e280  in... ...admin..
-00004680: 9d75 2900 0000 696e 7572 6c3a 20e2 809c  .u)...inurl: ...
-00004690: 6c6f 6769 6ee2 809d 20e2 809c 6164 6d69  login... ...admi
-000046a0: 6ee2 809d 20e2 809c 7573 6572 e280 9d75  n... ...user...u
-000046b0: 1b00 0000 696e 7465 7874 3ae2 809d 7072  ....intext:...pr
-000046c0: 6976 6163 7920 706f 6c69 6379 e280 9d7a  ivacy policy...z
-000046d0: 2222 7061 7373 776f 7264 732e 7478 7422  ""passwords.txt"
-000046e0: 2069 6e74 6974 6c65 3a22 496e 6465 7820   intitle:"Index 
-000046f0: 6f66 2275 1700 0000 696e 7465 7874 3ae2  of"u....intext:.
-00004700: 809d 4067 6d61 696c 2e63 6f6d e280 9d29  ..@gmail.com...)
-00004710: 0c72 1200 0000 7213 0000 0072 3b00 0000  .r....r....r;...
-00004720: 7275 0000 00da 0772 616e 6469 6e74 7278  ru.....randintrx
-00004730: 0000 00da 0362 7334 5a0d 4265 6175 7469  .....bs4Z.Beauti
-00004740: 6675 6c53 6f75 7072 8500 0000 da04 6669  fulSoupr......fi
-00004750: 6e64 723d 0000 0072 7600 0000 2905 724b  ndr=...rv...).rK
-00004760: 0000 00da 0a64 6f72 6b5f 7175 6572 795a  .....dork_queryZ
-00004770: 0b70 6172 7365 645f 6874 6d6c 7255 0000  .parsed_htmlrU..
-00004780: 005a 106c 6f63 616c 5f64 6f72 6b5f 7175  .Z.local_dork_qu
-00004790: 6572 7972 1500 0000 7215 0000 0072 1600  eryr....r....r..
-000047a0: 0000 72a2 0000 006b 0200 0073 1600 0000  ..r....k...s....
-000047b0: 0002 0201 0801 1e03 0a02 0e03 1802 0a01  ................
-000047c0: 0601 0603 0807 72a2 0000 0063 0000 0000  ......r....c....
-000047d0: 0000 0000 0000 0000 0000 0000 0900 0000  ................
-000047e0: 4300 0000 739a 0000 0074 00a0 0174 006a  C...s....t...t.j
-000047f0: 0264 016b 0272 1264 026e 0264 03a1 0101  .d.k.r.d.n.d....
-00004800: 0074 0364 0464 0564 0664 0774 04a0 0567  .t.d.d.d.d.t...g
-00004810: 0064 08a2 01a1 0167 0364 0964 0a8d 0401  .d.....g.d.d....
-00004820: 0074 0364 0b64 0564 0664 0774 04a0 0567  .t.d.d.d.d.t...g
-00004830: 0064 08a2 01a1 0167 0364 0c8d 0301 0074  .d.....g.d.....t
-00004840: 0364 0d64 0564 0664 0774 04a0 0567 0064  .d.d.d.d.t...g.d
-00004850: 08a2 01a1 0167 0364 0964 0e8d 0401 0074  .....g.d.d.....t
-00004860: 0364 0f64 0564 0664 0774 04a0 0567 0064  .d.d.d.d.t...g.d
-00004870: 08a2 01a1 0167 0364 0964 0e8d 0401 0064  .....g.d.d.....d
-00004880: 0053 0029 104e 728f 0000 00da 0363 6c73  .S.).Nr......cls
-00004890: 7208 0000 0075 7700 0000 e294 8020 e296  r....uw...... ..
-000048a0: 92e2 9688 e296 80e2 9680 e296 8820 e296  ............. ..
-000048b0: 92e2 9688 e296 91e2 9692 e296 8820 e296  ............. ..
-000048c0: 88e2 9680 e296 80e2 9688 20e2 9692 e296  .......... .....
-000048d0: 88e2 9680 e296 84e2 9680 e296 8820 e296  ............. ..
-000048e0: 92e2 9688 e296 80e2 9680 e296 8820 e296  ............. ..
-000048f0: 92e2 9688 e296 80e2 9680 e296 8020 e296  ............. ..
-00004900: 92e2 9688 e296 80e2 9680 e296 8820 e294  ............. ..
-00004910: 8072 3000 0000 721e 0000 0072 1f00 0000  .r0...r....r....
-00004920: 2907 7227 0000 00e9 5c00 0000 7220 0000  ).r'....\...r ..
-00004930: 00e9 5e00 0000 e95f 0000 00e9 6000 0000  ..^...._....`...
-00004940: e961 0000 0054 2903 7286 0000 0072 2200  .a...T).r....r".
-00004950: 0000 7289 0000 0075 7700 0000 e294 8020  ..r....uw...... 
-00004960: e296 92e2 9688 e296 84e2 9684 e296 8820  ............... 
-00004970: e296 92e2 9688 e296 80e2 9680 e296 8820  ............... 
-00004980: e296 88e2 9684 e296 80e2 9688 20e2 9692  ............ ...
-00004990: e296 88e2 9692 e296 88e2 9692 e296 8820  ............... 
-000049a0: e296 92e2 9688 e296 80e2 9680 e296 8420  ............... 
-000049b0: e296 92e2 9688 e296 80e2 9680 e296 8020  ............... 
-000049c0: e296 92e2 9688 e296 84e2 9684 e296 8020  ............... 
-000049d0: e294 8029 0272 8600 0000 7222 0000 0075  ...).r....r"...u
-000049e0: 7700 0000 e294 8020 e296 92e2 9688 e296  w...... ........
-000049f0: 91e2 9691 e296 9120 e296 92e2 9688 e296  ....... ........
-00004a00: 91e2 9692 e296 8820 e296 88e2 9684 e296  ....... ........
-00004a10: 84e2 9688 20e2 9692 e296 88e2 9691 e296  .... ...........
-00004a20: 91e2 9692 e296 8820 e296 92e2 9688 e296  ....... ........
-00004a30: 84e2 9684 e296 8820 e296 92e2 9688 e296  ....... ........
-00004a40: 84e2 9684 e296 8420 e296 92e2 9688 e296  ....... ........
-00004a50: 91e2 9692 e296 8820 e294 8029 0372 8600  ....... ...).r..
-00004a60: 0000 7222 0000 0072 2300 0000 7a29 4f53  ..r"...r#...z)OS
-00004a70: 494e 542d 4652 414d 4557 4f52 4b20 2020  INT-FRAMEWORK   
-00004a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004a90: 4073 3431 7234 6a29 0672 8100 0000 da06  @s41r4j).r......
-00004aa0: 7379 7374 656d da04 6e61 6d65 7237 0000  system..namer7..
-00004ab0: 0072 7500 0000 7276 0000 0072 1500 0000  .ru...rv...r....
-00004ac0: 7215 0000 0072 1500 0000 7216 0000 00da  r....r....r.....
-00004ad0: 046c 6f67 6f87 0200 0073 0a00 0000 0002  .logo....s......
-00004ae0: 1803 2001 1e01 2001 72ab 0000 0063 0200  .. ... .r....c..
-00004af0: 0000 0000 0000 0000 0000 0400 0000 0300  ................
-00004b00: 0000 0300 0000 7332 0000 0074 007d 0287  ......s2...t.}..
-00004b10: 0066 0164 0164 0284 087c 0244 0083 017d  .f.d.d...|.D...}
-00004b20: 037c 0174 017c 0383 016b 0072 2a7c 037c  .|.t.|...k.r*|.|
-00004b30: 0119 0053 0064 0053 0064 0053 0029 034e  ...S.d.S.d.S.).N
-00004b40: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
-00004b50: 0005 0000 0013 0000 0073 1a00 0000 6700  .........s....g.
-00004b60: 7c00 5d12 7d01 7c01 a000 8800 a101 7204  |.].}.|.......r.
-00004b70: 7c01 9102 7104 5300 7215 0000 0029 01da  |...q.S.r....)..
-00004b80: 0a73 7461 7274 7377 6974 6829 02da 022e  .startswith)....
-00004b90: 30da 0169 a901 7285 0000 0072 1500 0000  0..i..r....r....
-00004ba0: 7216 0000 00da 0a3c 6c69 7374 636f 6d70  r......<listcomp
-00004bb0: 3e93 0200 00f3 0000 0000 7a1d 636f 6d70  >.........z.comp
-00004bc0: 6c65 7465 722e 3c6c 6f63 616c 733e 2e3c  leter.<locals>.<
-00004bd0: 6c69 7374 636f 6d70 3e29 02da 1261 7661  listcomp>)...ava
-00004be0: 6c69 6162 6c65 5f63 6f6d 6d61 6e64 7372  liable_commandsr
-00004bf0: 4000 0000 2904 7285 0000 00da 0573 7461  @...).r......sta
-00004c00: 7465 da08 636f 6d6d 616e 6473 da07 6f70  te..commands..op
-00004c10: 7469 6f6e 7372 1500 0000 72af 0000 0072  tionsr....r....r
-00004c20: 1600 0000 da09 636f 6d70 6c65 7465 7291  ......completer.
-00004c30: 0200 0073 0a00 0000 0001 0401 1201 0c01  ...s............
-00004c40: 0802 72b6 0000 0063 0000 0000 0000 0000  ..r....c........
-00004c50: 0000 0000 2000 0000 0f00 0000 4300 0000  .... .......C...
-00004c60: 73f0 0900 0074 0073 2674 0164 0164 0264  s....t.s&t.d.d.d
-00004c70: 0374 02a0 0367 0064 04a2 01a1 0167 0364  .t...g.d.....g.d
-00004c80: 0564 0564 0564 068d 0501 0067 0064 07a2  .d.d.d.....g.d..
-00004c90: 017d 007c 0064 0819 007d 0164 097d 0264  .}.|.d...}.d.}.d
-00004ca0: 0a74 0474 05a0 06a1 0083 0117 0064 0b17  .t.t.........d..
-00004cb0: 0064 0c74 0764 0d74 0874 0474 05a0 06a1  .d.t.d.t.t.t....
-00004cc0: 0083 0183 0118 0083 0114 0017 007d 0364  .............}.d
-00004cd0: 0a74 0474 05a0 09a1 006a 0a83 0117 0064  .t.t.....j.....d
-00004ce0: 0b17 0064 0c74 0764 0d74 0874 0474 05a0  ...d.t.d.t.t.t..
-00004cf0: 09a1 006a 0a83 0183 0118 0083 0114 0017  ...j............
-00004d00: 007d 0464 0a74 0474 05a0 09a1 006a 0b83  .}.d.t.t.....j..
-00004d10: 0117 0064 0b17 0064 0c74 0764 0d74 0874  ...d...d.t.d.t.t
-00004d20: 0474 05a0 09a1 006a 0b83 0183 0118 0083  .t.....j........
-00004d30: 0114 0017 007d 0564 0a74 0474 0ca0 0da1  .....}.d.t.t....
-00004d40: 006a 0e83 0117 0064 0e17 0064 0b17 0064  .j.....d...d...d
-00004d50: 0c74 0764 0f74 0874 0474 0ca0 0da1 006a  .t.d.t.t.t.....j
-00004d60: 0e83 0183 0118 0083 0114 0017 007d 0664  .............}.d
-00004d70: 0a74 0474 0ca0 0fa1 0083 0117 0064 0e17  .t.t.........d..
-00004d80: 0064 0b17 0064 0c74 0764 1074 0874 0474  .d...d.t.d.t.t.t
-00004d90: 0ca0 0fa1 0083 0183 0118 0083 0114 0017  ................
-00004da0: 007d 0764 0a74 0474 0ca0 1064 11a1 016a  .}.d.t.t...d...j
-00004db0: 0e83 0117 0064 0e17 0064 0b17 0064 0c74  .....d...d...d.t
-00004dc0: 0764 0f74 0874 0474 0ca0 1064 11a1 016a  .d.t.t.t...d...j
-00004dd0: 0e83 0183 0118 0083 0114 0017 007d 0864  .............}.d
-00004de0: 1264 0c74 0764 0d74 0874 0464 1383 0183  .d.t.d.t.t.d....
-00004df0: 0118 0083 0114 0017 007d 0964 147c 039b  .........}.d.|..
-00004e00: 0064 157c 049b 0064 167c 059b 0064 177c  .d.|...d.|...d.|
-00004e10: 069b 0064 187c 079b 0064 197c 089b 0064  ...d.|...d.|...d
-00004e20: 1a7c 099b 0064 1b9d 0f7d 0a64 1c7d 0b64  .|...d...}.d.}.d
-00004e30: 1d7d 0c74 11a0 1264 1ea1 0101 0074 11a0  .}.t...d.....t..
-00004e40: 1374 14a1 0101 0064 1f64 2067 027d 0d7c  .t.....d.d g.}.|
-00004e50: 0d64 0219 007d 0e74 0164 217c 03a0 15a1  .d...}.t.d!|....
-00004e60: 009b 0064 227c 019b 0064 237c 0e9b 009d  ...d"|...d#|....
-00004e70: 0664 0564 0564 248d 03a0 15a1 007d 0f7c  .d.d.d$......}.|
-00004e80: 0f64 256b 0290 0272 3c7c 0064 0219 007d  .d%k...r<|.d...}
-00004e90: 0164 1d61 1674 177c 0b83 0101 0090 076e  .d.a.t.|.......n
-00004ea0: a87c 0f64 0064 2685 0219 0064 256b 0290  .|.d.d&....d%k..
-00004eb0: 0472 707c 0f64 2717 0064 2619 0064 0c6b  .rp|.d'..d&..d.k
-00004ec0: 0290 0472 507c 0f64 2864 0085 0219 007d  ...rP|.d(d.....}
-00004ed0: 0f7c 0f64 256b 0290 0272 8e7c 0064 0219  .|.d%k...r.|.d..
-00004ee0: 007d 0164 297d 1074 177c 1083 0101 0090  .}.d)}.t.|......
-00004ef0: 0471 687c 0f64 2a6b 0290 0273 a27c 0f64  .qh|.d*k...s.|.d
-00004f00: 2b6b 0290 0272 ba7c 0064 0219 007d 0164  +k...r.|.d...}.d
-00004f10: 2c7d 1174 177c 1183 0101 0090 0471 687c  ,}.t.|.......qh|
-00004f20: 0f64 2d6b 0290 0272 dc7c 0064 0219 007d  .d-k...r.|.d...}
-00004f30: 0164 2e7d 1274 177c 1283 0101 0090 0471  .d.}.t.|.......q
-00004f40: 687c 0f64 2f6b 0290 0272 fe7c 0064 0219  h|.d/k...r.|.d..
-00004f50: 007d 0164 307d 1374 177c 1383 0101 0090  .}.d0}.t.|......
-00004f60: 0471 687c 0f64 316b 0290 0372 207c 0064  .qh|.d1k...r |.d
-00004f70: 0219 007d 0164 327d 1474 177c 1483 0101  ...}.d2}.t.|....
-00004f80: 0090 0471 687c 0f64 336b 0290 0372 427c  ...qh|.d3k...rB|
-00004f90: 0064 0219 007d 0164 347d 1574 177c 1583  .d...}.d4}.t.|..
-00004fa0: 0101 0090 0471 687c 0f64 356b 0290 0372  .....qh|.d5k...r
-00004fb0: 627c 0064 0219 007d 0164 367d 1674 177c  b|.d...}.d6}.t.|
-00004fc0: 1683 0101 006e ec7c 0f64 0064 2885 0219  .....n.|.d.d(...
-00004fd0: 0064 376b 0290 0372 8a7c 0064 0219 007d  .d7k...r.|.d...}
-00004fe0: 0164 387d 1774 177c 1783 0101 006e c47c  .d8}.t.|.....n.|
-00004ff0: 0f64 396b 0290 0372 aa7c 0064 0219 007d  .d9k...r.|.d...}
-00005000: 0164 3a7d 1874 177c 1883 0101 006e a47c  .d:}.t.|.....n.|
-00005010: 0f64 3b6b 0290 0372 ca7c 0064 0219 007d  .d;k...r.|.d...}
-00005020: 0164 3c7d 1974 177c 1983 0101 006e 847c  .d<}.t.|.....n.|
-00005030: 0f64 3d6b 0290 0372 ea7c 0064 0219 007d  .d=k...r.|.d...}
-00005040: 0164 3e7d 1a74 177c 1a83 0101 006e 647c  .d>}.t.|.....nd|
-00005050: 0f64 3f6b 0290 0472 167c 0064 0219 007d  .d?k...r.|.d...}
-00005060: 0164 407c 03a0 15a1 009b 0064 419d 037d  .d@|.......dA..}
-00005070: 1b74 177c 1b83 0101 006e 387c 0f64 426b  .t.|.....n8|.dBk
-00005080: 0290 0472 367c 0064 0219 007d 0164 437d  ...r6|.d...}.dC}
-00005090: 1c74 177c 1c83 0101 006e 187c 0064 4419  .t.|.....n.|.dD.
-000050a0: 007d 0174 0164 4567 0064 46a2 0164 478d  .}.t.dEg.dF..dG.
-000050b0: 0201 006e 187c 0064 4419 007d 0174 0164  ...n.|.dD..}.t.d
-000050c0: 4867 0064 46a2 0164 478d 0201 0064 1d61  Hg.dF..dG....d.a
-000050d0: 1690 056e 747c 0f64 2a6b 0290 0473 847c  ...nt|.d*k...s.|
-000050e0: 0f64 2b6b 0290 0472 a874 0164 4964 0264  .d+k...r.t.dId.d
-000050f0: 0374 02a0 0367 0064 04a2 01a1 0167 0364  .t...g.d.....g.d
-00005100: 478d 0201 0074 1882 0190 056e 3c7c 0f64  G....t.....n<|.d
-00005110: 2d6b 0290 0472 ea7c 0064 0219 007d 0164  -k...r.|.d...}.d
-00005120: 1d61 1674 0164 4a67 0064 4ba2 0164 0564  .a.t.dJg.dK..d.d
-00005130: 4c8d 0301 0074 0164 4d74 1983 0017 0067  L....t.dMt.....g
-00005140: 0064 4ea2 0164 478d 0201 0090 046e fa7c  .dN..dG......n.|
-00005150: 0f64 2f6b 0290 0572 0c7c 0064 0219 007d  .d/k...r.|.d...}
-00005160: 0164 1d61 1674 177c 0283 0101 0090 046e  .d.a.t.|.......n
-00005170: d87c 0f64 316b 0290 0672 0c74 0164 4f67  .|.d1k...r.t.dOg
-00005180: 0064 4ba2 0164 0564 4c8d 0301 007a a674  .dK..d.dL....z.t
-00005190: 1aa0 1b64 50a1 0101 0074 0164 5167 0064  ...dP....t.dQg.d
-000051a0: 4ea2 0164 478d 0201 007a 1674 1aa0 1b64  N..dG....z.t...d
-000051b0: 52a1 01a0 1ca1 0064 5319 007d 1d57 006e  R......dS..}.W.n
-000051c0: 4c01 0001 0001 007a 1074 1aa0 1b64 54a1  L......z.t...dT.
-000051d0: 016a 1d7d 1d57 006e 2e01 0001 0001 007a  .j.}.W.n.......z
-000051e0: 1074 1aa0 1b64 55a1 016a 1d7d 1d57 006e  .t...dU..j.}.W.n
-000051f0: 1001 0001 0001 0064 567d 1d59 006e 0230  .......dV}.Y.n.0
-00005200: 0059 006e 0230 0059 006e 0230 007c 1d90  .Y.n.0.Y.n.0.|..
-00005210: 0572 c474 0164 577c 1d9b 009d 0267 0064  .r.t.dW|.....g.d
-00005220: 4ea2 0164 478d 0201 007c 0064 0819 007d  N..dG....|.d...}
-00005230: 0157 006e 3401 0001 0001 0074 0164 5867  .W.n4......t.dXg
-00005240: 0064 46a2 0164 478d 0201 0074 0164 5967  .dF..dG....t.dYg
-00005250: 0064 4ea2 0164 478d 0201 007c 0064 4419  .dN..dG....|.dD.
-00005260: 007d 0159 006e 0230 0064 1d61 1690 036e  .}.Y.n.0.d.a...n
-00005270: d87c 0f64 336b 0290 0672 407c 0064 0819  .|.d3k...r@|.d..
-00005280: 007d 0164 1d61 1674 05a0 1e74 056a 1f64  .}.d.a.t...t.j.d
-00005290: 5a6b 0290 0672 3664 5b6e 0264 33a1 0101  Zk...r6d[n.d3...
-000052a0: 0090 036e a47c 0f64 356b 0290 0672 a474  ...n.|.d5k...r.t
-000052b0: 0164 5c67 0064 4ba2 0164 0564 4c8d 0301  .d\g.dK..d.dL...
-000052c0: 0074 1664 1d6b 0290 0672 8074 0164 5d67  .t.d.k...r.t.d]g
-000052d0: 0064 46a2 0164 478d 0201 007c 0064 5e19  .dF..dG....|.d^.
-000052e0: 007d 016e 1c74 207c 0c83 0190 0672 947c  .}.n.t |.....r.|
-000052f0: 0064 0819 007d 016e 087c 0064 4419 007d  .d...}.n.|.dD..}
-00005300: 0164 1d61 1690 036e 407c 0f64 376b 0290  .d.a...n@|.d7k..
-00005310: 0672 ce7c 0064 5e19 007d 0164 1d61 1674  .r.|.d^..}.d.a.t
-00005320: 0164 5f67 0064 46a2 0164 478d 0201 0090  .d_g.dF..dG.....
-00005330: 036e 167c 0f64 0064 2885 0219 0064 376b  .n.|.d.d(....d7k
-00005340: 0290 0772 807c 0f64 2717 0064 2819 0064  ...r.|.d'..d(..d
-00005350: 0c6b 0290 0772 607c 0f64 6064 0085 0219  .k...r`|.d`d....
-00005360: 007d 0f64 6174 047c 0f83 019b 0064 629d  .}.dat.|.....db.
-00005370: 037d 1e74 177c 1e83 0101 0074 05a0 1e7c  .}.t.|.....t...|
-00005380: 0fa1 017d 1f7c 1f64 086b 0290 0772 4674  ...}.|.d.k...rFt
-00005390: 0164 6367 0064 64a2 0164 6564 668d 0301  .dcg.dd..dedf...
-000053a0: 007c 0064 0819 007d 016e 1874 0164 6767  .|.d...}.n.t.dgg
-000053b0: 0064 46a2 0164 478d 0201 007c 0064 4419  .dF..dG....|.dD.
-000053c0: 007d 016e 187c 0064 4419 007d 0174 0164  .}.n.|.dD..}.t.d
-000053d0: 4867 0064 46a2 0164 478d 0201 0064 1d61  Hg.dF..dG....d.a
-000053e0: 1690 026e 647c 0f64 396b 0290 0772 a27c  ...nd|.d9k...r.|
-000053f0: 0064 0219 007d 0164 1d61 1674 177c 0a83  .d...}.d.a.t.|..
-00005400: 0101 0090 026e 427c 0f64 3b6b 0290 0772  .....nB|.d;k...r
-00005410: cc7c 0064 5e19 007d 0164 1d61 1674 0164  .|.d^..}.d.a.t.d
-00005420: 6867 0064 46a2 0164 478d 0201 0090 026e  hg.dF..dG......n
-00005430: 187c 0f64 0064 6085 0219 0064 3b6b 0290  .|.d.d`....d;k..
-00005440: 0872 8e7c 0f64 2717 0064 6019 0064 0c6b  .r.|.d'..d`..d.k
-00005450: 0290 0872 6e7c 0f64 6964 0085 0219 007d  ...rn|.did.....}
-00005460: 0f7c 0f64 6a6b 0290 0872 287c 0d64 0819  .|.djk...r(|.d..
-00005470: 007d 0e7c 0064 0819 007d 0174 0164 6b67  .}.|.d...}.t.dkg
-00005480: 0064 4ea2 0164 478d 0201 006e 447c 0f64  .dN..dG....nD|.d
-00005490: 6c6b 0290 0872 547c 0d64 0219 007d 0e7c  lk...rT|.d...}.|
-000054a0: 0064 0819 007d 0174 0164 6d67 0064 4ea2  .d...}.t.dmg.dN.
-000054b0: 0164 478d 0201 006e 187c 0064 4419 007d  .dG....n.|.dD..}
-000054c0: 0174 0164 6e67 0064 46a2 0164 478d 0201  .t.dng.dF..dG...
-000054d0: 006e 187c 0064 4419 007d 0174 0164 4867  .n.|.dD..}.t.dHg
-000054e0: 0064 46a2 0164 478d 0201 0064 1d61 1690  .dF..dG....d.a..
-000054f0: 016e 567c 0f64 3d6b 0290 0872 b47c 0064  .nV|.d=k...r.|.d
-00005500: 5e19 007d 0174 0164 6f67 0064 46a2 0164  ^..}.t.dog.dF..d
-00005510: 478d 0201 0090 016e 307c 0f64 0064 6085  G......n0|.d.d`.
-00005520: 0219 0064 3d6b 0290 0972 2e7c 0f64 2717  ...d=k...r.|.d'.
-00005530: 0064 6019 0064 0c6b 0290 0972 147c 0f64  .d`..d.k...r.|.d
-00005540: 6964 0085 0219 007d 0f74 0164 7067 0064  id.....}.t.dpg.d
-00005550: 4ba2 0164 0564 4c8d 0301 0074 217c 0f83  K..d.dL....t!|..
-00005560: 0190 0972 0a7c 0064 2619 007d 016e 087c  ...r.|.d&..}.n.|
-00005570: 0064 4419 007d 016e 187c 0064 4419 007d  .dD..}.n.|.dD..}
-00005580: 0174 0164 4867 0064 46a2 0164 478d 0201  .t.dHg.dF..dG...
-00005590: 006e b67c 0f64 426b 0290 0972 527c 0064  .n.|.dBk...rR|.d
-000055a0: 5e19 007d 0174 0164 7167 0064 46a2 0164  ^..}.t.dqg.dF..d
-000055b0: 478d 0201 006e 927c 0f64 0064 5e85 0219  G....n.|.d.d^...
-000055c0: 0064 426b 0290 0972 cc7c 0f64 2717 0064  .dBk...r.|.d'..d
-000055d0: 5e19 0064 0c6b 0290 0972 b27c 0f64 4464  ^..d.k...r.|.dDd
-000055e0: 0085 0219 007d 0f74 0164 7267 0064 4ba2  .....}.t.drg.dK.
-000055f0: 0164 0564 4c8d 0301 0074 227c 0f83 0190  .d.dL....t"|....
-00005600: 0972 a87c 0064 2619 007d 016e 087c 0064  .r.|.d&..}.n.|.d
-00005610: 4419 007d 016e 187c 0064 4419 007d 0174  D..}.n.|.dD..}.t
-00005620: 0164 4867 0064 46a2 0164 478d 0201 006e  .dHg.dF..dG....n
-00005630: 187c 0064 4419 007d 0174 0164 4867 0064  .|.dD..}.t.dHg.d
-00005640: 46a2 0164 478d 0201 007c 0f7d 0c90 0171  F..dG....|.}...q
-00005650: f264 0053 0029 734e 7a27 5b23 5d20 496e  .d.S.)sNz'[#] In
-00005660: 6974 6961 6c69 7a69 6e67 2060 5048 304d  itializing `PH0M
-00005670: 4245 5260 2066 7261 6d65 776f 726b 2e2e  BER` framework..
-00005680: 2e72 1e00 0000 721f 0000 0029 0372 a400  .r....r....).r..
-00005690: 0000 72a7 0000 0072 a800 0000 5429 0472  ..r....r....T).r
-000056a0: 2200 0000 7288 0000 0072 8700 0000 7289  "...r....r....r.
-000056b0: 0000 0029 057a 101b 5b31 3b34 393b 3932  ...).z..[1;49;92
-000056c0: 6d3a 441b 5b30 6d7a 101b 5b31 3b34 393b  m:D.[0mz..[1;49;
-000056d0: 3936 6d3a 291b 5b30 6d7a 101b 5b31 3b34  96m:).[0mz..[1;4
-000056e0: 393b 3933 6d3a 7c1b 5b30 6d7a 101b 5b31  9;93m:|.[0mz..[1
-000056f0: 3b34 393b 3931 6d3a 281b 5b30 6d7a 101b  ;49;91m:(.[0mz..
-00005700: 5b31 3b34 393b 3937 6d3a 6f1b 5b30 6d72  [1;49;97m:o.[0mr
-00005710: 0100 0000 75f3 0300 0020 2020 201b 5b31  ....u....    .[1
-00005720: 3b34 393b 3933 6d3e 2045 7870 7265 7373  ;49;93m> Express
-00005730: 696f 6e73 2061 7265 2075 7365 6420 746f  ions are used to
-00005740: 2073 686f 7720 7468 6520 7374 6174 7573   show the status
-00005750: 206f 6620 7468 6520 7072 6576 696f 7573   of the previous
-00005760: 2063 6f6d 6d61 6e64 1b5b 306d 0a0a 2020   command.[0m..  
-00005770: 2020 1b5b 313b 3439 3b39 336d 3e20 5379    .[1;49;93m> Sy
-00005780: 6e74 6178 3a1b 5b30 6d20 1b5b 313b 3439  ntax:.[0m .[1;49
-00005790: 3b39 376d 5b3c 7573 6572 3e40 7068 306d  ;97m[<user>@ph0m
-000057a0: 6265 725d e2b8 ba20 1b5b 313b 3439 3b39  ber]... .[1;49;9
-000057b0: 366d 5b3c 6578 7072 6573 7369 6f6e 3e5d  6m[<expression>]
-000057c0: 1b5b 313b 3439 3b39 376d 2024 203c 636f  .[1;49;97m $ <co
-000057d0: 6d6d 616e 643e 1b5b 306d 0a0a 2020 2020  mmand>.[0m..    
-000057e0: e294 8ce2 9480 e294 80e2 9480 e294 80e2  ................
-000057f0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00005800: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00005810: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00005820: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00005830: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00005840: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00005850: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00005860: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00005870: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00005880: 9490 0a20 2020 207c 2045 5850 5245 5353  ...    | EXPRESS
-00005890: 494f 4e53 2020 207c 2044 4553 4352 4950  IONS   | DESCRIP
-000058a0: 5449 4f4e 2020 2020 2020 2020 2020 2020  TION            
-000058b0: 2020 2020 2020 2020 2020 2020 7c0a 2020              |.  
-000058c0: 2020 7c2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d    |-------------
-000058d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000058e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000058f0: 2d2d 2d2d 2d2d 2d7c 0a20 2020 207c 201b  -------|.    | .
-00005900: 5b31 3b34 393b 3932 6d3a 441b 5b30 6d20  [1;49;92m:D.[0m 
-00005910: 2020 2020 2020 2020 2020 207c 2045 7665             | Eve
-00005920: 7279 7468 696e 6720 6973 2066 696e 6520  rything is fine 
-00005930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005940: 7c0a 2020 2020 7c20 1b5b 313b 3439 3b39  |.    | .[1;49;9
-00005950: 366d 3a29 1b5b 306d 2020 2020 2020 2020  6m:).[0m        
-00005960: 2020 2020 7c20 496e 666f 726d 6174 696f      | Informatio
-00005970: 6e20 6176 6169 6c61 626c 6520 2020 2020  n available     
-00005980: 2020 2020 2020 2020 207c 0a20 2020 207c           |.    |
-00005990: 201b 5b31 3b34 393b 3933 6d3a 7c1b 5b30   .[1;49;93m:|.[0
-000059a0: 6d20 2020 2020 2020 2020 2020 207c 2049  m            | I
-000059b0: 7427 7320 6120 7761 726e 696e 6720 2872  t's a warning (r
-000059c0: 656d 656d 6265 7229 2020 2020 2020 2020  emember)        
-000059d0: 2020 7c0a 2020 2020 7c20 1b5b 313b 3439    |.    | .[1;49
-000059e0: 3b39 316d 3a28 1b5b 306d 2020 2020 2020  ;91m:(.[0m      
-000059f0: 2020 2020 2020 7c20 536f 6d65 7468 696e        | Somethin
-00005a00: 6720 7765 6e74 2077 726f 6e67 2020 2020  g went wrong    
-00005a10: 2020 2020 2020 2020 2020 207c 0a20 2020             |.   
-00005a20: 207c 201b 5b31 3b34 393b 3937 6d3a 6f1b   | .[1;49;97m:o.
-00005a30: 5b30 6d20 2020 2020 2020 2020 2020 207c  [0m            |
-00005a40: 2053 6361 6e20 7265 7375 6c74 7320 6176   Scan results av
-00005a50: 6169 6c61 626c 6520 2020 2020 2020 2020  ailable         
-00005a60: 2020 2020 7c0a 2020 2020 e294 94e2 9480      |.    ......
-00005a70: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00005a80: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00005a90: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00005aa0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00005ab0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00005ac0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00005ad0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00005ae0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00005af0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00005b00: e294 80e2 9480 e294 80e2 9498 7a0a 1b5b  ............z..[
-00005b10: 313b 3439 3b39 366d 7280 0000 0072 3000  1;49;96mr....r0.
-00005b20: 0000 e922 0000 00fa 0125 e921 0000 00e9  ...".....%.!....
-00005b30: 2000 0000 7234 0000 007a 161b 5b31 3b34   ...r4...z..[1;4
-00005b40: 393b 3936 6d33 2e30 2062 6574 611b 5b30  9;96m3.0 beta.[0
-00005b50: 6d67 0000 0000 0000 0840 7542 0100 000a  mg.......@uB....
-00005b60: 2020 2020 e294 8ce2 9480 e294 80e2 9480      ............
-00005b70: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00005b80: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00005b90: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00005ba0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00005bb0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00005bc0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00005bd0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00005be0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00005bf0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00005c00: e294 80e2 9490 0a20 2020 207c 2053 5953  .......    | SYS
-00005c10: 5445 4d20 494e 464f 2020 207c 2044 4553  TEM INFO   | DES
-00005c20: 4352 4950 5449 4f4e 2020 2020 2020 2020  CRIPTION        
-00005c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005c40: 7c0a 2020 2020 7c2d 2d2d 2d2d 2d2d 2d2d  |.    |---------
-00005c50: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00005c60: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00005c70: 2d2d 2d2d 2d2d 2d2d 2d2d 2d7c 0a20 2020  -----------|.   
-00005c80: 207c 201b 5b31 3b34 393b 3937 6d55 7365   | .[1;49;97mUse
-00005c90: 721b 5b30 6d20 2020 2020 2020 2020 207c  r.[0m          |
-00005ca0: 207a 2720 7c0a 2020 2020 7c20 1b5b 313b   z' |.    | .[1;
-00005cb0: 3439 3b39 376d 486f 7374 6e61 6d65 1b5b  49;97mHostname.[
-00005cc0: 306d 2020 2020 2020 7c20 7a27 207c 0a20  0m      | z' |. 
-00005cd0: 2020 207c 201b 5b31 3b34 393b 3937 6d4f     | .[1;49;97mO
-00005ce0: 531b 5b30 6d20 2020 2020 2020 2020 2020  S.[0m           
-00005cf0: 207c 207a 2720 7c0a 2020 2020 7c20 1b5b   | z' |.    | .[
-00005d00: 313b 3439 3b39 376d 5241 4d20 5573 6167  1;49;97mRAM Usag
-00005d10: 651b 5b30 6d20 2020 2020 7c20 7a27 207c  e.[0m     | z' |
-00005d20: 0a20 2020 207c 201b 5b31 3b34 393b 3937  .    | .[1;49;97
-00005d30: 6d43 5055 2055 7361 6765 1b5b 306d 2020  mCPU Usage.[0m  
-00005d40: 2020 207c 207a 2720 7c0a 2020 2020 7c20     | z' |.    | 
-00005d50: 1b5b 313b 3439 3b39 376d 4469 736b 2055  .[1;49;97mDisk U
-00005d60: 7361 6765 1b5b 306d 2020 2020 7c20 7543  sage.[0m    | uC
-00005d70: 0200 0020 7c0a 2020 2020 e294 94e2 9480  ... |.    ......
-00005d80: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00005d90: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00005da0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00005db0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00005dc0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00005dd0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00005de0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00005df0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00005e00: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00005e10: e294 80e2 9480 e294 80e2 9498 0a0a 2020  ..............  
-00005e20: 2020 e294 8ce2 9480 e294 80e2 9480 e294    ..............
-00005e30: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00005e40: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00005e50: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00005e60: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00005e70: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00005e80: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00005e90: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00005ea0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00005eb0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00005ec0: 80e2 9490 0a20 2020 207c 2046 5241 4d45  .....    | FRAME
-00005ed0: 574f 524b 2049 4e46 4f7c 2044 4553 4352  WORK INFO| DESCR
-00005ee0: 4950 5449 4f4e 2020 2020 2020 2020 2020  IPTION          
-00005ef0: 2020 2020 2020 2020 2020 2020 2020 7c0a                |.
-00005f00: 2020 2020 7c2d 2d2d 2d2d 2d2d 2d2d 2d2d      |-----------
-00005f10: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00005f20: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00005f30: 2d2d 2d2d 2d2d 2d2d 2d7c 0a20 2020 207c  ---------|.    |
-00005f40: 201b 5b31 3b34 393b 3937 6d4e 616d 651b   .[1;49;97mName.
-00005f50: 5b30 6d20 2020 2020 2020 2020 207c 201b  [0m          | .
-00005f60: 5b31 3b34 393b 3936 6d50 4830 4d42 4552  [1;49;96mPH0MBER
-00005f70: 1b5b 306d 2020 2020 2020 2020 2020 2020  .[0m            
-00005f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005f90: 7c0a 2020 2020 7c20 1b5b 313b 3439 3b39  |.    | .[1;49;9
-00005fa0: 376d 5665 7273 696f 6e1b 5b30 6d20 2020  7mVersion.[0m   
-00005fb0: 2020 2020 7c20 75b3 0100 0020 7c0a 2020      | u.... |.  
-00005fc0: 2020 7c20 1b5b 313b 3439 3b39 376d 5479    | .[1;49;97mTy
-00005fd0: 7065 1b5b 306d 2020 2020 2020 2020 2020  pe.[0m          
-00005fe0: 7c20 1b5b 313b 3439 3b39 366d 4f53 494e  | .[1;49;96mOSIN
-00005ff0: 541b 5b30 6d20 2020 2020 2020 2020 2020  T.[0m           
-00006000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006010: 2020 207c 0a20 2020 207c 201b 5b31 3b34     |.    | .[1;4
-00006020: 393b 3937 6d41 7574 686f 721b 5b30 6d20  9;97mAuthor.[0m 
-00006030: 2020 2020 2020 207c 201b 5b31 3b34 393b         | .[1;49;
-00006040: 3936 6d73 3431 7234 6a1b 5b30 6d20 2020  96ms41r4j.[0m   
-00006050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006060: 2020 2020 2020 2020 2020 7c0a 2020 2020            |.    
-00006070: 7c20 1b5b 313b 3439 3b39 376d 4769 7468  | .[1;49;97mGith
-00006080: 7562 1b5b 306d 2020 2020 2020 2020 7c20  ub.[0m        | 
-00006090: 1b5b 313b 3439 3b39 366d 6874 7470 733a  .[1;49;96mhttps:
-000060a0: 2f2f 6769 7468 7562 2e63 6f6d 2f73 3431  //github.com/s41
-000060b0: 7234 6a2f 7068 6f6d 6265 721b 5b30 6d20  r4j/phomber.[0m 
-000060c0: 207c 0a20 2020 20e2 9494 e294 80e2 9480   |.    .........
-000060d0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-000060e0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-000060f0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00006100: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00006110: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00006120: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00006130: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00006140: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00006150: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00006160: e294 80e2 9480 e294 980a 2020 2020 75ea  ..........    u.
-00006170: 0700 000a 2020 2020 e294 8ce2 9480 e294  ....    ........
-00006180: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00006190: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-000061a0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-000061b0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-000061c0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-000061d0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-000061e0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-000061f0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00006200: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00006210: 80e2 9480 e294 80e2 9490 0a20 2020 207c  ...........    |
-00006220: 2043 4f4d 4d41 4e44 5320 2020 2020 207c   COMMANDS      |
-00006230: 2044 4553 4352 4950 5449 4f4e 2020 2020   DESCRIPTION    
-00006240: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006250: 2020 2020 7c0a 2020 2020 7c2d 2d2d 2d2d      |.    |-----
-00006260: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00006270: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00006280: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d7c  ---------------|
-00006290: 0a20 2020 207c 2020 2020 2020 2020 2020  .    |          
-000062a0: 2020 2020 2020 3c42 6173 6963 2043 6f6d        <Basic Com
-000062b0: 6d61 6e64 733e 2020 2020 2020 2020 2020  mands>          
-000062c0: 2020 2020 2020 2020 2020 7c0a 2020 2020            |.    
-000062d0: 7c2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  |---------------
-000062e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000062f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00006300: 2d2d 2d2d 2d7c 0a20 2020 207c 201b 5b31  -----|.    | .[1
-00006310: 3b34 393b 3937 6d68 656c 701b 5b30 6d20  ;49;97mhelp.[0m 
-00006320: 2020 2020 2020 2020 207c 2044 6973 706c           | Displ
-00006330: 6179 2074 6869 7320 6865 6c70 206d 656e  ay this help men
-00006340: 7520 2020 2020 2020 2020 2020 2020 7c20  u             | 
-00006350: 0a20 2020 207c 201b 5b31 3b34 393b 3937  .    | .[1;49;97
-00006360: 6d65 7869 742f 7175 6974 1b5b 306d 2020  mexit/quit.[0m  
-00006370: 2020 207c 2045 7869 7420 7468 6520 6672     | Exit the fr
-00006380: 616d 6577 6f72 6b20 2020 2020 2020 2020  amework         
-00006390: 2020 2020 2020 2020 7c0a 2020 2020 7c20          |.    | 
-000063a0: 1b5b 313b 3439 3b39 376d 646f 726b 1b5b  .[1;49;97mdork.[
-000063b0: 306d 2020 2020 2020 2020 2020 7c20 5368  0m          | Sh
-000063c0: 6f77 2061 2072 616e 646f 6d20 676f 6f67  ow a random goog
-000063d0: 6c65 2064 6f72 6b20 7175 6572 7920 2020  le dork query   
-000063e0: 207c 2020 0a20 2020 207c 201b 5b31 3b34   |  .    | .[1;4
-000063f0: 393b 3937 6d65 7870 1b5b 306d 2020 2020  9;97mexp.[0m    
-00006400: 2020 2020 2020 207c 2053 686f 7720 696e         | Show in
-00006410: 666f 2061 626f 7574 2061 6c6c 2061 7661  fo about all ava
-00006420: 696c 6162 6c65 2020 2020 2020 7c20 2020  ilable      |   
-00006430: 2020 2020 0a20 2020 207c 2020 2020 2020      .    |      
-00006440: 2020 2020 2020 2020 207c 2065 7870 7265           | expre
-00006450: 7373 696f 6e73 2020 2020 2020 2020 2020  ssions          
-00006460: 2020 2020 2020 2020 2020 2020 2020 7c0a                |.
-00006470: 2020 2020 7c20 1b5b 313b 3439 3b39 376d      | .[1;49;97m
-00006480: 6368 6563 6b1b 5b30 6d20 2020 2020 2020  check.[0m       
-00006490: 2020 7c20 4368 6563 6b20 696e 7465 726e    | Check intern
-000064a0: 6574 2063 6f6e 6e65 6374 696f 6e20 2020  et connection   
-000064b0: 2020 2020 2020 207c 0a20 2020 207c 201b         |.    | .
-000064c0: 5b31 3b34 393b 3937 6d63 6c65 6172 1b5b  [1;49;97mclear.[
-000064d0: 306d 2020 2020 2020 2020 207c 2043 6c65  0m         | Cle
-000064e0: 6172 2073 6372 6565 6e20 2020 2020 2020  ar screen       
-000064f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006500: 7c0a 2020 2020 7c20 1b5b 313b 3439 3b39  |.    | .[1;49;9
-00006510: 376d 7361 7665 1b5b 306d 2020 2020 2020  7msave.[0m      
-00006520: 2020 2020 7c20 5361 7665 206f 7574 7075      | Save outpu
-00006530: 7420 6f66 2070 7265 7669 6f75 7320 7363  t of previous sc
-00006540: 616e 6e65 7220 2020 207c 0a20 2020 207c  anner    |.    |
-00006550: 2020 2020 2020 2020 2020 2020 2020 207c                 |
-00006560: 2063 6f6d 6d61 6e64 2069 6e20 6120 6669   command in a fi
-00006570: 6c65 2020 2020 2020 2020 2020 2020 2020  le              
-00006580: 2020 2020 7c0a 2020 2020 7c20 1b5b 313b      |.    | .[1;
-00006590: 3439 3b39 376d 7368 656c 6c20 3c63 6d64  49;97mshell <cmd
-000065a0: 3e1b 5b30 6d20 2020 7c20 4578 6563 7574  >.[0m   | Execut
-000065b0: 6520 6e61 7469 7665 2073 6865 6c6c 2f63  e native shell/c
-000065c0: 6d64 2063 6f6d 6d61 6e64 7320 207c 0a20  md commands  |. 
-000065d0: 2020 207c 201b 5b31 3b34 393b 3937 6d69     | .[1;49;97mi
-000065e0: 6e66 6f1b 5b30 6d20 2020 2020 2020 2020  nfo.[0m         
-000065f0: 207c 2053 686f 7720 696e 666f 2061 626f   | Show info abo
-00006600: 7574 2066 7261 6d65 776f 726b 2026 2073  ut framework & s
-00006610: 7973 7465 6d20 7c0a 2020 2020 7c20 1b5b  ystem |.    | .[
-00006620: 313b 3439 3b39 376d 6368 616e 6765 1b5b  1;49;97mchange.[
-00006630: 306d 2020 2020 2020 2020 7c20 4368 616e  0m        | Chan
-00006640: 6765 2075 7365 7220 636f 6d6d 616e 6420  ge user command 
-00006650: 696e 7075 7420 636f 6c6f 7220 2020 207c  input color    |
-00006660: 0a20 2020 207c 2d2d 2d2d 2d2d 2d2d 2d2d  .    |----------
-00006670: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00006680: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00006690: 2d2d 2d2d 2d2d 2d2d 2d2d 7c0a 2020 2020  ----------|.    
-000066a0: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
-000066b0: 2020 3c53 6361 6e6e 6572 2043 6f6d 6d61    <Scanner Comma
-000066c0: 6e64 733e 2020 2020 2020 2020 2020 2020  nds>            
-000066d0: 2020 2020 207c 0a20 2020 207c 2d2d 2d2d       |.    |----
-000066e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000066f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00006700: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00006710: 7c0a 2020 2020 7c20 1b5b 313b 3439 3b39  |.    | .[1;49;9
-00006720: 376d 6e75 6d62 6572 1b5b 306d 2020 2020  7mnumber.[0m    
-00006730: 2020 2020 7c20 5265 7665 7273 6520 7068      | Reverse ph
-00006740: 6f6e 6520 6e75 6d62 6572 206c 6f6f 6b75  one number looku
-00006750: 7020 2020 2020 2020 207c 0a20 2020 207c  p        |.    |
-00006760: 201b 5b31 3b34 393b 3937 6d69 701b 5b30   .[1;49;97mip.[0
-00006770: 6d20 2020 2020 2020 2020 2020 207c 2052  m            | R
-00006780: 6576 6572 7365 2069 7020 6164 6472 6573  everse ip addres
-00006790: 7320 6c6f 6f6b 7570 2020 2020 2020 2020  s lookup        
-000067a0: 2020 7c0a 2020 2020 7c20 1b5b 313b 3439    |.    | .[1;49
-000067b0: 3b39 316d 4d4f 5245 2053 4341 4e4e 4552  ;91mMORE SCANNER
-000067c0: 5320 434f 4d49 4e47 2053 4f4f 4e2c 2054  S COMING SOON, T
-000067d0: 4849 5320 4953 2041 2042 4554 4120 5645  HIS IS A BETA VE
-000067e0: 521b 5b30 6d20 2020 2020 207c 0a20 2020  R.[0m      |.   
-000067f0: 20e2 9494 e294 80e2 9480 e294 80e2 9480   ...............
-00006800: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00006810: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00006820: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00006830: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00006840: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00006850: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00006860: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00006870: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00006880: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00006890: e294 980a 0a20 2020 201b 5b31 3b34 393b  .....    .[1;49;
-000068a0: 3933 6d3e 2054 7970 6520 6068 656c 7020  93m> Type `help 
-000068b0: 3c63 6f6d 6d61 6e64 3e60 2074 6f20 7365  <command>` to se
-000068c0: 6520 6d6f 7265 2069 6e66 6f20 6162 6f75  e more info abou
-000068d0: 7420 6120 636f 6d6d 616e 641b 5b30 6d0a  t a command.[0m.
-000068e0: 2020 2020 1b5b 313b 3439 3b39 336d 3e20      .[1;49;93m> 
-000068f0: 5573 6520 6054 6162 6020 6b65 7920 746f  Use `Tab` key to
-00006900: 2061 7574 6f2d 636f 6d70 6c65 7465 2063   auto-complete c
-00006910: 6f6d 6d61 6e64 731b 5b30 6d0a 2020 2020  ommands.[0m.    
-00006920: 1b5b 313b 3439 3b39 336d 3e20 5472 7920  .[1;49;93m> Try 
-00006930: 7369 6c65 6e74 206d 6f64 6520 6279 2075  silent mode by u
-00006940: 7369 6e67 2060 2d73 602f 602d 2d73 696c  sing `-s`/`--sil
-00006950: 656e 7460 2066 6c61 671b 5b30 6d72 0f00  ent` flag.[0mr..
-00006960: 0000 7a0d 7461 623a 2063 6f6d 706c 6574  ..z.tab: complet
-00006970: 657a 0a1b 5b31 3b34 393b 3930 6d7a 0a1b  ez..[1;49;90mz..
-00006980: 5b31 3b34 393b 3937 6d7a 020a 5b75 0e00  [1;49;97mz..[u..
-00006990: 0000 4070 6830 6d62 6572 5de2 b8ba 205b  ..@ph0mber]... [
-000069a0: 7a04 5d20 2420 2902 728b 0000 0072 8900  z.] $ ).r....r..
-000069b0: 0000 7202 0000 00e9 0400 0000 fa01 23e9  ..r...........#.
-000069c0: 0500 0000 612b 0100 0020 201b 5b31 3b34  ....a+...  .[1;4
-000069d0: 393b 3933 6d5b 2b5d 2043 6f6d 6d61 6e64  9;93m[+] Command
-000069e0: 2049 6e66 6f3a 201b 5b31 3b34 393b 3933   Info: .[1;49;93
-000069f0: 6d68 656c 700a 0a20 2020 201b 5b31 3b34  mhelp..    .[1;4
-00006a00: 393b 3932 6d3e 2044 4553 4352 4950 5449  9;92m> DESCRIPTI
-00006a10: 4f4e 3a20 1b5b 313b 3439 3b39 376d 5768  ON: .[1;49;97mWh
-00006a20: 656e 2079 6f75 2074 7970 6520 6068 656c  en you type `hel
-00006a30: 7060 2c20 7468 6520 6865 6c70 206d 656e  p`, the help men
-00006a40: 7520 7769 6c6c 2062 6520 6469 7370 6c61  u will be displa
-00006a50: 7965 640a 2020 2020 1b5b 313b 3439 3b39  yed.    .[1;49;9
-00006a60: 326d 3e20 5359 4e54 4158 3a20 1b5b 313b  2m> SYNTAX: .[1;
-00006a70: 3439 3b39 376d 6865 6c70 201b 5b31 3b34  49;97mhelp .[1;4
-00006a80: 393b 3932 6d4f 5220 1b5b 313b 3439 3b39  9;92mOR .[1;49;9
-00006a90: 376d 6865 6c70 203c 636f 6d6d 616e 643e  7mhelp <command>
-00006aa0: 0a20 2020 201b 5b31 3b34 393b 3932 6d3e  .    .[1;49;92m>
-00006ab0: 2045 5841 4d50 4c45 3a20 1b5b 313b 3439   EXAMPLE: .[1;49
-00006ac0: 3b39 376d 6865 6c70 201b 5b31 3b34 393b  ;97mhelp .[1;49;
-00006ad0: 3932 6d4f 5220 1b5b 313b 3439 3b39 376d  92mOR .[1;49;97m
-00006ae0: 6865 6c70 206e 756d 6265 720a 2020 2020  help number.    
-00006af0: 1b5b 306d 7203 0000 0072 0400 0000 7aee  .[0mr....r....z.
-00006b00: 2020 1b5b 313b 3439 3b39 336d 5b2b 5d20    .[1;49;93m[+] 
-00006b10: 436f 6d6d 616e 6420 496e 666f 3a20 1b5b  Command Info: .[
-00006b20: 313b 3439 3b39 336d 6578 6974 2f1b 5b31  1;49;93mexit/.[1
-00006b30: 3b34 393b 3933 6d71 7569 740a 0a20 2020  ;49;93mquit..   
-00006b40: 201b 5b31 3b34 393b 3932 6d3e 2044 4553   .[1;49;92m> DES
-00006b50: 4352 4950 5449 4f4e 3a20 1b5b 313b 3439  CRIPTION: .[1;49
-00006b60: 3b39 376d 5768 656e 2079 6f75 2074 7970  ;97mWhen you typ
-00006b70: 6520 6065 7869 7460 206f 7220 6071 7569  e `exit` or `qui
-00006b80: 7460 2c20 7468 6520 7072 6f67 7261 6d20  t`, the program 
-00006b90: 7769 6c6c 2062 6520 7465 726d 696e 6174  will be terminat
-00006ba0: 6564 0a20 2020 201b 5b31 3b34 393b 3932  ed.    .[1;49;92
-00006bb0: 6d3e 2053 594e 5441 583a 201b 5b31 3b34  m> SYNTAX: .[1;4
-00006bc0: 393b 3937 6d65 7869 7420 1b5b 313b 3439  9;97mexit .[1;49
-00006bd0: 3b39 326d 4f52 201b 5b31 3b34 393b 3937  ;92mOR .[1;49;97
-00006be0: 6d71 7569 740a 2020 2020 1b5b 306d 7205  mquit.    .[0mr.
-00006bf0: 0000 007a c720 201b 5b31 3b34 393b 3933  ...z.  .[1;49;93
-00006c00: 6d5b 2b5d 2043 6f6d 6d61 6e64 2049 6e66  m[+] Command Inf
-00006c10: 6f3a 201b 5b31 3b34 393b 3933 6d64 6f72  o: .[1;49;93mdor
-00006c20: 6b0a 0a20 2020 201b 5b31 3b34 393b 3932  k..    .[1;49;92
-00006c30: 6d3e 2044 4553 4352 4950 5449 4f4e 3a20  m> DESCRIPTION: 
-00006c40: 1b5b 313b 3439 3b39 376d 5768 656e 2079  .[1;49;97mWhen y
-00006c50: 6f75 2074 7970 6520 6064 6f72 6b60 2c20  ou type `dork`, 
-00006c60: 6120 7261 6e64 6f6d 2067 6f6f 676c 6520  a random google 
-00006c70: 646f 726b 2071 7565 7279 2077 696c 6c20  dork query will 
-00006c80: 6265 2064 6973 706c 6179 6564 0a20 2020  be displayed.   
-00006c90: 201b 5b31 3b34 393b 3932 6d3e 2053 594e   .[1;49;92m> SYN
-00006ca0: 5441 583a 201b 5b31 3b34 393b 3937 6d64  TAX: .[1;49;97md
-00006cb0: 6f72 6b0a 2020 2020 1b5b 306d 7206 0000  ork.    .[0mr...
-00006cc0: 007a ce20 201b 5b31 3b34 393b 3933 6d5b  .z.  .[1;49;93m[
-00006cd0: 2b5d 2043 6f6d 6d61 6e64 2049 6e66 6f3a  +] Command Info:
-00006ce0: 201b 5b31 3b34 393b 3933 6d65 7870 0a0a   .[1;49;93mexp..
-00006cf0: 2020 2020 1b5b 313b 3439 3b39 326d 3e20      .[1;49;92m> 
-00006d00: 4445 5343 5249 5054 494f 4e3a 201b 5b31  DESCRIPTION: .[1
-00006d10: 3b34 393b 3937 6d57 6865 6e20 796f 7520  ;49;97mWhen you 
-00006d20: 7479 7065 2060 6578 7060 2c20 696e 666f  type `exp`, info
-00006d30: 2061 626f 7574 2061 6c6c 2061 7661 696c   about all avail
-00006d40: 6162 6c65 2065 7870 7265 7373 696f 6e73  able expressions
-00006d50: 2077 696c 6c20 6265 2064 6973 706c 6179   will be display
-00006d60: 6564 0a20 2020 201b 5b31 3b34 393b 3932  ed.    .[1;49;92
-00006d70: 6d3e 2053 594e 5441 583a 201b 5b31 3b34  m> SYNTAX: .[1;4
-00006d80: 393b 3937 6d65 7870 0a20 2020 201b 5b30  9;97mexp.    .[0
-00006d90: 6d72 0700 0000 7ad0 2020 1b5b 313b 3439  mr....z.  .[1;49
-00006da0: 3b39 336d 5b2b 5d20 436f 6d6d 616e 6420  ;93m[+] Command 
-00006db0: 496e 666f 3a20 1b5b 313b 3439 3b39 336d  Info: .[1;49;93m
-00006dc0: 6368 6563 6b0a 0a20 2020 201b 5b31 3b34  check..    .[1;4
-00006dd0: 393b 3932 6d3e 2044 4553 4352 4950 5449  9;92m> DESCRIPTI
-00006de0: 4f4e 3a20 1b5b 313b 3439 3b39 376d 5768  ON: .[1;49;97mWh
-00006df0: 656e 2079 6f75 2074 7970 6520 6063 6865  en you type `che
-00006e00: 636b 602c 2069 7420 7769 6c6c 2063 6865  ck`, it will che
-00006e10: 636b 2066 6f72 2069 6e74 6572 6e65 7420  ck for internet 
-00006e20: 636f 6e6e 6563 7469 6f6e 2061 7661 696c  connection avail
-00006e30: 6162 696c 6974 790a 2020 2020 1b5b 313b  ability.    .[1;
-00006e40: 3439 3b39 326d 3e20 5359 4e54 4158 3a20  49;92m> SYNTAX: 
-00006e50: 1b5b 313b 3439 3b39 376d 6368 6563 6b0a  .[1;49;97mcheck.
-00006e60: 2020 2020 1b5b 306d 7208 0000 007a b620      .[0mr....z. 
-00006e70: 201b 5b31 3b34 393b 3933 6d5b 2b5d 2043   .[1;49;93m[+] C
-00006e80: 6f6d 6d61 6e64 2049 6e66 6f3a 201b 5b31  ommand Info: .[1
-00006e90: 3b34 393b 3933 6d63 6c65 6172 0a0a 2020  ;49;93mclear..  
-00006ea0: 2020 1b5b 313b 3439 3b39 326d 3e20 4445    .[1;49;92m> DE
-00006eb0: 5343 5249 5054 494f 4e3a 201b 5b31 3b34  SCRIPTION: .[1;4
-00006ec0: 393b 3937 6d57 6865 6e20 796f 7520 7479  9;97mWhen you ty
-00006ed0: 7065 2060 636c 6561 7260 2c20 6974 2077  pe `clear`, it w
-00006ee0: 696c 6c20 636c 6561 7220 7468 6520 7363  ill clear the sc
-00006ef0: 7265 656e 0a20 2020 201b 5b31 3b34 393b  reen.    .[1;49;
-00006f00: 3932 6d3e 2053 594e 5441 583a 201b 5b31  92m> SYNTAX: .[1
-00006f10: 3b34 393b 3937 6d63 6c65 6172 0a20 2020  ;49;97mclear.   
-00006f20: 201b 5b30 6d72 0900 0000 7aee 2020 1b5b   .[0mr....z.  .[
-00006f30: 313b 3439 3b39 336d 5b2b 5d20 436f 6d6d  1;49;93m[+] Comm
-00006f40: 616e 6420 496e 666f 3a20 1b5b 313b 3439  and Info: .[1;49
-00006f50: 3b39 336d 7361 7665 0a0a 2020 2020 1b5b  ;93msave..    .[
-00006f60: 313b 3439 3b39 326d 3e20 4445 5343 5249  1;49;92m> DESCRI
-00006f70: 5054 494f 4e3a 201b 5b31 3b34 393b 3937  PTION: .[1;49;97
-00006f80: 6d57 6865 6e20 796f 7520 7479 7065 2060  mWhen you type `
-00006f90: 7361 7665 602c 2069 7420 7769 6c6c 2073  save`, it will s
-00006fa0: 6176 6520 7468 6520 6f75 7470 7574 206f  ave the output o
-00006fb0: 6620 7072 6576 696f 7573 2063 6f6d 6d61  f previous comma
-00006fc0: 6e64 0a20 2020 201b 5b31 3b34 393b 3932  nd.    .[1;49;92
-00006fd0: 6d3e 2053 594e 5441 583a 201b 5b31 3b34  m> SYNTAX: .[1;4
-00006fe0: 393b 3937 6d73 6176 650a 2020 2020 1b5b  9;97msave.    .[
-00006ff0: 313b 3439 3b39 326d 3e20 4558 414d 504c  1;49;92m> EXAMPL
-00007000: 453a 201b 5b31 3b34 393b 3937 6d73 6176  E: .[1;49;97msav
-00007010: 650a 2020 2020 1b5b 306d 720a 0000 0061  e.    .[0mr....a
-00007020: 0101 0000 2020 1b5b 313b 3439 3b39 336d  ....  .[1;49;93m
-00007030: 5b2b 5d20 436f 6d6d 616e 6420 496e 666f  [+] Command Info
-00007040: 3a20 1b5b 313b 3439 3b39 336d 7368 656c  : .[1;49;93mshel
-00007050: 6c0a 0a20 2020 201b 5b31 3b34 393b 3932  l..    .[1;49;92
-00007060: 6d3e 2044 4553 4352 4950 5449 4f4e 3a20  m> DESCRIPTION: 
-00007070: 1b5b 313b 3439 3b39 376d 5768 656e 2079  .[1;49;97mWhen y
-00007080: 6f75 2074 7970 6520 6073 6865 6c6c 602c  ou type `shell`,
-00007090: 2069 7420 7769 6c6c 2065 7865 6375 7465   it will execute
-000070a0: 2067 6976 656e 2063 6f6d 6d61 6e64 2069   given command i
-000070b0: 6e20 6e61 7469 7665 2073 6865 6c6c 2f63  n native shell/c
-000070c0: 6d64 0a20 2020 201b 5b31 3b34 393b 3932  md.    .[1;49;92
-000070d0: 6d3e 2053 594e 5441 583a 201b 5b31 3b34  m> SYNTAX: .[1;4
-000070e0: 393b 3937 6d73 6865 6c6c 203c 636d 643e  9;97mshell <cmd>
-000070f0: 0a20 2020 201b 5b31 3b34 393b 3932 6d3e  .    .[1;49;92m>
-00007100: 2045 5841 4d50 4c45 3a20 1b5b 313b 3439   EXAMPLE: .[1;49
-00007110: 3b39 376d 7368 656c 6c20 6c73 0a20 2020  ;97mshell ls.   
-00007120: 201b 5b30 6d72 0b00 0000 7ac5 2020 1b5b   .[0mr....z.  .[
-00007130: 313b 3439 3b39 336d 5b2b 5d20 436f 6d6d  1;49;93m[+] Comm
-00007140: 616e 6420 496e 666f 3a20 1b5b 313b 3439  and Info: .[1;49
-00007150: 3b39 336d 696e 666f 0a0a 2020 2020 1b5b  ;93minfo..    .[
-00007160: 313b 3439 3b39 326d 3e20 4445 5343 5249  1;49;92m> DESCRI
-00007170: 5054 494f 4e3a 201b 5b31 3b34 393b 3937  PTION: .[1;49;97
-00007180: 6d57 6865 6e20 796f 7520 7479 7065 2060  mWhen you type `
-00007190: 696e 666f 602c 2069 7420 7769 6c6c 2073  info`, it will s
-000071a0: 686f 7720 696e 666f 2061 626f 7574 2066  how info about f
-000071b0: 7261 6d65 776f 726b 2026 2073 7973 7465  ramework & syste
-000071c0: 6d0a 2020 2020 1b5b 313b 3439 3b39 326d  m.    .[1;49;92m
-000071d0: 3e20 5359 4e54 4158 3a20 1b5b 313b 3439  > SYNTAX: .[1;49
-000071e0: 3b39 376d 696e 666f 0a20 2020 201b 5b30  ;97minfo.    .[0
-000071f0: 6d72 0c00 0000 618a 0100 0020 201b 5b31  mr....a....  .[1
-00007200: 3b34 393b 3933 6d5b 2b5d 2043 6f6d 6d61  ;49;93m[+] Comma
-00007210: 6e64 2049 6e66 6f3a 201b 5b31 3b34 393b  nd Info: .[1;49;
-00007220: 3933 6d63 6861 6e67 650a 0a20 2020 201b  93mchange..    .
-00007230: 5b31 3b34 393b 3932 6d3e 2044 4553 4352  [1;49;92m> DESCR
-00007240: 4950 5449 4f4e 3a20 1b5b 313b 3439 3b39  IPTION: .[1;49;9
-00007250: 376d 5768 656e 2079 6f75 2074 7970 6520  7mWhen you type 
-00007260: 6063 6861 6e67 6560 2c20 6974 2077 696c  `change`, it wil
-00007270: 6c20 6368 616e 6765 2075 7365 7220 636f  l change user co
-00007280: 6d6d 616e 6420 696e 7075 7420 636f 6c6f  mmand input colo
-00007290: 720a 2020 2020 1b5b 313b 3439 3b39 326d  r.    .[1;49;92m
-000072a0: 3e20 4f50 5449 4f4e 533a 201b 5b31 3b34  > OPTIONS: .[1;4
-000072b0: 393b 3937 6d30 202d 3e20 1b5b 313b 3439  9;97m0 -> .[1;49
-000072c0: 3b39 306d 426c 6163 6b0a 2020 2020 2020  ;90mBlack.      
-000072d0: 2020 2020 2020 2020 201b 5b31 3b34 393b           .[1;49;
-000072e0: 3937 6d31 202d 3e20 5768 6974 6520 2020  97m1 -> White   
-000072f0: 2020 2020 200a 2020 2020 1b5b 313b 3439       .    .[1;49
-00007300: 3b39 326d 3e20 4465 6661 756c 743a 201b  ;92m> Default: .
-00007310: 5b31 3b34 393b 3937 6d31 0a20 2020 201b  [1;49;97m1.    .
-00007320: 5b31 3b34 393b 3932 6d3e 2053 594e 5441  [1;49;92m> SYNTA
-00007330: 583a 201b 5b31 3b34 393b 3937 6d63 6861  X: .[1;49;97mcha
-00007340: 6e67 6520 3c63 6f6c 6f72 5f63 6f64 653e  nge <color_code>
-00007350: 0a20 2020 201b 5b31 3b34 393b 3932 6d3e  .    .[1;49;92m>
-00007360: 2045 5841 4d50 4c45 3a20 1b5b 313b 3439   EXAMPLE: .[1;49
-00007370: 3b39 376d 6368 616e 6765 2030 0a20 2020  ;97mchange 0.   
-00007380: 201b 5b30 6d72 0d00 0000 6111 0100 0020   .[0mr....a.... 
-00007390: 201b 5b31 3b34 393b 3933 6d5b 2b5d 2043   .[1;49;93m[+] C
-000073a0: 6f6d 6d61 6e64 2049 6e66 6f3a 201b 5b31  ommand Info: .[1
-000073b0: 3b34 393b 3933 6d6e 756d 6265 720a 0a20  ;49;93mnumber.. 
-000073c0: 2020 201b 5b31 3b34 393b 3932 6d3e 2044     .[1;49;92m> D
-000073d0: 4553 4352 4950 5449 4f4e 3a20 1b5b 313b  ESCRIPTION: .[1;
-000073e0: 3439 3b39 376d 5768 656e 2079 6f75 2074  49;97mWhen you t
-000073f0: 7970 6520 606e 756d 6265 7260 2c20 6974  ype `number`, it
-00007400: 2077 696c 6c20 7065 7266 6f72 6d20 7265   will perform re
-00007410: 7665 7273 6520 7068 6f6e 6520 6e75 6d62  verse phone numb
-00007420: 6572 206c 6f6f 6b75 700a 2020 2020 1b5b  er lookup.    .[
-00007430: 313b 3439 3b39 326d 3e20 5359 4e54 4158  1;49;92m> SYNTAX
-00007440: 3a20 1b5b 313b 3439 3b39 376d 6e75 6d62  : .[1;49;97mnumb
-00007450: 6572 203c 7068 6f6e 655f 6e75 6d62 6572  er <phone_number
-00007460: 3e0a 2020 2020 1b5b 313b 3439 3b39 326d  >.    .[1;49;92m
-00007470: 3e20 4558 414d 504c 453a 201b 5b31 3b34  > EXAMPLE: .[1;4
-00007480: 393b 3937 6d6e 756d 6265 7220 2b31 3233  9;97mnumber +123
-00007490: 3435 3637 3839 300a 2020 2020 1b5b 306d  4567890.    .[0m
-000074a0: da05 656d 6169 6c7a f320 201b 5b31 3b34  ..emailz.  .[1;4
-000074b0: 393b 3933 6d5b 2b5d 2043 6f6d 6d61 6e64  9;93m[+] Command
-000074c0: 2049 6e66 6f3a 201b 5b31 3b34 393b 3933   Info: .[1;49;93
-000074d0: 6d65 6d61 696c 0a0a 2020 2020 1b5b 313b  memail..    .[1;
-000074e0: 3439 3b39 326d 3e20 4445 5343 5249 5054  49;92m> DESCRIPT
-000074f0: 494f 4e3a 201b 5b31 3b34 393b 3937 6d57  ION: .[1;49;97mW
-00007500: 6865 6e20 796f 7520 7479 7065 2060 656d  hen you type `em
-00007510: 6169 6c60 2c20 6974 2077 696c 6c20 7065  ail`, it will pe
-00007520: 7266 6f72 6d20 7265 7665 7273 6520 656d  rform reverse em
-00007530: 6169 6c20 6c6f 6f6b 7570 0a20 2020 201b  ail lookup.    .
-00007540: 5b31 3b34 393b 3932 6d3e 2053 594e 5441  [1;49;92m> SYNTA
-00007550: 583a 201b 5b31 3b34 393b 3937 6d65 6d61  X: .[1;49;97mema
-00007560: 696c 203c 656d 6169 6c5f 6164 6472 6573  il <email_addres
-00007570: 733e 0a20 2020 201b 5b31 3b34 393b 3932  s>.    .[1;49;92
-00007580: 6d3e 2045 5841 4d50 4c45 3a20 1b5b 313b  m> EXAMPLE: .[1;
-00007590: 3439 3b39 376d 656d 6169 6c20 7a1d 1b5b  49;97memail z..[
-000075a0: 313b 3439 3b39 366d 4067 6d61 696c 2e63  1;49;96m@gmail.c
-000075b0: 6f6d 0a20 2020 201b 5b30 6d72 0e00 0000  om.    .[0mr....
-000075c0: 7af9 2020 1b5b 313b 3439 3b39 336d 5b2b  z.  .[1;49;93m[+
-000075d0: 5d20 436f 6d6d 616e 6420 496e 666f 3a20  ] Command Info: 
-000075e0: 1b5b 313b 3439 3b39 336d 6970 0a0a 2020  .[1;49;93mip..  
-000075f0: 2020 1b5b 313b 3439 3b39 326d 3e20 4445    .[1;49;92m> DE
-00007600: 5343 5249 5054 494f 4e3a 201b 5b31 3b34  SCRIPTION: .[1;4
-00007610: 393b 3937 6d57 6865 6e20 796f 7520 7479  9;97mWhen you ty
-00007620: 7065 2060 6970 602c 2069 7420 7769 6c6c  pe `ip`, it will
-00007630: 2070 6572 666f 726d 2072 6576 6572 7365   perform reverse
-00007640: 2069 7020 6164 6472 6573 7320 6c6f 6f6b   ip address look
-00007650: 7570 0a20 2020 201b 5b31 3b34 393b 3932  up.    .[1;49;92
-00007660: 6d3e 2053 594e 5441 583a 201b 5b31 3b34  m> SYNTAX: .[1;4
-00007670: 393b 3937 6d69 7020 3c69 705f 6164 6472  9;97mip <ip_addr
-00007680: 6573 733e 0a20 2020 201b 5b31 3b34 393b  ess>.    .[1;49;
-00007690: 3932 6d3e 2045 5841 4d50 4c45 3a20 1b5b  92m> EXAMPLE: .[
-000076a0: 313b 3439 3b39 376d 6970 2038 2e38 2e38  1;49;97mip 8.8.8
-000076b0: 2e38 0a20 2020 201b 5b30 6de9 0300 0000  .8.    .[0m.....
-000076c0: 7a47 2020 2020 5b21 5d20 496e 7661 6c69  zG    [!] Invali
-000076d0: 6420 7375 622d 636f 6d6d 616e 6421 2054  d sub-command! T
-000076e0: 7970 6520 6068 656c 7060 2074 6f20 7365  ype `help` to se
-000076f0: 6520 616c 6c20 6176 6169 6c61 626c 6520  e all available 
-00007700: 636f 6d6d 616e 6473 2e72 2600 0000 7228  commands.r&...r(
-00007710: 0000 007a 4320 2020 205b 215d 2049 6e76  ...zC    [!] Inv
-00007720: 616c 6964 2063 6f6d 6d61 6e64 2120 5479  alid command! Ty
-00007730: 7065 2060 6865 6c70 6020 746f 2073 6565  pe `help` to see
-00007740: 2061 6c6c 2061 7661 696c 6162 6c65 2063   all available c
-00007750: 6f6d 6d61 6e64 732e 7a38 2020 2020 5b40  ommands.z8    [@
-00007760: 5d20 5468 616e 6b20 796f 7520 666f 7220  ] Thank you for 
-00007770: 7573 696e 6720 6050 4830 4d42 4552 6020  using `PH0MBER` 
-00007780: 6f73 696e 7420 6672 616d 6577 6f72 6b20  osint framework 
-00007790: 3a29 7a27 2020 2020 5b2b 5d20 4765 6e65  :)z'    [+] Gene
-000077a0: 7261 7469 6e67 2072 616e 646f 6d20 646f  rating random do
-000077b0: 726b 2071 7565 7279 2e2e 2e72 1d00 0000  rk query...r....
-000077c0: 7221 0000 007a 0620 2020 203e 2029 0372  r!...z.    > ).r
-000077d0: 1e00 0000 721f 0000 0072 a400 0000 7a27  ....r....r....z'
-000077e0: 2020 2020 5b2b 5d20 4368 6563 6b69 6e67      [+] Checking
-000077f0: 2069 6e74 6572 6e65 7420 636f 6e6e 6563   internet connec
-00007800: 7469 6f6e 2e2e 2e7a 1768 7474 7073 3a2f  tion...z.https:/
-00007810: 2f77 7777 2e67 6f6f 676c 652e 636f 6d2f  /www.google.com/
-00007820: 7a27 2020 2020 3e20 496e 7465 726e 6574  z'    > Internet
-00007830: 2063 6f6e 6e65 6374 696f 6e20 6973 2061   connection is a
-00007840: 7661 696c 6162 6c65 217a 1668 7474 7073  vailable!z.https
-00007850: 3a2f 2f68 7474 7062 696e 2e6f 7267 2f69  ://httpbin.org/i
-00007860: 70da 066f 7269 6769 6e7a 1068 7474 7073  p..originz.https
-00007870: 3a2f 2f69 6465 6e74 2e6d 657a 1568 7474  ://ident.mez.htt
-00007880: 7073 3a2f 2f61 7069 2e69 7069 6679 2e6f  ps://api.ipify.o
-00007890: 7267 467a 1920 2020 203e 2050 7562 6c69  rgFz.    > Publi
-000078a0: 6320 4950 2061 6464 7265 7373 3a20 7a2b  c IP address: z+
-000078b0: 2020 2020 3e20 496e 7465 726e 6574 2063      > Internet c
-000078c0: 6f6e 6e65 6374 696f 6e20 6973 206e 6f74  onnection is not
-000078d0: 2061 7661 696c 6162 6c65 217a 2120 2020   available!z!   
-000078e0: 203e 204c 6f63 616c 2049 5020 6164 6472   > Local IP addr
-000078f0: 6573 733a 2031 3237 2e30 2e30 2e31 728f  ess: 127.0.0.1r.
-00007900: 0000 0072 a300 0000 7a2c 2020 2020 5b2b  ...r....z,    [+
-00007910: 5d20 5361 7669 6e67 206f 7574 7075 7420  ] Saving output 
-00007920: 6f66 2070 7265 7669 6f75 7320 636f 6d6d  of previous comm
-00007930: 616e 642e 2e2e 7a45 2020 2020 3e20 4e6f  and...zE    > No
-00007940: 206f 7574 7075 7420 666f 756e 6421 2053   output found! S
-00007950: 6176 6573 206f 7574 7075 7420 6f66 2070  aves output of p
-00007960: 7265 7669 6f75 7320 7363 616e 6e65 7220  revious scanner 
-00007970: 636f 6d6d 616e 6420 6f6e 6c79 2172 4a00  command only!rJ.
-00007980: 0000 7a3b 2020 2020 3e20 4e6f 2063 6f6d  ..z;    > No com
-00007990: 6d61 6e64 2066 6f75 6e64 2120 5479 7065  mand found! Type
-000079a0: 2060 6865 6c70 2073 6865 6c6c 6020 746f   `help shell` to
-000079b0: 2073 6565 206d 6f72 6520 696e 666f 2ee9   see more info..
-000079c0: 0600 0000 7a25 2020 2020 1b5b 373b 3439  ....z%    .[7;49
-000079d0: 3b39 336d 5b2b 5d20 4578 6563 7574 696e  ;93m[+] Executin
-000079e0: 6720 636f 6d6d 616e 643a 207a 051b 5b30  g command: z..[0
-000079f0: 6d0a 7a20 3e20 436f 6d6d 616e 6420 6578  m.z > Command ex
-00007a00: 6563 7574 6564 2073 7563 6365 7373 6675  ecuted successfu
-00007a10: 6c6c 7921 2903 e907 0000 0072 1f00 0000  lly!)......r....
-00007a20: 72a4 0000 007a 050a 2020 2020 2902 7222  r....z..    ).r"
-00007a30: 0000 0072 8a00 0000 7a20 0a20 2020 203e  ...r....z .    >
-00007a40: 2043 6f6d 6d61 6e64 2065 7865 6375 7469   Command executi
-00007a50: 6f6e 2066 6169 6c65 6421 7a3f 2020 2020  on failed!z?    
-00007a60: 3e20 4e6f 2063 6f6c 6f72 2063 6f64 6520  > No color code 
-00007a70: 666f 756e 6421 2054 7970 6520 6068 656c  found! Type `hel
-00007a80: 7020 6368 616e 6765 6020 746f 2073 6565  p change` to see
-00007a90: 206d 6f72 6520 696e 666f 2e72 c200 0000   more info.r....
-00007aa0: da01 307a 2a20 2020 203e 2043 6f6c 6f72  ..0z*    > Color
-00007ab0: 2063 6861 6e67 6564 2073 7563 6365 7373   changed success
-00007ac0: 6675 6c6c 7920 746f 2042 4c41 434b 21da  fully to BLACK!.
-00007ad0: 0131 7a2a 2020 2020 3e20 436f 6c6f 7220  .1z*    > Color 
-00007ae0: 6368 616e 6765 6420 7375 6363 6573 7366  changed successf
-00007af0: 756c 6c79 2074 6f20 5748 4954 4521 7a40  ully to WHITE!z@
-00007b00: 2020 2020 5b21 5d20 496e 7661 6c69 6420      [!] Invalid 
-00007b10: 636f 6c6f 7220 636f 6465 2120 5479 7065  color code! Type
-00007b20: 2060 6865 6c70 2063 6861 6e67 6560 2074   `help change` t
-00007b30: 6f20 7365 6520 6d6f 7265 2069 6e66 6f2e  o see more info.
-00007b40: 7a40 2020 2020 3e20 4e6f 2070 686f 6e65  z@    > No phone
-00007b50: 206e 756d 6265 7220 666f 756e 6421 2054   number found! T
-00007b60: 7970 6520 6068 656c 7020 6e75 6d62 6572  ype `help number
-00007b70: 6020 746f 2073 6565 206d 6f72 6520 696e  ` to see more in
-00007b80: 666f 7a31 2020 2020 5b2b 5d20 5065 7266  foz1    [+] Perf
-00007b90: 6f72 6d69 6e67 2072 6576 6572 7365 2070  orming reverse p
-00007ba0: 686f 6e65 206e 756d 6265 7220 6c6f 6f6b  hone number look
-00007bb0: 7570 2e2e 2e7a 3a20 2020 203e 204e 6f20  up...z:    > No 
-00007bc0: 6970 2061 6464 7265 7373 2066 6f75 6e64  ip address found
-00007bd0: 2120 5479 7065 2060 6865 6c70 2069 7060  ! Type `help ip`
-00007be0: 2074 6f20 7365 6520 6d6f 7265 2069 6e66   to see more inf
-00007bf0: 6f7a 2f20 2020 205b 2b5d 2050 6572 666f  oz/    [+] Perfo
-00007c00: 726d 696e 6720 7265 7665 7273 6520 6970  rming reverse ip
-00007c10: 2061 6464 7265 7373 206c 6f6f 6b75 702e   address lookup.
-00007c20: 2e2e 2923 da0b 7369 6c65 6e74 5f6d 6f64  ..)#..silent_mod
-00007c30: 6572 3700 0000 7275 0000 0072 7600 0000  er7...ru...rv...
-00007c40: 723b 0000 0072 8100 0000 da08 6765 746c  r;...r......getl
-00007c50: 6f67 696e 723f 0000 0072 4000 0000 7293  oginr?...r@...r.
-00007c60: 0000 00da 086e 6f64 656e 616d 65da 0773  .....nodename..s
-00007c70: 7973 6e61 6d65 da06 7073 7574 696c 5a0e  ysname..psutilZ.
-00007c80: 7669 7274 7561 6c5f 6d65 6d6f 7279 da07  virtual_memory..
-00007c90: 7065 7263 656e 745a 0b63 7075 5f70 6572  percentZ.cpu_per
-00007ca0: 6365 6e74 da0a 6469 736b 5f75 7361 6765  cent..disk_usage
-00007cb0: da08 7265 6164 6c69 6e65 da0e 7061 7273  ..readline..pars
-00007cc0: 655f 616e 645f 6269 6e64 5a0d 7365 745f  e_and_bindZ.set_
-00007cd0: 636f 6d70 6c65 7465 7272 b600 0000 723d  completerr....r=
-00007ce0: 0000 0072 3600 0000 7241 0000 00da 114b  ...r6...rA.....K
-00007cf0: 6579 626f 6172 6449 6e74 6572 7275 7074  eyboardInterrupt
-00007d00: 72a2 0000 0072 1200 0000 7213 0000 0072  r....r....r....r
-00007d10: 7700 0000 7285 0000 0072 a900 0000 72aa  w...r....r....r.
-00007d20: 0000 0072 9c00 0000 7248 0000 0072 7c00  ...r....rH...r|.
-00007d30: 0000 2920 7206 0000 005a 0763 7274 5f65  ..) r....Z.crt_e
-00007d40: 7870 5a08 6578 705f 696e 666f da04 7573  xpZ.exp_info..us
-00007d50: 6572 da08 686f 7374 6e61 6d65 7299 0000  er..hostnamer...
-00007d60: 005a 0372 616d 5a03 6370 755a 0464 6973  .Z.ramZ.cpuZ.dis
-00007d70: 6bda 0376 6572 5a07 7379 7369 6e66 6f72  k..verZ.sysinfor
-00007d80: 0200 0000 7296 0000 005a 0963 6d64 5f63  ....r....Z.cmd_c
-00007d90: 6f6c 6f72 5a09 6372 745f 636f 6c6f 72da  olorZ.crt_color.
-00007da0: 0363 6d64 5a09 6865 6c70 5f68 656c 705a  .cmdZ.help_helpZ
-00007db0: 0965 7869 745f 6865 6c70 5a09 646f 726b  .exit_helpZ.dork
-00007dc0: 5f68 656c 705a 0865 7870 5f68 656c 705a  _helpZ.exp_helpZ
-00007dd0: 0a63 6865 636b 5f68 656c 705a 0a63 6c65  .check_helpZ.cle
-00007de0: 6172 5f68 656c 705a 0973 6176 655f 6865  ar_helpZ.save_he
-00007df0: 6c70 5a0a 7368 656c 6c5f 6865 6c70 5a09  lpZ.shell_helpZ.
-00007e00: 696e 666f 5f68 656c 705a 0b63 6861 6e67  info_helpZ.chang
-00007e10: 655f 6865 6c70 5a0b 6e75 6d62 6572 5f68  e_helpZ.number_h
-00007e20: 656c 705a 0a65 6d61 696c 5f68 656c 705a  elpZ.email_helpZ
-00007e30: 0769 705f 6865 6c70 5a09 7075 626c 6963  .ip_helpZ.public
-00007e40: 5f69 705a 0865 7865 635f 636d 64da 066f  _ipZ.exec_cmd..o
-00007e50: 7574 7075 7472 1500 0000 7215 0000 0072  utputr....r....r
-00007e60: 1600 0000 da0e 636f 6e74 726f 6c5f 6365  ......control_ce
-00007e70: 6e74 6572 9b02 0000 73b0 0100 0000 0526  nter....s......&
-00007e80: 0908 0708 0204 0f30 0134 0134 0138 0134  .......0.4.4.8.4
-00007e90: 013c 021c 0202 0402 fc04 0502 fb04 0602  .<..............
-00007ea0: fa04 0702 f904 0802 f804 0902 f704 1002  ................
-00007eb0: f008 1704 1f04 040a 010a 0308 0108 0528  ...............(
-00007ec0: 020a 0108 0104 010c 0112 0112 010c 010a  ................
-00007ed0: 0108 0104 050c 0114 0108 0104 040c 010a  ................
-00007ee0: 0108 0104 040c 010a 0108 0104 040c 010a  ................
-00007ef0: 0108 0104 040c 010a 0108 0104 040c 010a  ................
-00007f00: 0108 0104 050a 0112 0108 0104 050a 010a  ................
-00007f10: 0108 0104 040a 010a 0108 0104 080a 010a  ................
-00007f20: 0108 0104 050a 010a 0108 0102 0306 fd08  ................
-00007f30: 050a 010a 0108 0104 050a 0208 0112 0208  ................
-00007f40: 0110 0108 0314 011c 0108 010a 0108 0104  ................
-00007f50: 0112 011a 010a 0108 0104 010c 010a 0112  ................
-00007f60: 0102 010a 0110 0102 0116 0106 0102 0110  ................
-00007f70: 0106 0102 0110 0106 0116 0106 0116 010c  ................
-00007f80: 0106 0110 0110 010e 0108 010a 0108 0104  ................
-00007f90: 011e 010a 0112 010a 0110 010a 020a 010a  ................
-00007fa0: 0208 0108 010a 0108 0104 0114 0112 0112  ................
-00007fb0: 010c 0110 0108 020a 010a 0112 010a 0210  ................
-00007fc0: 010a 0208 0110 0108 010a 0108 0104 010c  ................
-00007fd0: 010a 0108 0104 0114 0112 0112 010c 010a  ................
-00007fe0: 0108 0108 0112 010a 0108 0108 0112 0208  ................
-00007ff0: 0112 0208 0110 0108 030a 0108 0114 0112  ................
-00008000: 0112 010c 0112 010a 010a 020a 0208 0112  ................
-00008010: 010a 0108 0112 0112 0112 010c 0112 010a  ................
-00008020: 010a 020a 0208 0112 0408 0110 0372 d400  .............r..
-00008030: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
-00008040: 0000 000b 0000 0043 0000 0073 9800 0000  .......C...s....
-00008050: 7a24 7400 6a01 6401 1900 6402 6b02 731e  z$t.j.d...d.k.s.
-00008060: 7400 6a01 6401 1900 6403 6b02 7222 6404  t.j.d...d.k.r"d.
-00008070: 6102 5700 6e12 0400 7403 7936 0100 0100  a.W.n...t.y6....
-00008080: 0100 5900 6e02 3000 7402 7342 7404 8300  ..Y.n.0.t.sBt...
-00008090: 0100 7a0a 7405 8300 0100 5700 6e46 0400  ..z.t.....W.nF..
-000080a0: 7406 7992 0100 0100 0100 7407 8300 0100  t.y.......t.....
-000080b0: 7402 738e 7408 6405 6401 6406 7409 a00a  t.s.t.d.d.d.t...
-000080c0: 6407 6408 6702 a101 6703 6404 6404 6404  d.d.g...g.d.d.d.
-000080d0: 6404 6409 8d06 0100 740b 8300 0100 5900  d.d.....t.....Y.
-000080e0: 6e02 3000 6400 5300 290a 4e72 1e00 0000  n.0.d.S.).Nr....
-000080f0: 7a02 2d73 7a08 2d2d 7369 6c65 6e74 547a  z.-sz.--silentTz
-00008100: 265b 235d 2054 6572 6d69 6e61 7469 6e67  &[#] Terminating
-00008110: 2060 5048 304d 4245 5260 2066 7261 6d65   `PH0MBER` frame
-00008120: 776f 726b 2e2e 2e72 1f00 0000 7227 0000  work...r....r'..
-00008130: 0072 2000 0000 2905 7222 0000 0072 2300  .r ...).r"...r#.
-00008140: 0000 7288 0000 0072 8700 0000 7289 0000  ..r....r....r...
-00008150: 0029 0cda 0373 7973 da04 6172 6776 72c5  .)...sys..argvr.
-00008160: 0000 00da 0a49 6e64 6578 4572 726f 7272  .....IndexErrorr
-00008170: ab00 0000 72d4 0000 0072 ce00 0000 7241  ....r....r....rA
-00008180: 0000 0072 3700 0000 7275 0000 0072 7600  ...r7...ru...rv.
-00008190: 0000 7203 0000 0072 1500 0000 7215 0000  ..r....r....r...
-000081a0: 0072 1500 0000 7216 0000 00da 046d 6169  .r....r......mai
-000081b0: 6e0d 0400 0073 1a00 0000 0005 0201 1c01  n....s..........
-000081c0: 0801 0c01 0603 0a03 0201 0a01 0c01 0601  ................
-000081d0: 0401 2401 72d8 0000 0029 1772 1200 0000  ..$.r....).r....
-000081e0: 7281 0000 0072 d500 0000 7275 0000 0072  r....r....ru...r
-000081f0: 9000 0000 72cc 0000 0072 3800 0000 72c9  ....r....r8...r.
-00008200: 0000 0072 a000 0000 7235 0000 0072 b200  ...r....r5...r..
-00008210: 0000 7236 0000 0072 c500 0000 7217 0000  ..r6...r....r...
-00008220: 0072 4800 0000 727c 0000 0072 3700 0000  .rH...r|...r7...
-00008230: 729c 0000 0072 a200 0000 72ab 0000 0072  r....r....r....r
-00008240: b600 0000 72d4 0000 0072 d800 0000 7215  ....r....r....r.
-00008250: 0000 0072 1500 0000 7215 0000 0072 1600  ...r....r....r..
-00008260: 0000 da08 3c6d 6f64 756c 653e 1f00 0000  ....<module>....
-00008270: 7336 0000 0008 0108 0108 0108 0108 0108  s6..............
-00008280: 0108 0108 0108 0108 0408 0104 0104 0508  ................
-00008290: 0908 7f00 0808 7f00 7f00 7024 1b08 1f08  ..........p$....
-000082a0: 1c08 0a08 0a08 7f00 7f00 74              ..........t
+000030e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 7c0a 2020  ------------|.  
+000030f0: 2020 7c20 1b5b 313b 3439 3b39 376d 436f    | .[1;49;97mCo
+00003100: 756e 7472 7920 4361 7069 7461 6c1b 5b30  untry Capital.[0
+00003110: 6d20 2020 2020 7c20 7a2d 207c 0a20 2020  m     | z- |.   
+00003120: 207c 201b 5b31 3b34 393b 3937 6d43 6f6e   | .[1;49;97mCon
+00003130: 7469 6e65 6e74 1b5b 306d 2020 2020 2020  tinent.[0m      
+00003140: 2020 2020 207c 207a 2d20 7c0a 2020 2020       | z- |.    
+00003150: 7c20 1b5b 313b 3439 3b39 376d 5368 6172  | .[1;49;97mShar
+00003160: 696e 6720 426f 7264 6572 2077 6974 681b  ing Border with.
+00003170: 5b30 6d20 7c20 7a2d 207c 0a20 2020 207c  [0m | z- |.    |
+00003180: 201b 5b31 3b34 393b 3937 6d46 6c61 6720   .[1;49;97mFlag 
+00003190: 456d 6f6a 691b 5b30 6d20 2020 2020 2020  Emoji.[0m       
+000031a0: 2020 207c 207a 6a20 7c0a 2020 2020 7c2d     | zj |.    |-
+000031b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000031c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000031d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000031e0: 2d2d 2d2d 2d7c 0a20 2020 207c 201b 5b31  -----|.    | .[1
+000031f0: 3b34 393b 3937 6d54 696d 657a 6f6e 651b  ;49;97mTimezone.
+00003200: 5b30 6d20 2020 2020 2020 2020 2020 207c  [0m            |
+00003210: 207a 2d20 7c0a 2020 2020 7c20 1b5b 313b   z- |.    | .[1;
+00003220: 3439 3b39 376d 5469 6d65 7a6f 6e65 2041  49;97mTimezone A
+00003230: 6262 721b 5b30 6d20 2020 2020 2020 7c20  bbr.[0m       | 
+00003240: 7a2d 207c 0a20 2020 207c 201b 5b31 3b34  z- |.    | .[1;4
+00003250: 393b 3937 6d54 696d 657a 6f6e 6520 6973  9;97mTimezone is
+00003260: 2044 5354 1b5b 306d 2020 2020 207c 207a   DST.[0m     | z
+00003270: 2d20 7c0a 2020 2020 7c20 1b5b 313b 3439  - |.    | .[1;49
+00003280: 3b39 376d 5469 6d65 7a6f 6e65 204f 6666  ;97mTimezone Off
+00003290: 7365 741b 5b30 6d20 2020 2020 7c20 7a2d  set.[0m     | z-
+000032a0: 207c 0a20 2020 207c 201b 5b31 3b34 393b   |.    | .[1;49;
+000032b0: 3937 6d54 696d 657a 6f6e 6520 5554 431b  97mTimezone UTC.
+000032c0: 5b30 6d20 2020 2020 2020 207c 207a 2d20  [0m        | z- 
+000032d0: 7c0a 2020 2020 7c20 1b5b 313b 3439 3b39  |.    | .[1;49;9
+000032e0: 376d 4375 7272 656e 7420 5469 6d65 1b5b  7mCurrent Time.[
+000032f0: 306d 2020 2020 2020 2020 7c20 7a2d 207c  0m        | z- |
+00003300: 0a20 2020 207c 201b 5b31 3b34 393b 3937  .    | .[1;49;97
+00003310: 6d44 6f6d 6169 6e1b 5b30 6d20 2020 2020  mDomain.[0m     
+00003320: 2020 2020 2020 2020 207c 2029 1072 3d00           | ).r=.
+00003330: 0000 723e 0000 0072 1d00 0000 723f 0000  ..r>...r....r?..
+00003340: 0072 4000 0000 7242 0000 0072 4600 0000  .r@...rB...rF...
+00003350: 7247 0000 0072 1800 0000 7219 0000 0072  rG...r....r....r
+00003360: 1600 0000 7217 0000 00da 046a 736f 6eda  ....r......json.
+00003370: 0b73 7461 7475 735f 636f 6465 da09 4578  .status_code..Ex
+00003380: 6365 7074 696f 6e72 4800 0000 2936 5a0a  ceptionrH...)6Z.
+00003390: 6970 5f61 6464 7265 7373 5a0c 6970 5f61  ip_addressZ.ip_a
+000033a0: 6464 7265 7373 6573 7254 0000 005a 0a72  ddressesrT...Z.r
+000033b0: 616e 646f 6d5f 6170 69da 0872 6573 706f  andom_api..respo
+000033c0: 6e73 655a 0d72 6573 706f 6e73 655f 6a73  nseZ.response_js
+000033d0: 6f6e 724d 0000 0072 5800 0000 7259 0000  onrM...rX...rY..
+000033e0: 005a 0a72 6567 696f 6e43 6f64 6572 5a00  .Z.regionCoderZ.
+000033f0: 0000 725b 0000 0072 5c00 0000 721e 0000  ..r[...r\...r...
+00003400: 0072 6800 0000 7269 0000 0072 6a00 0000  .rh...ri...rj...
+00003410: 720c 0000 0072 4e00 0000 da01 6572 6000  r....rN.....er`.
+00003420: 0000 7261 0000 0072 4c00 0000 7262 0000  ..ra...rL...rb..
+00003430: 0072 4a00 0000 7263 0000 0072 6400 0000  .rJ...rc...rd...
+00003440: 7265 0000 0072 6600 0000 7267 0000 0072  re...rf...rg...r
+00003450: 6b00 0000 726c 0000 0072 6d00 0000 726e  k...rl...rm...rn
+00003460: 0000 0072 6f00 0000 7270 0000 0072 7100  ...ro...rp...rq.
+00003470: 0000 7272 0000 005a 0769 705f 7479 7065  ..rr...Z.ip_type
+00003480: 7274 0000 0072 7500 0000 7276 0000 0072  rt...ru...rv...r
+00003490: 7700 0000 7278 0000 005a 0866 6c61 675f  w...rx...Z.flag_
+000034a0: 696d 675a 0a66 6c61 675f 656d 6f6a 695a  imgZ.flag_emojiZ
+000034b0: 1266 6c61 675f 656d 6f6a 695f 756e 6963  .flag_emoji_unic
+000034c0: 6f64 6572 7b00 0000 5a0b 7469 6d65 7a6f  oder{...Z.timezo
+000034d0: 6e65 5f69 645a 0d74 696d 657a 6f6e 655f  ne_idZ.timezone_
+000034e0: 6162 6272 5a0f 7469 6d65 7a6f 6e65 5f69  abbrZ.timezone_i
+000034f0: 735f 6473 745a 0f74 696d 657a 6f6e 655f  s_dstZ.timezone_
+00003500: 6f66 6673 6574 5a0c 7469 6d65 7a6f 6e65  offsetZ.timezone
+00003510: 5f75 7463 5a15 7469 6d65 7a6f 6e65 5f63  _utcZ.timezone_c
+00003520: 7572 7265 6e74 5f74 696d 6572 1b00 0000  urrent_timer....
+00003530: 721b 0000 0072 1c00 0000 da09 6970 5f6c  r....r......ip_l
+00003540: 6f6f 6b75 70d1 0000 0073 9002 0000 0003  ookup....s......
+00003550: 0403 1201 0601 1201 0403 1a01 1403 0c01  ................
+00003560: 1001 0403 1e01 2004 04ff 0405 0e03 0a01  ...... .........
+00003570: 0402 1401 0803 1a01 0801 0801 0801 0801  ................
+00003580: 0801 0801 0801 0801 0801 0801 0801 0a02  ................
+00003590: 0803 2001 2001 2001 2001 2001 2001 2001  .. . . . . . . .
+000035a0: 2001 2001 2001 2001 2003 0202 02fe 0406   . . . . .......
+000035b0: 02fa 0407 02f9 0408 02f8 0409 02f7 040a  ................
+000035c0: 02f6 040c 02f4 040d 02f3 040e 02f2 040f  ................
+000035d0: 02f1 0411 02ef 0412 02ee 0815 0801 1002  ................
+000035e0: 1001 0801 0202 02fe 0807 0801 2603 0a01  ............&...
+000035f0: 0402 1401 0803 0c01 0801 0801 0801 0801  ................
+00003600: 0801 0801 0801 0801 0801 0801 0801 0801  ................
+00003610: 0801 0801 0801 0801 0801 0801 0801 0801  ................
+00003620: 0801 0801 0801 0801 0801 0801 0a02 0803  ................
+00003630: 2001 2001 2001 2001 2001 2001 2001 2001   . . . . . . . .
+00003640: 2001 2001 2001 2001 2001 2001 2001 2001   . . . . . . . .
+00003650: 2001 2001 2001 2001 2001 2001 2001 2001   . . . . . . . .
+00003660: 2001 2001 2003 0202 02fe 0406 02fa 0407   . . ...........
+00003670: 02f9 0409 02f7 040a 02f6 040b 02f5 040c  ................
+00003680: 02f4 040d 02f3 040e 02f2 040f 02f1 0410  ................
+00003690: 02f0 0412 02ee 0413 02ed 0414 02ec 0415  ................
+000036a0: 02eb 0416 02ea 0417 02e9 0418 02e8 0419  ................
+000036b0: 02e7 041a 02e6 041c 02e4 041d 02e3 041e  ................
+000036c0: 02e2 041f 02e1 0420 02e0 0422 02de 0423  ....... ..."...#
+000036d0: 02dd 0826 0801 1002 0601 0202 02fe 0807  ...&............
+000036e0: 0801 1603 0a01 0402 1401 0803 1a01 0801  ................
+000036f0: 0801 0801 0801 0801 0801 0801 0801 0801  ................
+00003700: 0801 0801 0801 0801 0801 0801 0801 0c01  ................
+00003710: 0c01 0c01 0c01 0c01 0c01 0c01 0c01 0c01  ................
+00003720: 0c01 0c01 0c01 0e02 0803 2001 2001 2001  .......... . . .
+00003730: 2001 2001 2001 2001 2001 2001 2001 2001   . . . . . . . .
+00003740: 2001 2001 2001 2001 2001 2001 2001 2001   . . . . . . . .
+00003750: 2001 2001 2001 2001 2001 2001 2001 2001   . . . . . . . .
+00003760: 2001 2003 0202 02fe 0406 02fa 0408 02f8   . .............
+00003770: 0409 02f7 040a 02f6 040b 02f5 040c 02f4  ................
+00003780: 040e 02f2 040f 02f1 0410 02f0 0411 02ef  ................
+00003790: 0412 02ee 0413 02ed 0415 02eb 0416 02ea  ................
+000037a0: 0417 02e9 0418 02e8 041a 02e6 041b 02e5  ................
+000037b0: 041c 02e4 041d 02e3 041e 02e2 041f 02e1  ................
+000037c0: 0421 02df 0422 02de 0423 02dd 0826 0801  .!..."...#...&..
+000037d0: 1002 0601 0202 02fe 0807 0801 1202 7284  ..............r.
+000037e0: 0000 0063 0100 0000 0000 0000 0000 0000  ...c............
+000037f0: 0400 0000 0800 0000 4300 0000 73ec 0000  ........C...s...
+00003800: 0064 0161 0074 0164 027c 009b 0064 039d  .d.a.t.d.|...d..
+00003810: 0367 0064 04a2 0164 0564 068d 0301 0074  .g.d...d.d.....t
+00003820: 0064 077c 009b 0064 089d 0364 0917 0037  .d.|...d...d...7
+00003830: 0061 0074 02a0 0364 0a7c 00a1 0273 5274  .a.t...d.|...sRt
+00003840: 0164 0b67 0064 0ca2 0164 0d8d 0201 0064  .d.g.d...d.....d
+00003850: 0e53 007a 1474 0483 00a0 057c 00a1 017d  .S.z.t.....|...}
+00003860: 0164 057d 0257 006e 1a04 0074 0679 8001  .d.}.W.n...t.y..
+00003870: 0001 0001 0064 0f7d 0164 0e7d 0259 006e  .....d.}.d.}.Y.n
+00003880: 0230 0074 077c 0083 0164 1074 0864 1174  .0.t.|...d.t.d.t
+00003890: 0974 077c 0083 0183 0118 0083 0114 0017  .t.|............
+000038a0: 007d 0074 077c 0183 0164 1074 0864 1274  .}.t.|...d.t.d.t
+000038b0: 0974 077c 0183 0183 0118 0083 0114 0017  .t.|............
+000038c0: 007d 0164 137c 009b 0064 147c 019b 0064  .}.d.|...d.|...d
+000038d0: 159d 057d 0374 0a7c 0383 0101 0074 007c  ...}.t.|.....t.|
+000038e0: 0364 1617 0037 0061 007c 0253 0029 174e  .d...7.a.|.S.).N
+000038f0: 7213 0000 0072 2100 0000 7222 0000 0072  r....r!...r"...r
+00003900: 2300 0000 5472 2700 0000 7a3b 2020 2020  #...Tr'...z;    
+00003910: 1b5b 313b 3439 3b39 336d 5b23 5d20 5265  .[1;49;93m[#] Re
+00003920: 7665 7273 6520 6d61 6320 6164 6472 6573  verse mac addres
+00003930: 7320 6c6f 6f6b 7570 2066 6f72 201b 5b31  s lookup for .[1
+00003940: 3b34 393b 3936 6d72 2a00 0000 722b 0000  ;49;96mr*...r+..
+00003950: 007a 295e 285b 302d 3941 2d46 612d 665d  .z)^([0-9A-Fa-f]
+00003960: 7b32 7d5b 3a2d 5d29 7b35 7d28 5b30 2d39  {2}[:-]){5}([0-9
+00003970: 412d 4661 2d66 5d7b 327d 2924 7a3e 2020  A-Fa-f]{2})$z>  
+00003980: 2020 3e20 496e 7661 6c69 6420 6d61 6320    > Invalid mac 
+00003990: 6164 6472 6573 7320 666f 726d 6174 2120  address format! 
+000039a0: 2845 7861 6d70 6c65 3a20 3030 3a30 303a  (Example: 00:00:
+000039b0: 3030 3a30 303a 3030 3a30 3029 722c 0000  00:00:00:00)r,..
+000039c0: 0072 2e00 0000 46fa 171b 5b31 3b34 393b  .r....F...[1;49;
+000039d0: 3931 6d4e 6f74 2046 6f75 6e64 1b5b 306d  91mNot Found.[0m
+000039e0: 7236 0000 00e9 1f00 0000 e924 0000 0075  r6.........$...u
+000039f0: d300 0000 0a20 2020 20e2 948c e294 80e2  .....    .......
+00003a00: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00003a10: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00003a20: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00003a30: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00003a40: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00003a50: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00003a60: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00003a70: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00003a80: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00003a90: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00003aa0: 900a 2020 2020 7c20 5363 616e 6e65 6420  ..    | Scanned 
+00003ab0: 4d41 4320 4164 6472 6573 733a 201b 5b31  MAC Address: .[1
+00003ac0: 3b34 393b 3936 6d7a e21b 5b30 6d20 7c0a  ;49;96mz..[0m |.
+00003ad0: 2020 2020 7c2d 2d2d 2d2d 2d2d 2d2d 2d2d      |-----------
+00003ae0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00003af0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00003b00: 2d2d 2d2d 2d2d 2d2d 2d2d 2d7c 0a20 2020  -----------|.   
+00003b10: 207c 2049 4e46 4f52 4d41 5449 4f4e 2020   | INFORMATION  
+00003b20: 207c 2044 4553 4352 4950 5449 4f4e 2020   | DESCRIPTION  
+00003b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003b40: 2020 2020 2020 2020 7c0a 2020 2020 7c2d          |.    |-
+00003b50: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00003b60: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00003b70: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00003b80: 2d2d 2d2d 2d7c 0a20 2020 207c 201b 5b31  -----|.    | .[1
+00003b90: 3b34 393b 3937 6d56 656e 646f 721b 5b30  ;49;97mVendor.[0
+00003ba0: 6d20 2020 2020 2020 207c 2072 5f00 0000  m        | r_...
+00003bb0: 723a 0000 0029 0b72 3d00 0000 723e 0000  r:...).r=...r>..
+00003bc0: 0072 3f00 0000 7240 0000 0072 0200 0000  .r?...r@...r....
+00003bd0: da06 6c6f 6f6b 7570 da08 4b65 7945 7272  ..lookup..KeyErr
+00003be0: 6f72 7242 0000 0072 4600 0000 7247 0000  orrB...rF...rG..
+00003bf0: 0072 4800 0000 2904 da0b 6d61 635f 6164  .rH...)...mac_ad
+00003c00: 6472 6573 73da 0676 656e 646f 72da 0762  dress..vendor..b
+00003c10: 6f6c 5f76 616c 724e 0000 0072 1b00 0000  ol_valrN...r....
+00003c20: 721b 0000 0072 1c00 0000 da0a 6d61 635f  r....r......mac_
+00003c30: 6c6f 6f6b 7570 3502 0000 732c 0000 0000  lookup5...s,....
+00003c40: 0504 031a 0114 030c 0110 0104 0302 010c  ................
+00003c50: 0108 010c 0104 010a 0320 0120 0302 0202  ......... . ....
+00003c60: fe04 0602 fa08 0908 010c 0272 8d00 0000  ...........r....
+00003c70: 6301 0000 0000 0000 0000 0000 0009 0000  c...............
+00003c80: 000a 0000 0043 0000 0073 8002 0000 6401  .....C...s....d.
+00003c90: 6100 7401 6402 6700 6403 a201 6404 6405  a.t.d.g.d...d.d.
+00003ca0: 8d03 0100 7402 8300 7332 7401 6406 6700  ....t...s2t.d.g.
+00003cb0: 6407 a201 6404 6405 8d03 0100 6408 5300  d...d.d.....d.S.
+00003cc0: 7401 6409 7c00 9b00 640a 9d03 6700 6403  t.d.|...d...g.d.
+00003cd0: a201 6404 6405 8d03 0100 7400 640b 7c00  ..d.d.....t.d.|.
+00003ce0: 9b00 640c 9d03 640d 1700 3700 6100 7403  ..d...d...7.a.t.
+00003cf0: a004 640e 7c00 a102 7380 7401 640f 6700  ..d.|...s.t.d.g.
+00003d00: 6407 a201 6410 8d02 0100 6408 5300 7a12  d...d.....d.S.z.
+00003d10: 7405 a005 7c00 a101 7d01 6404 7d02 5700  t...|...}.d.}.W.
+00003d20: 6e10 0100 0100 0100 6408 7d02 5900 6e02  n.......d.}.Y.n.
+00003d30: 3000 7406 7c00 8301 6411 7407 6412 7408  0.t.|...d.t.d.t.
+00003d40: 7406 7c00 8301 8301 1800 8301 1400 1700  t.|.............
+00003d50: 7d00 6413 7c00 9b00 6414 9d03 7d03 7c02  }.d.|...d...}.|.
+00003d60: 9002 7240 7c01 a009 a100 4400 9001 5d5c  ..r@|.....D...]\
+00003d70: 5c02 7d04 7d05 7c04 6415 6b02 72f2 71de  \.}.}.|.d.k.r.q.
+00003d80: 7c04 6416 6b02 72fe 6417 7d04 7c04 6418  |.d.k.r.d.}.|.d.
+00003d90: 6b02 9001 720c 6419 7d04 7c04 a00a 641a  k...r.d.}.|...d.
+00003da0: 6411 a102 a00b a100 7d04 740c 7c05 8301  d.......}.t.|...
+00003db0: 740d 6b02 9001 72e6 7406 7c04 8301 6411  t.k...r.t.|...d.
+00003dc0: 7407 641b 7408 7406 7c04 8301 8301 1800  t.d.t.t.|.......
+00003dd0: 8301 1400 1700 7d04 7406 7c05 641c 1900  ......}.t.|.d...
+00003de0: 8301 6411 7407 6412 7408 7406 7c05 641c  ..d.t.d.t.t.|.d.
+00003df0: 1900 8301 8301 1800 8301 1400 1700 7d06  ..............}.
+00003e00: 7c03 641d 7c04 9b00 641e 7c06 9b00 641f  |.d.|...d.|...d.
+00003e10: 9d05 3700 7d03 7408 7c05 8301 6420 6b04  ..7.}.t.|...d k.
+00003e20: 9002 723c 740e 6420 7408 7c05 8301 8302  ..r<t.d t.|.....
+00003e30: 4400 5d3e 7d07 7406 7c05 7c07 1900 8301  D.]>}.t.|.|.....
+00003e40: 6411 7407 6412 7408 7406 7c05 7c07 1900  d.t.d.t.t.|.|...
+00003e50: 8301 8301 1800 8301 1400 1700 7d08 7c03  ............}.|.
+00003e60: 6421 7c08 9b00 641f 9d03 3700 7d03 9001  d!|...d...7.}...
+00003e70: 71a4 71de 7406 7c04 8301 6411 7407 641b  q.q.t.|...d.t.d.
+00003e80: 7408 7406 7c04 8301 8301 1800 8301 1400  t.t.|...........
+00003e90: 1700 7d04 7406 7c05 8301 6411 7407 6412  ..}.t.|...d.t.d.
+00003ea0: 7408 7406 7c05 8301 8301 1800 8301 1400  t.t.|...........
+00003eb0: 1700 7d05 7c03 641d 7c04 9b00 641e 7c05  ..}.|.d.|...d.|.
+00003ec0: 9b00 641f 9d05 3700 7d03 71de 6e20 7c03  ..d...7.}.q.n |.
+00003ed0: 6422 6411 7407 6412 7408 6423 8301 1800  d"d.t.d.t.d#....
+00003ee0: 8301 1400 9b00 641f 9d03 3700 7d03 7c03  ......d...7.}.|.
+00003ef0: 6424 3700 7d03 740f 7c03 8301 0100 7400  d$7.}.t.|.....t.
+00003f00: 7c03 6425 1700 3700 6100 7c02 5300 2926  |.d%..7.a.|.S.)&
+00003f10: 4e72 1300 0000 7250 0000 0072 2300 0000  Nr....rP...r#...
+00003f20: 5472 2700 0000 7251 0000 0072 2c00 0000  Tr'...rQ...r,...
+00003f30: 4672 2100 0000 7222 0000 007a 3520 2020  Fr!...r"...z5   
+00003f40: 201b 5b31 3b34 393b 3933 6d5b 235d 2052   .[1;49;93m[#] R
+00003f50: 6576 6572 7365 2077 686f 6973 206c 6f6f  everse whois loo
+00003f60: 6b75 7020 666f 7220 1b5b 313b 3439 3b39  kup for .[1;49;9
+00003f70: 366d 722a 0000 0072 2b00 0000 fa2f 5e28  6mr*...r+..../^(
+00003f80: 5b61 2d7a 412d 5a30 2d39 5d2b 282d 5b61  [a-zA-Z0-9]+(-[a
+00003f90: 2d7a 412d 5a30 2d39 5d2b 292a 5c2e 292b  -zA-Z0-9]+)*\.)+
+00003fa0: 5b61 2d7a 412d 5a5d 7b32 2c7d 247a 3320  [a-zA-Z]{2,}$z3 
+00003fb0: 2020 203e 2049 6e76 616c 6964 2064 6f6d     > Invalid dom
+00003fc0: 6169 6e20 666f 726d 6174 2120 2845 7861  ain format! (Exa
+00003fd0: 6d70 6c65 3a20 6578 616d 706c 652e 636f  mple: example.co
+00003fe0: 6d29 722e 0000 0072 3600 0000 7287 0000  m)r....r6...r...
+00003ff0: 0075 ce00 0000 0a20 2020 20e2 948c e294  .u.....    .....
+00004000: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00004010: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00004020: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00004030: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00004040: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00004050: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00004060: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00004070: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00004080: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00004090: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+000040a0: e294 900a 2020 2020 7c20 5363 616e 6e65  ....    | Scanne
+000040b0: 6420 446f 6d61 696e 3a20 1b5b 313b 3439  d Domain: .[1;49
+000040c0: 3b39 366d 7abd 1b5b 306d 207c 0a20 2020  ;96mz..[0m |.   
+000040d0: 207c 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   |--------------
+000040e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000040f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00004100: 2d2d 2d2d 2d2d 2d2d 7c0a 2020 2020 7c20  --------|.    | 
+00004110: 494e 464f 524d 4154 494f 4e20 2020 7c20  INFORMATION   | 
+00004120: 4445 5343 5249 5054 494f 4e20 2020 2020  DESCRIPTION     
+00004130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004140: 2020 2020 207c 0a20 2020 207c 2d2d 2d2d       |.    |----
+00004150: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00004160: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00004170: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00004180: 2d2d 7c72 5600 0000 5a0f 6578 7069 7261  --|rV...Z.expira
+00004190: 7469 6f6e 5f64 6174 655a 0b65 7870 6972  tion_dateZ.expir
+000041a0: 795f 6461 7465 5a16 7265 6769 7374 7261  y_dateZ.registra
+000041b0: 6e74 5f70 6f73 7461 6c5f 636f 6465 5a0b  nt_postal_codeZ.
+000041c0: 706f 7374 616c 5f63 6f64 65da 015f e90d  postal_code.._..
+000041d0: 0000 0072 0100 0000 7a11 0a20 2020 207c  ...r....z..    |
+000041e0: 201b 5b31 3b34 393b 3937 6d7a 071b 5b30   .[1;49;97mz..[0
+000041f0: 6d20 7c20 7a02 207c 7224 0000 007a 170a  m | z. |r$...z..
+00004200: 2020 2020 7c20 2020 2020 2020 2020 2020      |           
+00004210: 2020 2020 7c20 7a3c 0a20 2020 207c 201b      | z<.    | .
+00004220: 5b31 3b34 393b 3937 6d49 6e66 6f72 6d61  [1;49;97mInforma
+00004230: 7469 6f6e 1b5b 306d 2020 207c 201b 5b31  tion.[0m   | .[1
+00004240: 3b34 393b 3931 6d4e 6f74 2046 6f75 6e64  ;49;91mNot Found
+00004250: 1b5b 306d fa09 4e6f 7420 466f 756e 6475  .[0m..Not Foundu
+00004260: ad00 0000 0a20 2020 20e2 9494 e294 80e2  .....    .......
+00004270: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00004280: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00004290: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+000042a0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+000042b0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+000042c0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+000042d0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+000042e0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+000042f0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00004300: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00004310: 9872 3a00 0000 2910 723d 0000 0072 3e00  .r:...).r=...r>.
+00004320: 0000 721d 0000 0072 3f00 0000 7240 0000  ..r....r?...r@..
+00004330: 0072 1200 0000 7242 0000 0072 4600 0000  .r....rB...rF...
+00004340: 7247 0000 00da 0569 7465 6d73 7245 0000  rG.....itemsrE..
+00004350: 00da 0a63 6170 6974 616c 697a 6572 7300  ...capitalizers.
+00004360: 0000 da04 6c69 7374 da05 7261 6e67 6572  ....list..ranger
+00004370: 4800 0000 2909 727b 0000 005a 0a77 686f  H...).r{...Z.who
+00004380: 6973 5f69 6e66 6f72 8c00 0000 724e 0000  is_infor....rN..
+00004390: 00da 036b 6579 da05 7661 6c75 655a 0776  ...key..valueZ.v
+000043a0: 616c 7565 5f31 da01 695a 0776 616c 7565  alue_1..iZ.value
+000043b0: 5f32 721b 0000 0072 1b00 0000 721c 0000  _2r....r....r...
+000043c0: 00da 0c77 686f 6973 5f6c 6f6f 6b75 7061  ...whois_lookupa
+000043d0: 0200 0073 5200 0000 0003 0403 1201 0601  ...sR...........
+000043e0: 1201 0403 1a01 1403 0c01 1001 0403 0201  ................
+000043f0: 0a01 0801 0601 0a03 2003 0202 02fe 0808  ........ .......
+00004400: 0602 1202 0a01 0c01 0e03 1003 0e01 2001  .............. .
+00004410: 2801 1601 0e01 1201 2801 1602 2001 2001  (.......(... . .
+00004420: 1a02 2003 0802 0801 0c02 7299 0000 0063  .. .......r....c
+00004430: 0100 0000 0000 0000 0000 0000 0500 0000  ................
+00004440: 0900 0000 4300 0000 73d2 0100 0064 0161  ....C...s....d.a
+00004450: 0074 0164 0267 0064 03a2 0164 0464 058d  .t.d.g.d...d.d..
+00004460: 0301 0074 0283 0073 3274 0164 0667 0064  ...t...s2t.d.g.d
+00004470: 07a2 0164 0464 058d 0301 0064 0853 0074  ...d.d.....d.S.t
+00004480: 0164 097c 009b 0064 0a9d 0367 0064 03a2  .d.|...d...g.d..
+00004490: 0164 0464 058d 0301 0074 03a0 0464 0b7c  .d.d.....t...d.|
+000044a0: 00a1 0272 e674 0064 0c7c 009b 0064 0d9d  ...r.t.d.|...d..
+000044b0: 0364 0e17 0037 0061 007c 0064 0f74 0564  .d...7.a.|.d.t.d
+000044c0: 1074 067c 0083 0118 0083 0114 0017 007d  .t.|...........}
+000044d0: 0164 117c 019b 0064 129d 037d 027a 2e74  .d.|...d...}.z.t
+000044e0: 07a0 087c 00a1 017d 0374 097c 0383 0164  ...|...}.t.|...d
+000044f0: 0f74 0564 1074 0674 097c 0383 0183 0118  .t.d.t.t.|......
+00004500: 0083 0114 0017 007d 0357 006e 2401 0001  .......}.W.n$...
+00004510: 0001 0064 1364 0f74 0564 1074 0664 1483  ...d.d.t.d.t.d..
+00004520: 0118 0083 0114 0017 007d 0359 006e 0230  .........}.Y.n.0
+00004530: 006e b674 03a0 0464 157c 00a1 0290 0172  .n.t...d.|.....r
+00004540: 8674 0064 167c 009b 0064 0d9d 0364 0e17  .t.d.|...d...d..
+00004550: 0037 0061 007c 0064 0f74 0564 1074 067c  .7.a.|.d.t.d.t.|
+00004560: 0083 0118 0083 0114 0017 007d 0364 177c  ...........}.d.|
+00004570: 039b 0064 189d 037d 027a 3274 07a0 0a7c  ...d...}.z2t...|
+00004580: 00a1 0164 1919 007d 0174 097c 0183 0164  ...d...}.t.|...d
+00004590: 0f74 0564 1074 0674 097c 0183 0183 0118  .t.d.t.t.|......
+000045a0: 0083 0114 0017 007d 0157 006e 2401 0001  .......}.W.n$...
+000045b0: 0001 0064 1364 0f74 0564 1074 0664 1483  ...d.d.t.d.t.d..
+000045c0: 0118 0083 0114 0017 007d 0159 006e 0230  .........}.Y.n.0
+000045d0: 006e 1674 0164 1a67 0064 07a2 0164 0464  .n.t.d.g.d...d.d
+000045e0: 058d 0301 0064 0853 0064 1b7c 039b 0064  .....d.S.d.|...d
+000045f0: 1c7c 019b 0064 1d9d 057d 0474 0b64 1e7c  .|...d...}.t.d.|
+00004600: 0217 007c 0417 0083 0101 0074 0064 1e7c  ...|.......t.d.|
+00004610: 0217 007c 0417 0037 0061 0064 0453 0029  ...|...7.a.d.S.)
+00004620: 1f4e 7213 0000 0072 5000 0000 7223 0000  .Nr....rP...r#..
+00004630: 0054 7227 0000 0072 5100 0000 722c 0000  .Tr'...rQ...r,..
+00004640: 0046 7221 0000 0072 2200 0000 728e 0000  .Fr!...r"...r...
+00004650: 007a 2b20 2020 201b 5b31 3b34 393b 3933  .z+    .[1;49;93
+00004660: 6d5b 235d 2044 4e53 206c 6f6f 6b75 7020  m[#] DNS lookup 
+00004670: 666f 7220 1b5b 313b 3439 3b39 366d 722a  for .[1;49;96mr*
+00004680: 0000 0072 2b00 0000 7236 0000 0072 8700  ...r+...r6...r..
+00004690: 0000 7a20 2020 2020 7c20 5363 616e 6e65  ..z     | Scanne
+000046a0: 6420 446f 6d61 696e 3a20 1b5b 313b 3439  d Domain: .[1;49
+000046b0: 3b39 366d 7a06 1b5b 306d 207c 7285 0000  ;96mz..[0m |r...
+000046c0: 0072 9100 0000 7a1d 5e28 5b30 2d39 5d7b  .r....z.^([0-9]{
+000046d0: 312c 337d 5c2e 297b 337d 5b30 2d39 5d7b  1,3}\.){3}[0-9]{
+000046e0: 312c 337d 247a 3320 2020 201b 5b31 3b34  1,3}$z3    .[1;4
+000046f0: 393b 3933 6d5b 235d 2052 6576 6572 7365  9;93m[#] Reverse
+00004700: 2044 4e53 206c 6f6f 6b75 7020 666f 7220   DNS lookup for 
+00004710: 1b5b 313b 3439 3b39 366d 7a1c 2020 2020  .[1;49;96mz.    
+00004720: 7c20 5363 616e 6e65 6420 4950 3a20 1b5b  | Scanned IP: .[
+00004730: 313b 3439 3b39 366d 7a0a 1b5b 306d 2020  1;49;96mz..[0m  
+00004740: 2020 207c 7201 0000 007a 2820 2020 203e     |r....z(    >
+00004750: 2049 6e76 616c 6964 2069 7020 6164 6472   Invalid ip addr
+00004760: 6573 7320 6f72 2064 6f6d 6169 6e20 6e61  ess or domain na
+00004770: 6d65 217a dc0a 2020 2020 7c2d 2d2d 2d2d  me!z..    |-----
+00004780: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00004790: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000047a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000047b0: 2d7c 0a20 2020 207c 2049 4e46 4f52 4d41  -|.    | INFORMA
+000047c0: 5449 4f4e 2020 207c 2044 4553 4352 4950  TION   | DESCRIP
+000047d0: 5449 4f4e 2020 2020 2020 2020 2020 2020  TION            
+000047e0: 2020 2020 2020 2020 2020 2020 2020 7c0a                |.
+000047f0: 2020 2020 7c2d 2d2d 2d2d 2d2d 2d2d 2d2d      |-----------
+00004800: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00004810: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00004820: 2d2d 2d2d 2d2d 2d2d 2d2d 2d7c 0a20 2020  -----------|.   
+00004830: 207c 201b 5b31 3b34 393b 3937 6d49 501b   | .[1;49;97mIP.
+00004840: 5b30 6d20 2020 2020 2020 2020 2020 207c  [0m            |
+00004850: 207a 2720 7c0a 2020 2020 7c20 1b5b 313b   z' |.    | .[1;
+00004860: 3439 3b39 376d 446f 6d61 696e 1b5b 306d  49;97mDomain.[0m
+00004870: 2020 2020 2020 2020 7c20 725f 0000 0075          | r_...u
+00004880: ae00 0000 0a20 2020 20e2 948c e294 80e2  .....    .......
+00004890: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+000048a0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+000048b0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+000048c0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+000048d0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+000048e0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+000048f0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00004900: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00004910: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00004920: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00004930: 900a 290c 723d 0000 0072 3e00 0000 721d  ..).r=...r>...r.
+00004940: 0000 0072 3f00 0000 7240 0000 0072 4600  ...r?...r@...rF.
+00004950: 0000 7247 0000 00da 0673 6f63 6b65 74da  ..rG.....socket.
+00004960: 0d67 6574 686f 7374 6279 6e61 6d65 7242  .gethostbynamerB
+00004970: 0000 00da 0d67 6574 686f 7374 6279 6164  .....gethostbyad
+00004980: 6472 7248 0000 0029 055a 0c69 705f 6f72  drrH...).Z.ip_or
+00004990: 5f64 6f6d 6169 6e72 7b00 0000 5a14 6669  _domainr{...Z.fi
+000049a0: 6e61 6c5f 6f75 7470 7574 5f73 6361 6e6e  nal_output_scann
+000049b0: 6564 720c 0000 005a 1666 696e 616c 5f6f  edr....Z.final_o
+000049c0: 7574 7075 745f 7265 6d61 696e 696e 6772  utput_remainingr
+000049d0: 1b00 0000 721b 0000 0072 1c00 0000 da0a  ....r....r......
+000049e0: 646e 735f 6c6f 6f6b 7570 ac02 0000 7344  dns_lookup....sD
+000049f0: 0000 0000 0304 0312 0106 0112 0104 031a  ................
+00004a00: 030c 0114 0118 010c 0102 010a 0124 0106  .............$..
+00004a10: 0120 010e 0114 0118 010c 0102 010e 0124  . .............$
+00004a20: 0106 0120 0212 0104 0502 0402 fc04 0502  ... ............
+00004a30: fb08 0910 0110 0272 9d00 0000 2903 7201  .......r....).r.
+00004a40: 0000 0072 0100 0000 7201 0000 0063 0c00  ...r....r....c..
+00004a50: 0000 0000 0000 0000 0000 0f00 0000 0800  ................
+00004a60: 0000 4300 0000 735e 0100 007c 0972 0a7c  ..C...s^...|.r.|
+00004a70: 0a90 0172 5a74 00a0 01a1 006a 027d 0c7c  ...rZt.....j.}.|
+00004a80: 0472 1e74 0383 0001 007c 0272 2e74 0364  .r.t.....|.r.t.d
+00004a90: 017c 0c14 0083 0101 0074 037c 0764 0264  .|.......t.|.d.d
+00004aa0: 038d 0201 0074 047c 0083 017c 0c6b 0072  .....t.|...|.k.r
+00004ab0: ce74 057c 0c74 047c 0083 0118 0064 041b  .t.|.t.|.....d..
+00004ac0: 0083 017d 0d74 037c 017c 0d14 0064 0264  ...}.t.|.|...d.d
+00004ad0: 038d 0201 0074 0364 057c 0664 0619 009b  .....t.d.|.d....
+00004ae0: 0064 077c 0664 0819 009b 0064 077c 0664  .d.|.d.....d.|.d
+00004af0: 0419 009b 0064 099d 0764 0264 038d 0201  .....d...d.d....
+00004b00: 007c 0b72 a474 067c 0083 017d 0e6e 1074  .|.r.t.|...}.n.t
+00004b10: 0374 077c 0083 0164 0264 038d 0201 0074  .t.|...d.d.....t
+00004b20: 0364 0a64 0264 038d 0201 0074 037c 017c  .d.d.d.....t.|.|
+00004b30: 0d14 0083 0101 006e 5874 0364 057c 0664  .......nXt.d.|.d
+00004b40: 0619 009b 0064 077c 0664 0819 009b 0064  .....d.|.d.....d
+00004b50: 077c 0664 0419 009b 0064 099d 0764 0264  .|.d.....d...d.d
+00004b60: 038d 0201 007c 0b90 0172 0a74 067c 0083  .....|...r.t.|..
+00004b70: 017d 0e6e 1074 0374 077c 0083 0164 0264  .}.n.t.t.|...d.d
+00004b80: 038d 0201 0074 0364 0a64 0264 038d 0201  .....t.d.d.d....
+00004b90: 0074 037c 0864 0264 038d 0201 007c 0390  .t.|.d.d.....|..
+00004ba0: 0172 4474 0364 017c 0c14 0083 0101 007c  .rDt.d.|.......|
+00004bb0: 0590 0172 5074 0383 0001 007c 0b90 0172  ...rPt.....|...r
+00004bc0: 5a7c 0e53 0064 0053 0029 0b4e 7503 0000  Z|.S.d.S.).Nu...
+00004bd0: 00e2 b8ba 7213 0000 0029 01da 0365 6e64  ....r....)...end
+00004be0: 7253 0000 007a 021b 5b72 0100 0000 fa01  rS...z..[r......
+00004bf0: 3b72 2400 0000 da01 6dfa 041b 5b30 6d29  ;r$.....m...[0m)
+00004c00: 08da 026f 73da 1167 6574 5f74 6572 6d69  ...os..get_termi
+00004c10: 6e61 6c5f 7369 7a65 da07 636f 6c75 6d6e  nal_size..column
+00004c20: 7372 4800 0000 7247 0000 0072 4600 0000  srH...rG...rF...
+00004c30: da05 696e 7075 7472 4200 0000 290f da04  ..inputrB...)...
+00004c40: 7465 7874 da06 6365 6e74 6572 da07 6c69  text..center..li
+00004c50: 6e65 5f75 70da 096c 696e 655f 646f 776e  ne_up..line_down
+00004c60: da08 7370 6163 655f 7570 7229 0000 0072  ..space_upr)...r
+00004c70: 2800 0000 da0f 6e6f 726d 616c 7478 745f  (.....normaltxt_
+00004c80: 7374 6172 745a 0d6e 6f72 6d61 6c74 7874  startZ.normaltxt
+00004c90: 5f65 6e64 5a04 6869 6465 5a0c 7665 7262  _endZ.hideZ.verb
+00004ca0: 6f73 655f 6d6f 6465 da0a 696e 7075 745f  ose_mode..input_
+00004cb0: 6d6f 6465 da05 7769 6474 685a 096e 6577  mode..widthZ.new
+00004cc0: 5f77 6964 7468 5a09 696e 7075 745f 7661  _widthZ.input_va
+00004cd0: 7272 1b00 0000 721b 0000 0072 1c00 0000  rr....r....r....
+00004ce0: 723e 0000 00e4 0200 0073 2a00 0000 0001  r>.......s*.....
+00004cf0: 0a02 0a03 0a01 1002 0c02 0c01 1401 1001  ................
+00004d00: 2c01 0e01 1001 0c01 0e02 2c01 1001 1001  ,.........,.....
+00004d10: 0c02 0c02 1201 0c02 723e 0000 0063 0100  ........r>...c..
+00004d20: 0000 0000 0000 0000 0000 0900 0000 0b00  ................
+00004d30: 0000 4300 0000 7342 0100 0090 017a 1a7c  ..C...sB.....z.|
+00004d40: 0064 0117 0074 0074 01a0 0264 02a1 0183  .d...t.t...d....
+00004d50: 0117 0064 0317 007d 0174 03a0 04a1 007d  ...d...}.t.....}
+00004d60: 0274 03a0 05a1 007d 037c 0264 0417 007c  .t.....}.|.d...|
+00004d70: 0117 007d 0464 057c 019b 0064 067c 049b  ...}.d.|...d.|..
+00004d80: 0064 079d 057d 0574 067c 0583 0101 0064  .d...}.t.|.....d
+00004d90: 087c 019b 0064 097c 049b 0064 0a74 0074  .|...d.|...d.t.t
+00004da0: 01a0 0264 0ba1 0183 019b 0064 0c74 0074  ...d.......d.t.t
+00004db0: 01a0 0264 0da1 0183 019b 0064 0e74 07a0  ...d.......d.t..
+00004dc0: 08a1 009b 0064 0f9d 0b7d 0674 097c 0464  .....d...}.t.|.d
+00004dd0: 1083 028f 247d 077c 07a0 0a7c 06a1 0101  ....$}.|...|....
+00004de0: 007c 07a0 0a74 0ba1 0101 0057 0064 0004  .|...t.....W.d..
+00004df0: 0004 0083 0301 006e 1031 0073 c430 0001  .......n.1.s.0..
+00004e00: 0001 0001 0059 0001 0074 0c64 1167 0064  .....Y...t.d.g.d
+00004e10: 12a2 0164 1364 1364 148d 0401 007c 0364  ...d.d.d.....|.d
+00004e20: 156b 0272 fe64 167c 019b 0064 177c 019b  .k.r.d.|...d.|..
+00004e30: 0064 189d 057d 086e 1264 197c 019b 0064  .d...}.n.d.|...d
+00004e40: 1a7c 019b 0064 189d 057d 0874 067c 0883  .|...d...}.t.|..
+00004e50: 0101 0057 0064 1353 0001 0001 0001 0074  ...W.d.S.......t
+00004e60: 0c64 1b67 0064 1ca2 0164 1364 1d8d 0301  .d.g.d...d.d....
+00004e70: 0059 0064 1e53 0030 0064 0053 0029 1f4e  .Y.d.S.0.d.S.).N
+00004e80: 5a09 5f70 6830 6d62 6572 5f7a 1125 642d  Z._ph0mber_z.%d-
+00004e90: 256d 2d25 595f 2548 2d25 4d2d 2553 7a04  %m-%Y_%H-%M-%Sz.
+00004ea0: 2e74 7874 723b 0000 007a 2f0a 2020 2020  .txtr;...z/.    
+00004eb0: 1b5b 313b 3439 3b39 336d 5b23 5d20 4f75  .[1;49;93m[#] Ou
+00004ec0: 7470 7574 2046 696c 6520 4e61 6d65 3a20  tput File Name: 
+00004ed0: 1b5b 313b 3439 3b39 376d 7a33 1b5b 306d  .[1;49;97mz3.[0m
+00004ee0: 0a20 2020 201b 5b31 3b34 393b 3933 6d5b  .    .[1;49;93m[
+00004ef0: 235d 204f 7574 7075 7420 4669 6c65 2050  #] Output File P
+00004f00: 6174 683a 201b 5b31 3b34 393b 3937 6d7a  ath: .[1;49;97mz
+00004f10: 0d1b 5b30 6d0a 2020 2020 2020 2020 7aab  ..[0m.        z.
+00004f20: 0a20 2020 201b 5b31 3b34 393b 3933 6d5b  .    .[1;49;93m[
+00004f30: 405d 204f 7369 6e74 2066 7261 6d65 776f  @] Osint framewo
+00004f40: 726b 3a20 1b5b 313b 3439 3b39 366d 5048  rk: .[1;49;96mPH
+00004f50: 304d 4245 520a 2020 2020 1b5b 313b 3439  0MBER.    .[1;49
+00004f60: 3b39 336d 5b40 5d20 4769 7468 7562 3a20  ;93m[@] Github: 
+00004f70: 1b5b 313b 3439 3b39 366d 6874 7470 733a  .[1;49;96mhttps:
+00004f80: 2f2f 6769 7468 7562 2e63 6f6d 2f73 3431  //github.com/s41
+00004f90: 7234 6a2f 7068 6f6d 6265 720a 0a20 2020  r4j/phomber..   
+00004fa0: 201b 5b31 3b34 393b 3933 6d5b 235d 204f   .[1;49;93m[#] O
+00004fb0: 7574 7075 7420 4669 6c65 204e 616d 653a  utput File Name:
+00004fc0: 201b 5b31 3b34 393b 3937 6d7a 2f0a 2020   .[1;49;97mz/.  
+00004fd0: 2020 1b5b 313b 3439 3b39 336d 5b23 5d20    .[1;49;93m[#] 
+00004fe0: 4f75 7470 7574 2046 696c 6520 5061 7468  Output File Path
+00004ff0: 3a20 1b5b 313b 3439 3b39 376d 7a23 0a20  : .[1;49;97mz#. 
+00005000: 2020 201b 5b31 3b34 393b 3933 6d5b 235d     .[1;49;93m[#]
+00005010: 2044 6174 653a 201b 5b31 3b34 393b 3937   Date: .[1;49;97
+00005020: 6d7a 0825 642d 256d 2d25 597a 230a 2020  mz.%d-%m-%Yz#.  
+00005030: 2020 1b5b 313b 3439 3b39 336d 5b23 5d20    .[1;49;93m[#] 
+00005040: 5469 6d65 3a20 1b5b 313b 3439 3b39 376d  Time: .[1;49;97m
+00005050: 7a08 2548 3a25 4d3a 2553 7a30 0a0a 2020  z.%H:%M:%Sz0..  
+00005060: 2020 1b5b 313b 3439 3b39 336d 5b23 5d20    .[1;49;93m[#] 
+00005070: 436f 6d6d 616e 6420 4578 6563 7574 6564  Command Executed
+00005080: 3a20 1b5b 313b 3439 3b39 366d 723a 0000  : .[1;49;96mr:..
+00005090: 00da 0177 7a31 2020 2020 5b2b 5d20 4578  ...wz1    [+] Ex
+000050a0: 6375 7465 2066 6f6c 6c6f 7769 6e67 2063  cute following c
+000050b0: 6f6d 6d61 6e64 7320 746f 2076 6965 7720  ommands to view 
+000050c0: 6f75 7470 7574 3a72 2300 0000 5429 0372  output:r#...T).r
+000050d0: 2800 0000 7229 0000 0072 aa00 0000 da02  (...r)...r......
+000050e0: 6e74 7a25 2020 2020 1b5b 313b 3439 3b39  ntz%    .[1;49;9
+000050f0: 336d 3e20 1b5b 313b 3439 3b39 326d 7368  3m> .[1;49;92msh
+00005100: 656c 6c20 6d6f 7265 207a 2a1b 5b30 6d0a  ell more z*.[0m.
+00005110: 2020 2020 1b5b 313b 3439 3b39 336d 3e20      .[1;49;93m> 
+00005120: 1b5b 313b 3439 3b39 326d 7368 656c 6c20  .[1;49;92mshell 
+00005130: 7479 7065 2072 a100 0000 7a24 2020 2020  type r....z$    
+00005140: 1b5b 313b 3439 3b39 336d 3e20 1b5b 313b  .[1;49;93m> .[1;
+00005150: 3439 3b39 326d 7368 656c 6c20 6361 7420  49;92mshell cat 
+00005160: 7a2a 1b5b 306d 0a20 2020 201b 5b31 3b34  z*.[0m.    .[1;4
+00005170: 393b 3933 6d3e 201b 5b31 3b34 393b 3932  9;93m> .[1;49;92
+00005180: 6d73 6865 6c6c 206c 6573 7320 7a22 2020  mshell less z"  
+00005190: 2020 5b21 5d20 4f75 7470 7574 2063 6f75    [!] Output cou
+000051a0: 6c64 206e 6f74 2062 6520 7361 7665 6421  ld not be saved!
+000051b0: 722c 0000 0072 2700 0000 4629 0d72 4200  r,...r'...F).rB.
+000051c0: 0000 da04 7469 6d65 da08 7374 7266 7469  ....time..strfti
+000051d0: 6d65 72a2 0000 00da 0667 6574 6377 64da  mer......getcwd.
+000051e0: 0575 6e61 6d65 7248 0000 00da 0866 756c  .unamerH.....ful
+000051f0: 6c5f 636d 6472 4400 0000 da04 6f70 656e  l_cmdrD.....open
+00005200: da05 7772 6974 6572 3d00 0000 723e 0000  ..writer=...r>..
+00005210: 0029 09da 0770 7276 5f63 6d64 da08 6669  .)...prv_cmd..fi
+00005220: 6c65 6e61 6d65 da03 7077 64da 076f 735f  lename..pwd..os_
+00005230: 6e61 6d65 da04 7061 7468 5a0e 6669 6c65  name..pathZ.file
+00005240: 5f73 6176 655f 696e 666f da06 6865 6164  _save_info..head
+00005250: 6572 da01 665a 0765 7865 5f63 6d64 721b  er..fZ.exe_cmdr.
+00005260: 0000 0072 1b00 0000 721c 0000 00da 0b73  ...r....r......s
+00005270: 6176 655f 6f75 7470 7574 0403 0000 7344  ave_output....sD
+00005280: 0000 0000 0104 011a 0108 0108 010c 0202  ................
+00005290: 0102 ff04 0202 fe08 0408 0202 0402 fc04  ................
+000052a0: 0502 fb04 060c fa04 070c f904 0906 f708  ................
+000052b0: 0b0c 010a 0128 0214 0208 0114 0312 0208  .....(..........
+000052c0: 0206 0106 0112 0172 be00 0000 6300 0000  .......r....c...
+000052d0: 0000 0000 0000 0000 0005 0000 0007 0000  ................
+000052e0: 0043 0000 0073 8000 0000 7a60 6401 6402  .C...s....z`d.d.
+000052f0: 6901 7d00 7400 6a01 6403 7402 7403 a004  i.}.t.j.d.t.t...
+00005300: 6404 6405 a102 8301 1700 7c00 6406 8d02  d.d.......|.d...
+00005310: 7d01 7c01 6a05 6407 6b02 725e 7406 a007  }.|.j.d.k.r^t...
+00005320: 7c01 6a08 6408 a102 7d02 7c02 6a09 6409  |.j.d...}.|.j.d.
+00005330: 640a 640b 6901 640c 8d02 6a08 a00a a100  d.d.i.d...j.....
+00005340: 7d03 7c03 5700 5300 5700 6e0c 0100 0100  }.|.W.S.W.n.....
+00005350: 0100 5900 6e02 3000 6700 640d a201 7d04  ..Y.n.0.g.d...}.
+00005360: 7403 a00b 7c04 a101 5300 290e 4e72 5200  t...|...S.).NrR.
+00005370: 0000 7a44 4d6f 7a69 6c6c 612f 352e 3020  ..zDMozilla/5.0 
+00005380: 2858 3131 3b20 4c69 6e75 7820 7838 365f  (X11; Linux x86_
+00005390: 3634 3b20 7276 3a39 302e 3029 2047 6563  64; rv:90.0) Gec
+000053a0: 6b6f 2f32 3031 3030 3130 3120 4669 7265  ko/20100101 Fire
+000053b0: 666f 782f 3930 2e30 7a20 6874 7470 733a  fox/90.0z https:
+000053c0: 2f2f 7777 772e 6578 706c 6f69 742d 6462  //www.exploit-db
+000053d0: 2e63 6f6d 2f67 6864 622f 69e8 0300 0069  .com/ghdb/i....i
+000053e0: 401f 0000 2901 7254 0000 0072 5500 0000  @...).rT...rU...
+000053f0: 7a0b 6874 6d6c 2e70 6172 7365 725a 0268  z.html.parserZ.h
+00005400: 31da 0563 6c61 7373 7a0a 6361 7264 2d74  1..classz.card-t
+00005410: 6974 6c65 2901 da05 6174 7472 7329 167a  itle)...attrs).z
+00005420: 1d73 6974 653a 646f 6d61 696e 2e63 6f6d  .site:domain.com
+00005430: 2066 696c 6574 7970 653a 2070 6466 7a0f   filetype: pdfz.
+00005440: 696e 7572 6c3a 2070 6173 7377 6f72 6475  inurl: passwordu
+00005450: 1500 0000 696e 7465 7874 3ae2 809d 7573  ....intext:...us
+00005460: 6572 6e61 6d65 e280 9d7a 0c66 696c 6574  ername...z.filet
+00005470: 7970 653a 786c 7375 1b00 0000 6669 6c65  ype:xlsu....file
+00005480: 7479 7065 3a74 7874 20e2 809c 7573 6572  type:txt ...user
+00005490: 6e61 6d65 e280 9d75 4800 0000 6669 6c65  name...uH...file
+000054a0: 7479 7065 3a6c 6f67 20e2 809c 5048 5020  type:log ...PHP 
+000054b0: 5061 7273 6520 6572 726f 72e2 809d 207c  Parse error... |
+000054c0: 20e2 809c 5048 5020 5761 726e 696e 67e2   ...PHP Warning.
+000054d0: 809d 207c 20e2 809c 5048 5020 4572 726f  .. | ...PHP Erro
+000054e0: 72e2 809d 7517 0000 0069 6e74 6974 6c65  r...u....intitle
+000054f0: 3a20 e280 9c69 6e64 6578 206f 66e2 809d  : ...index of...
+00005500: 7522 0000 0069 6e74 6974 6c65 3a20 e280  u"...intitle: ..
+00005510: 9c69 6e64 6578 206f 66e2 809d 20e2 809c  .index of... ...
+00005520: 2e67 6974 e280 9d75 2200 0000 696e 7469  .git...u"...inti
+00005530: 746c 653a 20e2 809c 696e 6465 7820 6f66  tle: ...index of
+00005540: e280 9d20 e280 9c2e 7376 6ee2 809d 7519  ... ....svn...u.
+00005550: 0000 0069 6e75 726c 3ae2 809d 7669 6577  ...inurl:...view
+00005560: 6572 6672 616d 653f 6d6f 6465 7528 0000  erframe?modeu(..
+00005570: 0069 6e75 726c 3ae2 809d 4d75 6c74 6943  .inurl:...MultiC
+00005580: 616d 6572 6146 7261 6d65 3f4d 6f64 653d  ameraFrame?Mode=
+00005590: 4d6f 7469 6f6e e280 9d75 2b00 0000 696e  Motion...u+...in
+000055a0: 7469 746c 653a 20e2 809c 696e 6465 7820  title: ...index 
+000055b0: 6f66 e280 9d20 e280 9c2e 6261 7368 5f68  of... ....bash_h
+000055c0: 6973 746f 7279 e280 9d75 1b00 0000 696e  istory...u....in
+000055d0: 7465 7874 3a20 e280 9c4c 6173 7420 6d6f  text: ...Last mo
+000055e0: 6469 6669 6564 e280 9d75 1800 0000 696e  dified...u....in
+000055f0: 7465 7874 3a20 e280 9c49 6e64 6578 206f  text: ...Index o
+00005600: 6620 2fe2 809d 751e 0000 0069 6e74 6578  f /...u....intex
+00005610: 743a 20e2 809c 5061 7265 6e74 2044 6972  t: ...Parent Dir
+00005620: 6563 746f 7279 e280 9d75 1200 0000 696e  ectory...u....in
+00005630: 7572 6c3a 20e2 809c 6164 6d69 6ee2 809d  url: ...admin...
+00005640: 7512 0000 0069 6e75 726c 3a20 e280 9c6c  u....inurl: ...l
+00005650: 6f67 696e e280 9d75 1e00 0000 696e 7572  ogin...u....inur
+00005660: 6c3a 20e2 809c 6c6f 6769 6ee2 809d 20e2  l: ...login... .
+00005670: 809c 6164 6d69 6ee2 809d 7529 0000 0069  ..admin...u)...i
+00005680: 6e75 726c 3a20 e280 9c6c 6f67 696e e280  nurl: ...login..
+00005690: 9d20 e280 9c61 646d 696e e280 9d20 e280  . ...admin... ..
+000056a0: 9c75 7365 72e2 809d 751b 0000 0069 6e74  .user...u....int
+000056b0: 6578 743a e280 9d70 7269 7661 6379 2070  ext:...privacy p
+000056c0: 6f6c 6963 79e2 809d 7a22 2270 6173 7377  olicy...z""passw
+000056d0: 6f72 6473 2e74 7874 2220 696e 7469 746c  ords.txt" intitl
+000056e0: 653a 2249 6e64 6578 206f 6622 7517 0000  e:"Index of"u...
+000056f0: 0069 6e74 6578 743a e280 9d40 676d 6169  .intext:...@gmai
+00005700: 6c2e 636f 6de2 809d 290c 7216 0000 0072  l.com...).r....r
+00005710: 1700 0000 7242 0000 0072 1800 0000 da07  ....rB...r......
+00005720: 7261 6e64 696e 7472 8000 0000 da03 6273  randintr......bs
+00005730: 345a 0d42 6561 7574 6966 756c 536f 7570  4Z.BeautifulSoup
+00005740: 72a6 0000 00da 0466 696e 6472 4400 0000  r......findrD...
+00005750: 7219 0000 0029 0572 5400 0000 da0a 646f  r....).rT.....do
+00005760: 726b 5f71 7565 7279 5a0b 7061 7273 6564  rk_queryZ.parsed
+00005770: 5f68 746d 6c72 5e00 0000 5a10 6c6f 6361  _htmlr^...Z.loca
+00005780: 6c5f 646f 726b 5f71 7565 7279 721b 0000  l_dork_queryr...
+00005790: 0072 1b00 0000 721c 0000 0072 c400 0000  .r....r....r....
+000057a0: 2f03 0000 7316 0000 0000 0202 0108 011e  /...s...........
+000057b0: 030a 020e 0318 020a 0106 0106 0308 0772  ...............r
+000057c0: c400 0000 6300 0000 0000 0000 0000 0000  ....c...........
+000057d0: 0000 0000 0009 0000 0043 0000 0073 9a00  .........C...s..
+000057e0: 0000 7400 a001 7400 6a02 6401 6b02 7212  ..t...t.j.d.k.r.
+000057f0: 6402 6e02 6403 a101 0100 7403 6404 6405  d.n.d.....t.d.d.
+00005800: 6406 6407 7404 a005 6700 6408 a201 a101  d.d.t...g.d.....
+00005810: 6703 6409 640a 8d04 0100 7403 640b 6405  g.d.d.....t.d.d.
+00005820: 6406 6407 7404 a005 6700 6408 a201 a101  d.d.t...g.d.....
+00005830: 6703 640c 8d03 0100 7403 640d 6405 6406  g.d.....t.d.d.d.
+00005840: 6407 7404 a005 6700 6408 a201 a101 6703  d.t...g.d.....g.
+00005850: 6409 640e 8d04 0100 7403 640f 6405 6406  d.d.....t.d.d.d.
+00005860: 6407 7404 a005 6700 6408 a201 a101 6703  d.t...g.d.....g.
+00005870: 6409 640e 8d04 0100 6400 5300 2910 4e72  d.d.....d.S.).Nr
+00005880: af00 0000 da03 636c 7372 0500 0000 7577  ......clsr....uw
+00005890: 0000 00e2 9480 20e2 9692 e296 88e2 9680  ...... .........
+000058a0: e296 80e2 9688 20e2 9692 e296 88e2 9691  ...... .........
+000058b0: e296 92e2 9688 20e2 9688 e296 80e2 9680  ...... .........
+000058c0: e296 8820 e296 92e2 9688 e296 80e2 9684  ... ............
+000058d0: e296 80e2 9688 20e2 9692 e296 88e2 9680  ...... .........
+000058e0: e296 80e2 9688 20e2 9692 e296 88e2 9680  ...... .........
+000058f0: e296 80e2 9680 20e2 9692 e296 88e2 9680  ...... .........
+00005900: e296 80e2 9688 20e2 9480 7236 0000 0072  ...... ...r6...r
+00005910: 2400 0000 7225 0000 0029 0772 2d00 0000  $...r%...).r-...
+00005920: e95c 0000 0072 2600 0000 e95e 0000 00e9  .\...r&....^....
+00005930: 5f00 0000 e960 0000 00e9 6100 0000 5429  _....`....a...T)
+00005940: 0372 a700 0000 7228 0000 0072 aa00 0000  .r....r(...r....
+00005950: 7577 0000 00e2 9480 20e2 9692 e296 88e2  uw...... .......
+00005960: 9684 e296 84e2 9688 20e2 9692 e296 88e2  ........ .......
+00005970: 9680 e296 80e2 9688 20e2 9688 e296 84e2  ........ .......
+00005980: 9680 e296 8820 e296 92e2 9688 e296 92e2  ..... ..........
+00005990: 9688 e296 92e2 9688 20e2 9692 e296 88e2  ........ .......
+000059a0: 9680 e296 80e2 9684 20e2 9692 e296 88e2  ........ .......
+000059b0: 9680 e296 80e2 9680 20e2 9692 e296 88e2  ........ .......
+000059c0: 9684 e296 84e2 9680 20e2 9480 2902 72a7  ........ ...).r.
+000059d0: 0000 0072 2800 0000 7577 0000 00e2 9480  ...r(...uw......
+000059e0: 20e2 9692 e296 88e2 9691 e296 91e2 9691   ...............
+000059f0: 20e2 9692 e296 88e2 9691 e296 92e2 9688   ...............
+00005a00: 20e2 9688 e296 84e2 9684 e296 8820 e296   ............ ..
+00005a10: 92e2 9688 e296 91e2 9691 e296 92e2 9688  ................
+00005a20: 20e2 9692 e296 88e2 9684 e296 84e2 9688   ...............
+00005a30: 20e2 9692 e296 88e2 9684 e296 84e2 9684   ...............
+00005a40: 20e2 9692 e296 88e2 9691 e296 92e2 9688   ...............
+00005a50: 20e2 9480 2903 72a7 0000 0072 2800 0000   ...).r....r(...
+00005a60: 7229 0000 007a 294f 5349 4e54 2d46 5241  r)...z)OSINT-FRA
+00005a70: 4d45 574f 524b 2020 2020 2020 2020 2020  MEWORK          
+00005a80: 2020 2020 2020 2020 2040 7334 3172 346a           @s41r4j
+00005a90: 2906 72a2 0000 00da 0673 7973 7465 6dda  ).r......system.
+00005aa0: 046e 616d 6572 3e00 0000 7218 0000 0072  .namer>...r....r
+00005ab0: 1900 0000 721b 0000 0072 1b00 0000 721b  ....r....r....r.
+00005ac0: 0000 0072 1c00 0000 da04 6c6f 676f 4b03  ...r......logoK.
+00005ad0: 0000 730a 0000 0000 0218 0320 011e 0120  ..s........ ... 
+00005ae0: 0172 cd00 0000 6302 0000 0000 0000 0000  .r....c.........
+00005af0: 0000 0004 0000 0003 0000 0003 0000 0073  ...............s
+00005b00: 3200 0000 7400 7d02 8700 6601 6401 6402  2...t.}...f.d.d.
+00005b10: 8408 7c02 4400 8301 7d03 7c01 7401 7c03  ..|.D...}.|.t.|.
+00005b20: 8301 6b00 722a 7c03 7c01 1900 5300 6400  ..k.r*|.|...S.d.
+00005b30: 5300 6400 5300 2903 4e63 0100 0000 0000  S.d.S.).Nc......
+00005b40: 0000 0000 0000 0200 0000 0500 0000 1300  ................
+00005b50: 0000 731a 0000 0067 007c 005d 127d 017c  ..s....g.|.].}.|
+00005b60: 01a0 0088 00a1 0172 047c 0191 0271 0453  .......r.|...q.S
+00005b70: 0072 1b00 0000 2901 da0a 7374 6172 7473  .r....)...starts
+00005b80: 7769 7468 2902 da02 2e30 7298 0000 00a9  with)....0r.....
+00005b90: 0172 a600 0000 721b 0000 0072 1c00 0000  .r....r....r....
+00005ba0: da0a 3c6c 6973 7463 6f6d 703e 5703 0000  ..<listcomp>W...
+00005bb0: f300 0000 007a 1d63 6f6d 706c 6574 6572  .....z.completer
+00005bc0: 2e3c 6c6f 6361 6c73 3e2e 3c6c 6973 7463  .<locals>.<listc
+00005bd0: 6f6d 703e 2902 da12 6176 616c 6961 626c  omp>)...avaliabl
+00005be0: 655f 636f 6d6d 616e 6473 7247 0000 0029  e_commandsrG...)
+00005bf0: 0472 a600 0000 da05 7374 6174 65da 0863  .r......state..c
+00005c00: 6f6d 6d61 6e64 73da 076f 7074 696f 6e73  ommands..options
+00005c10: 721b 0000 0072 d000 0000 721c 0000 00da  r....r....r.....
+00005c20: 0963 6f6d 706c 6574 6572 5503 0000 730a  .completerU...s.
+00005c30: 0000 0000 0104 0112 010c 0108 0272 d700  .............r..
+00005c40: 0000 6300 0000 0000 0000 0000 0000 0026  ..c............&
+00005c50: 0000 0013 0000 0043 0000 0073 f20c 0000  .......C...s....
+00005c60: 7400 7326 7401 6401 6402 6403 7402 a003  t.s&t.d.d.d.t...
+00005c70: 6700 6404 a201 a101 6703 6405 6405 6405  g.d.....g.d.d.d.
+00005c80: 6406 8d05 0100 6700 6407 a201 7d00 7c00  d.....g.d...}.|.
+00005c90: 6408 1900 7d01 6409 7d02 640a 7404 7405  d...}.d.}.d.t.t.
+00005ca0: a006 a100 8301 1700 640b 1700 640c 7407  ........d...d.t.
+00005cb0: 640d 7408 7404 7405 a006 a100 8301 8301  d.t.t.t.........
+00005cc0: 1800 8301 1400 1700 7d03 640a 7404 7405  ........}.d.t.t.
+00005cd0: a009 a100 6a0a 8301 1700 640b 1700 640c  ....j.....d...d.
+00005ce0: 7407 640d 7408 7404 7405 a009 a100 6a0a  t.d.t.t.t.....j.
+00005cf0: 8301 8301 1800 8301 1400 1700 7d04 640a  ............}.d.
+00005d00: 7404 7405 a009 a100 6a0b 8301 1700 640b  t.t.....j.....d.
+00005d10: 1700 640c 7407 640d 7408 7404 7405 a009  ..d.t.d.t.t.t...
+00005d20: a100 6a0b 8301 8301 1800 8301 1400 1700  ..j.............
+00005d30: 7d05 640a 7404 740c a00d a100 6a0e 8301  }.d.t.t.....j...
+00005d40: 1700 640e 1700 640b 1700 640c 7407 640f  ..d...d...d.t.d.
+00005d50: 7408 7404 740c a00d a100 6a0e 8301 8301  t.t.t.....j.....
+00005d60: 1800 8301 1400 1700 7d06 640a 7404 740c  ........}.d.t.t.
+00005d70: a00f a100 8301 1700 640e 1700 640b 1700  ........d...d...
+00005d80: 640c 7407 6410 7408 7404 740c a00f a100  d.t.d.t.t.t.....
+00005d90: 8301 8301 1800 8301 1400 1700 7d07 640a  ............}.d.
+00005da0: 7404 740c a010 6411 a101 6a0e 8301 1700  t.t...d...j.....
+00005db0: 640e 1700 640b 1700 640c 7407 640f 7408  d...d...d.t.d.t.
+00005dc0: 7404 740c a010 6411 a101 6a0e 8301 8301  t.t...d...j.....
+00005dd0: 1800 8301 1400 1700 7d08 640a 7404 6412  ........}.d.t.d.
+00005de0: a011 7412 a013 6413 6414 7414 a015 a100  ..t...d.d.t.....
+00005df0: 1600 a102 a101 8301 1700 640b 1700 640c  ..........d...d.
+00005e00: 7407 640d 7408 7404 6412 a011 7412 a013  t.d.t.t.d...t...
+00005e10: 6413 6414 7414 a015 a100 1600 a102 a101  d.d.t...........
+00005e20: 8301 8301 1800 8301 1400 1700 7d09 640a  ............}.d.
+00005e30: 7404 7405 a009 a100 6a16 8301 1700 640b  t.t.....j.....d.
+00005e40: 1700 640c 7407 640d 7408 7404 7405 a009  ..d.t.d.t.t.t...
+00005e50: a100 6a16 8301 8301 1800 8301 1400 1700  ..j.............
+00005e60: 7d0a 6415 640c 7407 640d 7408 7404 6416  }.d.d.t.d.t.t.d.
+00005e70: 8301 8301 1800 8301 1400 1700 7d0b 6417  ............}.d.
+00005e80: 7c03 9b00 6418 7c04 9b00 6419 7c05 9b00  |...d.|...d.|...
+00005e90: 641a 7c0a 9b00 641b 7c09 9b00 641c 7c06  d.|...d.|...d.|.
+00005ea0: 9b00 641d 7c07 9b00 641e 7c08 9b00 641f  ..d.|...d.|...d.
+00005eb0: 7c0b 9b00 6420 9d13 7d0c 6421 7d0d 6700  |...d ..}.d!}.g.
+00005ec0: 6422 a201 7d0e 6423 7d0f 7417 a018 6424  d"..}.d#}.t...d$
+00005ed0: a101 0100 7417 a019 741a a101 0100 6425  ....t...t.....d%
+00005ee0: 6426 6702 7d10 7c10 6402 1900 7d11 7401  d&g.}.|.d...}.t.
+00005ef0: 6427 7c03 a01b a100 9b00 6428 7c01 9b00  d'|.......d(|...
+00005f00: 6429 7c11 9b00 9d06 6405 6405 642a 8d03  d)|.....d.d.d*..
+00005f10: a01b a100 7d12 7c12 642b 6b02 9002 72f2  ....}.|.d+k...r.
+00005f20: 7c00 6402 1900 7d01 6423 611c 741d 7c0d  |.d...}.d#a.t.|.
+00005f30: 8301 0100 7402 a003 7c0e a101 7d13 741d  ....t...|...}.t.
+00005f40: 642c 7c13 9b00 640b 9d03 8301 0100 9009  d,|...d.........
+00005f50: 6ef4 7c12 6400 642d 8502 1900 642b 6b02  n.|.d.d-....d+k.
+00005f60: 9005 725c 7c12 642e 1700 642d 1900 640c  ..r\|.d...d-..d.
+00005f70: 6b02 9005 723c 7c12 642f 6400 8502 1900  k...r<|.d/d.....
+00005f80: 7d12 7c12 642b 6b02 9003 7244 7c00 6402  }.|.d+k...rD|.d.
+00005f90: 1900 7d01 6430 7d14 741d 7c14 8301 0100  ..}.d0}.t.|.....
+00005fa0: 9005 7154 7c12 6431 6b02 9003 7358 7c12  ..qT|.d1k...sX|.
+00005fb0: 6432 6b02 9003 7270 7c00 6402 1900 7d01  d2k...rp|.d...}.
+00005fc0: 6433 7d15 741d 7c15 8301 0100 9005 7154  d3}.t.|.......qT
+00005fd0: 7c12 6434 6b02 9003 7292 7c00 6402 1900  |.d4k...r.|.d...
+00005fe0: 7d01 6435 7d16 741d 7c16 8301 0100 9005  }.d5}.t.|.......
+00005ff0: 7154 7c12 6436 6b02 9003 72b4 7c00 6402  qT|.d6k...r.|.d.
+00006000: 1900 7d01 6437 7d17 741d 7c17 8301 0100  ..}.d7}.t.|.....
+00006010: 9005 7154 7c12 6438 6b02 9003 72d6 7c00  ..qT|.d8k...r.|.
+00006020: 6402 1900 7d01 6439 7d18 741d 7c18 8301  d...}.d9}.t.|...
+00006030: 0100 9005 7154 7c12 643a 6b02 9003 72f8  ....qT|.d:k...r.
+00006040: 7c00 6402 1900 7d01 643b 7d19 741d 7c19  |.d...}.d;}.t.|.
+00006050: 8301 0100 9005 7154 7c12 643c 6b02 9004  ......qT|.d<k...
+00006060: 721a 7c00 6402 1900 7d01 643d 7d1a 741d  r.|.d...}.d=}.t.
+00006070: 7c1a 8301 0100 9005 7154 7c12 6400 642f  |.......qT|.d.d/
+00006080: 8502 1900 643e 6b02 9004 7242 7c00 6402  ....d>k...rB|.d.
+00006090: 1900 7d01 643f 7d1b 741d 7c1b 8301 0100  ..}.d?}.t.|.....
+000060a0: 6ef8 7c12 6440 6b02 9004 7262 7c00 6402  n.|.d@k...rb|.d.
+000060b0: 1900 7d01 6441 7d1c 741d 7c1c 8301 0100  ..}.dA}.t.|.....
+000060c0: 6ed8 7c12 6442 6b02 9004 7282 7c00 6402  n.|.dBk...r.|.d.
+000060d0: 1900 7d01 6443 7d1d 741d 7c1d 8301 0100  ..}.dC}.t.|.....
+000060e0: 6eb8 7c12 6444 6b02 9004 72a2 7c00 6402  n.|.dDk...r.|.d.
+000060f0: 1900 7d01 6445 7d1e 741d 7c1e 8301 0100  ..}.dE}.t.|.....
+00006100: 6e98 7c12 6446 6b02 9004 72c2 7c00 6402  n.|.dFk...r.|.d.
+00006110: 1900 7d01 6447 7d1f 741d 7c1f 8301 0100  ..}.dG}.t.|.....
+00006120: 6e78 7c12 6448 6b02 9004 72e2 7c00 6402  nx|.dHk...r.|.d.
+00006130: 1900 7d01 6449 7d20 741d 7c20 8301 0100  ..}.dI} t.| ....
+00006140: 6e58 7c12 644a 6b02 9005 7202 7c00 6402  nX|.dJk...r.|.d.
+00006150: 1900 7d01 644b 7d21 741d 7c21 8301 0100  ..}.dK}!t.|!....
+00006160: 6e38 7c12 644c 6b02 9005 7222 7c00 6402  n8|.dLk...r"|.d.
+00006170: 1900 7d01 644d 7d22 741d 7c22 8301 0100  ..}.dM}"t.|"....
+00006180: 6e18 7c00 644e 1900 7d01 7401 644f 6700  n.|.dN..}.t.dOg.
+00006190: 6450 a201 6451 8d02 0100 6e18 7c00 644e  dP..dQ....n.|.dN
+000061a0: 1900 7d01 7401 6452 6700 6450 a201 6451  ..}.t.dRg.dP..dQ
+000061b0: 8d02 0100 6423 611c 9007 6e8a 7c12 6431  ....d#a...n.|.d1
+000061c0: 6b02 9005 7370 7c12 6432 6b02 9005 729a  k...sp|.d2k...r.
+000061d0: 7400 9005 7392 7401 6453 6402 6403 7402  t...s.t.dSd.d.t.
+000061e0: a003 6700 6404 a201 a101 6703 6451 8d02  ..g.d.....g.dQ..
+000061f0: 0100 741e 8201 9007 6e4c 7c12 6434 6b02  ..t.....nL|.d4k.
+00006200: 9005 72dc 7c00 6402 1900 7d01 6423 611c  ..r.|.d...}.d#a.
+00006210: 7401 6454 6700 6455 a201 6405 6456 8d03  t.dTg.dU..d.dV..
+00006220: 0100 7401 6457 741f 8300 1700 6700 6458  ..t.dWt.....g.dX
+00006230: a201 6451 8d02 0100 9007 6e0a 7c12 6436  ..dQ......n.|.d6
+00006240: 6b02 9005 72fe 7c00 6402 1900 7d01 6423  k...r.|.d...}.d#
+00006250: 611c 741d 7c02 8301 0100 9006 6ee8 7c12  a.t.|.......n.|.
+00006260: 6438 6b02 9006 72fe 7401 6459 6700 6455  d8k...r.t.dYg.dU
+00006270: a201 6405 6456 8d03 0100 7aa6 7420 a021  ..d.dV....z.t .!
+00006280: 645a a101 0100 7401 645b 6700 6458 a201  dZ....t.d[g.dX..
+00006290: 6451 8d02 0100 7a16 7420 a021 645c a101  dQ....z.t .!d\..
+000062a0: a022 a100 645d 1900 7d23 5700 6e4c 0100  ."..d]..}#W.nL..
+000062b0: 0100 0100 7a10 7420 a021 645e a101 6a23  ....z.t .!d^..j#
+000062c0: 7d23 5700 6e2e 0100 0100 0100 7a10 7420  }#W.n.......z.t 
+000062d0: a021 645f a101 6a23 7d23 5700 6e10 0100  .!d_..j#}#W.n...
+000062e0: 0100 0100 6460 7d23 5900 6e02 3000 5900  ....d`}#Y.n.0.Y.
+000062f0: 6e02 3000 5900 6e02 3000 7c23 9006 72b6  n.0.Y.n.0.|#..r.
+00006300: 7401 6461 7c23 9b00 9d02 6700 6458 a201  t.da|#....g.dX..
+00006310: 6451 8d02 0100 7c00 6408 1900 7d01 5700  dQ....|.d...}.W.
+00006320: 6e34 0100 0100 0100 7401 6462 6700 6450  n4......t.dbg.dP
+00006330: a201 6451 8d02 0100 7401 6463 6700 6458  ..dQ....t.dcg.dX
+00006340: a201 6451 8d02 0100 7c00 644e 1900 7d01  ..dQ....|.dN..}.
+00006350: 5900 6e02 3000 6423 611c 9005 6ee8 7c12  Y.n.0.d#a...n.|.
+00006360: 643a 6b02 9007 7232 7c00 6408 1900 7d01  d:k...r2|.d...}.
+00006370: 6423 611c 7405 a024 7405 6a25 6464 6b02  d#a.t..$t.j%ddk.
+00006380: 9007 7228 6465 6e02 643a a101 0100 9005  ..r(den.d:......
+00006390: 6eb4 7c12 643c 6b02 9007 7296 7401 6466  n.|.d<k...r.t.df
+000063a0: 6700 6455 a201 6405 6456 8d03 0100 741c  g.dU..d.dV....t.
+000063b0: 6423 6b02 9007 7272 7401 6467 6700 6450  d#k...rrt.dgg.dP
+000063c0: a201 6451 8d02 0100 7c00 6468 1900 7d01  ..dQ....|.dh..}.
+000063d0: 6e1c 7426 7c0f 8301 9007 7286 7c00 6408  n.t&|.....r.|.d.
+000063e0: 1900 7d01 6e08 7c00 644e 1900 7d01 6423  ..}.n.|.dN..}.d#
+000063f0: 611c 9005 6e50 7c12 643e 6b02 9007 72c0  a...nP|.d>k...r.
+00006400: 7c00 6468 1900 7d01 6423 611c 7401 6469  |.dh..}.d#a.t.di
+00006410: 6700 6450 a201 6451 8d02 0100 9005 6e26  g.dP..dQ......n&
+00006420: 7c12 6400 642f 8502 1900 643e 6b02 9008  |.d.d/....d>k...
+00006430: 7274 7c12 642e 1700 642f 1900 640c 6b02  rt|.d...d/..d.k.
+00006440: 9008 7254 7c12 646a 6400 8502 1900 7d12  ..rT|.djd.....}.
+00006450: 646b 7404 7c12 8301 9b00 646c 9d03 7d24  dkt.|.....dl..}$
+00006460: 741d 7c24 8301 0100 7405 a024 7c12 a101  t.|$....t..$|...
+00006470: 7d25 7c25 6408 6b02 9008 7238 7401 646d  }%|%d.k...r8t.dm
+00006480: 6700 646e a201 646f 6470 8d03 0100 7c00  g.dn..dodp....|.
+00006490: 6408 1900 7d01 6e1a 7401 6471 6700 6472  d...}.n.t.dqg.dr
+000064a0: a201 646f 6470 8d03 0100 7c00 644e 1900  ..dodp....|.dN..
+000064b0: 7d01 6e18 7c00 644e 1900 7d01 7401 6452  }.n.|.dN..}.t.dR
+000064c0: 6700 6450 a201 6451 8d02 0100 6423 611c  g.dP..dQ....d#a.
+000064d0: 9004 6e72 7c12 6440 6b02 9008 7296 7c00  ..nr|.d@k...r.|.
+000064e0: 6402 1900 7d01 6423 611c 741d 7c0c 8301  d...}.d#a.t.|...
+000064f0: 0100 9004 6e50 7c12 6442 6b02 9008 72c0  ....nP|.dBk...r.
+00006500: 7c00 6468 1900 7d01 6423 611c 7401 6473  |.dh..}.d#a.t.ds
+00006510: 6700 6450 a201 6451 8d02 0100 9004 6e26  g.dP..dQ......n&
+00006520: 7c12 6400 646a 8502 1900 6442 6b02 9009  |.d.dj....dBk...
+00006530: 7282 7c12 642e 1700 646a 1900 640c 6b02  r.|.d...dj..d.k.
+00006540: 9009 7262 7c12 6474 6400 8502 1900 7d12  ..rb|.dtd.....}.
+00006550: 7c12 6475 6b02 9009 721c 7c10 6408 1900  |.duk...r.|.d...
+00006560: 7d11 7c00 6408 1900 7d01 7401 6476 6700  }.|.d...}.t.dvg.
+00006570: 6458 a201 6451 8d02 0100 6e44 7c12 6477  dX..dQ....nD|.dw
+00006580: 6b02 9009 7248 7c10 6402 1900 7d11 7c00  k...rH|.d...}.|.
+00006590: 6408 1900 7d01 7401 6478 6700 6458 a201  d...}.t.dxg.dX..
+000065a0: 6451 8d02 0100 6e18 7c00 644e 1900 7d01  dQ....n.|.dN..}.
+000065b0: 7401 6479 6700 6450 a201 6451 8d02 0100  t.dyg.dP..dQ....
+000065c0: 6e18 7c00 644e 1900 7d01 7401 6452 6700  n.|.dN..}.t.dRg.
+000065d0: 6450 a201 6451 8d02 0100 6423 611c 9003  dP..dQ....d#a...
+000065e0: 6e64 7c12 6444 6b02 9009 72a8 7c00 6468  nd|.dDk...r.|.dh
+000065f0: 1900 7d01 7401 647a 6700 6450 a201 6451  ..}.t.dzg.dP..dQ
+00006600: 8d02 0100 9003 6e3e 7c12 6400 646a 8502  ......n>|.d.dj..
+00006610: 1900 6444 6b02 900a 722c 7c12 6127 7c12  ..dDk...r,|.a'|.
+00006620: 642e 1700 646a 1900 640c 6b02 900a 7210  d...dj..d.k...r.
+00006630: 7c12 6474 6400 8502 1900 7d12 7401 647b  |.dtd.....}.t.d{
+00006640: 6700 6455 a201 6405 6456 8d03 0100 7428  g.dU..d.dV....t(
+00006650: 7c12 8301 900a 7202 7c00 642d 1900 7d01  |.....r.|.d-..}.
+00006660: 6e0c 7c00 644e 1900 7d01 6423 611c 6e18  n.|.dN..}.d#a.n.
+00006670: 7c00 644e 1900 7d01 7401 6452 6700 6450  |.dN..}.t.dRg.dP
+00006680: a201 6451 8d02 0100 9002 6eba 7c12 644a  ..dQ......n.|.dJ
+00006690: 6b02 900a 7252 7c00 6468 1900 7d01 7401  k...rR|.dh..}.t.
+000066a0: 647c 6700 6450 a201 6451 8d02 0100 9002  d|g.dP..dQ......
+000066b0: 6e94 7c12 6400 6468 8502 1900 644a 6b02  n.|.d.dh....dJk.
+000066c0: 900a 72d6 7c12 6127 7c12 642e 1700 6468  ..r.|.a'|.d...dh
+000066d0: 1900 640c 6b02 900a 72ba 7c12 644e 6400  ..d.k...r.|.dNd.
+000066e0: 8502 1900 7d12 7401 647d 6700 6455 a201  ....}.t.d}g.dU..
+000066f0: 6405 6456 8d03 0100 7429 7c12 8301 900a  d.dV....t)|.....
+00006700: 72ac 7c00 642d 1900 7d01 6e0c 7c00 644e  r.|.d-..}.n.|.dN
+00006710: 1900 7d01 6423 611c 6e18 7c00 644e 1900  ..}.d#a.n.|.dN..
+00006720: 7d01 7401 6452 6700 6450 a201 6451 8d02  }.t.dRg.dP..dQ..
+00006730: 0100 9002 6e10 7c12 644c 6b02 900a 72fc  ....n.|.dLk...r.
+00006740: 7c00 6468 1900 7d01 7401 647e 6700 6450  |.dh..}.t.d~g.dP
+00006750: a201 6451 8d02 0100 9001 6eea 7c12 6400  ..dQ......n.|.d.
+00006760: 644e 8502 1900 644c 6b02 900b 7280 7c12  dN....dLk...r.|.
+00006770: 6127 7c12 642e 1700 644e 1900 640c 6b02  a'|.d...dN..d.k.
+00006780: 900b 7264 7c12 642d 6400 8502 1900 7d12  ..rd|.d-d.....}.
+00006790: 7401 647f 6700 6455 a201 6405 6456 8d03  t.d.g.dU..d.dV..
+000067a0: 0100 742a 7c12 8301 900b 7256 7c00 642d  ..t*|.....rV|.d-
+000067b0: 1900 7d01 6e0c 7c00 644e 1900 7d01 6423  ..}.n.|.dN..}.d#
+000067c0: 611c 6e18 7c00 644e 1900 7d01 7401 6452  a.n.|.dN..}.t.dR
+000067d0: 6700 6450 a201 6451 8d02 0100 9001 6e66  g.dP..dQ......nf
+000067e0: 7c12 6446 6b02 900b 72a6 7c00 6468 1900  |.dFk...r.|.dh..
+000067f0: 7d01 7401 6480 6700 6450 a201 6451 8d02  }.t.d.g.dP..dQ..
+00006800: 0100 9001 6e40 7c12 6400 642f 8502 1900  ....n@|.d.d/....
+00006810: 6446 6b02 900c 7228 7c12 6127 7c12 642e  dFk...r(|.a'|.d.
+00006820: 1700 642f 1900 640c 6b02 900c 720e 7c12  ..d/..d.k...r.|.
+00006830: 646a 6400 8502 1900 7d12 7401 6481 6700  djd.....}.t.d.g.
+00006840: 6455 a201 6405 6456 8d03 0100 742b 7c12  dU..d.dV....t+|.
+00006850: 8301 900c 7200 7c00 642d 1900 7d01 6e0c  ....r.|.d-..}.n.
+00006860: 7c00 644e 1900 7d01 6423 611c 6e18 7c00  |.dN..}.d#a.n.|.
+00006870: 644e 1900 7d01 7401 6452 6700 6450 a201  dN..}.t.dRg.dP..
+00006880: 6451 8d02 0100 6ebe 7c12 6448 6b02 900c  dQ....n.|.dHk...
+00006890: 724c 7c00 6468 1900 7d01 7401 6482 6700  rL|.dh..}.t.d.g.
+000068a0: 6450 a201 6451 8d02 0100 6e9a 7c12 6400  dP..dQ....n.|.d.
+000068b0: 644e 8502 1900 6448 6b02 900c 72ce 7c12  dN....dHk...r.|.
+000068c0: 6127 7c12 642e 1700 644e 1900 640c 6b02  a'|.d...dN..d.k.
+000068d0: 900c 72b4 7c12 642d 6400 8502 1900 7d12  ..r.|.d-d.....}.
+000068e0: 7401 6483 6700 6455 a201 6405 6456 8d03  t.d.g.dU..d.dV..
+000068f0: 0100 742c 7c12 8301 900c 72a6 7c00 642d  ..t,|.....r.|.d-
+00006900: 1900 7d01 6e0c 7c00 644e 1900 7d01 6423  ..}.n.|.dN..}.d#
+00006910: 611c 6e18 7c00 644e 1900 7d01 7401 6452  a.n.|.dN..}.t.dR
+00006920: 6700 6450 a201 6451 8d02 0100 6e18 7c00  g.dP..dQ....n.|.
+00006930: 644e 1900 7d01 7401 6452 6700 6450 a201  dN..}.t.dRg.dP..
+00006940: 6451 8d02 0100 7c12 7d0f 9002 718e 6400  dQ....|.}...q.d.
+00006950: 5300 2984 4e7a 275b 235d 2049 6e69 7469  S.).Nz'[#] Initi
+00006960: 616c 697a 696e 6720 6050 4830 4d42 4552  alizing `PH0MBER
+00006970: 6020 6672 616d 6577 6f72 6b2e 2e2e 7224  ` framework...r$
+00006980: 0000 0072 2500 0000 2903 72c6 0000 0072  ...r%...).r....r
+00006990: c900 0000 72ca 0000 0054 2904 7228 0000  ....r....T).r(..
+000069a0: 0072 a900 0000 72a8 0000 0072 aa00 0000  .r....r....r....
+000069b0: 2905 7a10 1b5b 313b 3439 3b39 326d 3a44  ).z..[1;49;92m:D
+000069c0: 1b5b 306d 7a10 1b5b 313b 3439 3b39 366d  .[0mz..[1;49;96m
+000069d0: 3a29 1b5b 306d 7a10 1b5b 313b 3439 3b39  :).[0mz..[1;49;9
+000069e0: 336d 3a7c 1b5b 306d 7a10 1b5b 313b 3439  3m:|.[0mz..[1;49
+000069f0: 3b39 316d 3a28 1b5b 306d 7a10 1b5b 313b  ;91m:(.[0mz..[1;
+00006a00: 3439 3b39 376d 3a6f 1b5b 306d 7201 0000  49;97m:o.[0mr...
+00006a10: 0075 f303 0000 2020 2020 1b5b 313b 3439  .u....    .[1;49
+00006a20: 3b39 336d 3e20 4578 7072 6573 7369 6f6e  ;93m> Expression
+00006a30: 7320 6172 6520 7573 6564 2074 6f20 7368  s are used to sh
+00006a40: 6f77 2074 6865 2073 7461 7475 7320 6f66  ow the status of
+00006a50: 2074 6865 2070 7265 7669 6f75 7320 636f   the previous co
+00006a60: 6d6d 616e 641b 5b30 6d0a 0a20 2020 201b  mmand.[0m..    .
+00006a70: 5b31 3b34 393b 3933 6d3e 2053 796e 7461  [1;49;93m> Synta
+00006a80: 783a 1b5b 306d 201b 5b31 3b34 393b 3937  x:.[0m .[1;49;97
+00006a90: 6d5b 3c75 7365 723e 4070 6830 6d62 6572  m[<user>@ph0mber
+00006aa0: 5de2 b8ba 201b 5b31 3b34 393b 3936 6d5b  ]... .[1;49;96m[
+00006ab0: 3c65 7870 7265 7373 696f 6e3e 5d1b 5b31  <expression>].[1
+00006ac0: 3b34 393b 3937 6d20 2420 3c63 6f6d 6d61  ;49;97m $ <comma
+00006ad0: 6e64 3e1b 5b30 6d0a 0a20 2020 20e2 948c  nd>.[0m..    ...
+00006ae0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00006af0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00006b00: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00006b10: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00006b20: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00006b30: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00006b40: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00006b50: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00006b60: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00006b70: e294 80e2 9480 e294 80e2 9480 e294 900a  ................
+00006b80: 2020 2020 7c20 4558 5052 4553 5349 4f4e      | EXPRESSION
+00006b90: 5320 2020 7c20 4445 5343 5249 5054 494f  S   | DESCRIPTIO
+00006ba0: 4e20 2020 2020 2020 2020 2020 2020 2020  N               
+00006bb0: 2020 2020 2020 2020 207c 0a20 2020 207c           |.    |
+00006bc0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00006bd0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00006be0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00006bf0: 2d2d 2d2d 7c0a 2020 2020 7c20 1b5b 313b  ----|.    | .[1;
+00006c00: 3439 3b39 326d 3a44 1b5b 306d 2020 2020  49;92m:D.[0m    
+00006c10: 2020 2020 2020 2020 7c20 4576 6572 7974          | Everyt
+00006c20: 6869 6e67 2069 7320 6669 6e65 2020 2020  hing is fine    
+00006c30: 2020 2020 2020 2020 2020 2020 207c 0a20               |. 
+00006c40: 2020 207c 201b 5b31 3b34 393b 3936 6d3a     | .[1;49;96m:
+00006c50: 291b 5b30 6d20 2020 2020 2020 2020 2020  ).[0m           
+00006c60: 207c 2049 6e66 6f72 6d61 7469 6f6e 2061   | Information a
+00006c70: 7661 696c 6162 6c65 2020 2020 2020 2020  vailable        
+00006c80: 2020 2020 2020 7c0a 2020 2020 7c20 1b5b        |.    | .[
+00006c90: 313b 3439 3b39 336d 3a7c 1b5b 306d 2020  1;49;93m:|.[0m  
+00006ca0: 2020 2020 2020 2020 2020 7c20 4974 2773            | It's
+00006cb0: 2061 2077 6172 6e69 6e67 2028 7265 6d65   a warning (reme
+00006cc0: 6d62 6572 2920 2020 2020 2020 2020 207c  mber)          |
+00006cd0: 0a20 2020 207c 201b 5b31 3b34 393b 3931  .    | .[1;49;91
+00006ce0: 6d3a 281b 5b30 6d20 2020 2020 2020 2020  m:(.[0m         
+00006cf0: 2020 207c 2053 6f6d 6574 6869 6e67 2077     | Something w
+00006d00: 656e 7420 7772 6f6e 6720 2020 2020 2020  ent wrong       
+00006d10: 2020 2020 2020 2020 7c0a 2020 2020 7c20          |.    | 
+00006d20: 1b5b 313b 3439 3b39 376d 3a6f 1b5b 306d  .[1;49;97m:o.[0m
+00006d30: 2020 2020 2020 2020 2020 2020 7c20 5363              | Sc
+00006d40: 616e 2072 6573 756c 7473 2061 7661 696c  an results avail
+00006d50: 6162 6c65 2020 2020 2020 2020 2020 2020  able            
+00006d60: 207c 0a20 2020 20e2 9494 e294 80e2 9480   |.    .........
+00006d70: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00006d80: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00006d90: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00006da0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00006db0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00006dc0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00006dd0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00006de0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00006df0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00006e00: e294 80e2 9480 e294 987a 0a1b 5b31 3b34  .........z..[1;4
+00006e10: 393b 3936 6d72 a100 0000 7236 0000 00e9  9;96mr....r6....
+00006e20: 2200 0000 fa01 25e9 2100 0000 e920 0000  ".....%.!.... ..
+00006e30: 0072 3b00 0000 fa01 3a7a 022e 2e7a 0525  .r;.....:z...z.%
+00006e40: 3031 3278 7a1a 1b5b 313b 3439 3b39 366d  012xz..[1;49;96m
+00006e50: 332e 302e 3220 2862 6574 6129 1b5b 306d  3.0.2 (beta).[0m
+00006e60: 7a0c 332e 302e 3220 2862 6574 6129 7542  z.3.0.2 (beta)uB
+00006e70: 0100 000a 2020 2020 e294 8ce2 9480 e294  ....    ........
+00006e80: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00006e90: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00006ea0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00006eb0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00006ec0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00006ed0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00006ee0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00006ef0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00006f00: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00006f10: 80e2 9480 e294 80e2 9490 0a20 2020 207c  ...........    |
+00006f20: 2053 5953 5445 4d20 494e 464f 2020 207c   SYSTEM INFO   |
+00006f30: 2044 4553 4352 4950 5449 4f4e 2020 2020   DESCRIPTION    
+00006f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006f50: 2020 2020 7c0a 2020 2020 7c2d 2d2d 2d2d      |.    |-----
+00006f60: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00006f70: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00006f80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d7c  ---------------|
+00006f90: 0a20 2020 207c 201b 5b31 3b34 393b 3937  .    | .[1;49;97
+00006fa0: 6d55 7365 721b 5b30 6d20 2020 2020 2020  mUser.[0m       
+00006fb0: 2020 207c 207a 2720 7c0a 2020 2020 7c20     | z' |.    | 
+00006fc0: 1b5b 313b 3439 3b39 376d 486f 7374 6e61  .[1;49;97mHostna
+00006fd0: 6d65 1b5b 306d 2020 2020 2020 7c20 7a27  me.[0m      | z'
+00006fe0: 207c 0a20 2020 207c 201b 5b31 3b34 393b   |.    | .[1;49;
+00006ff0: 3937 6d4f 531b 5b30 6d20 2020 2020 2020  97mOS.[0m       
+00007000: 2020 2020 207c 207a 2720 7c0a 2020 2020       | z' |.    
+00007010: 7c20 1b5b 313b 3439 3b39 376d 4172 6368  | .[1;49;97mArch
+00007020: 6974 6563 7475 7265 1b5b 306d 2020 7c20  itecture.[0m  | 
+00007030: 7a27 207c 0a20 2020 207c 201b 5b31 3b34  z' |.    | .[1;4
+00007040: 393b 3937 6d53 7973 7465 6d20 4d41 431b  9;97mSystem MAC.
+00007050: 5b30 6d20 2020 207c 207a 6220 7c0a 2020  [0m    | zb |.  
+00007060: 2020 7c2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d    |-------------
+00007070: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00007080: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00007090: 2d2d 2d2d 2d2d 2d7c 0a20 2020 207c 201b  -------|.    | .
+000070a0: 5b31 3b34 393b 3937 6d52 414d 2055 7361  [1;49;97mRAM Usa
+000070b0: 6765 1b5b 306d 2020 2020 207c 207a 2720  ge.[0m     | z' 
+000070c0: 7c0a 2020 2020 7c20 1b5b 313b 3439 3b39  |.    | .[1;49;9
+000070d0: 376d 4350 5520 5573 6167 651b 5b30 6d20  7mCPU Usage.[0m 
+000070e0: 2020 2020 7c20 7a27 207c 0a20 2020 207c      | z' |.    |
+000070f0: 201b 5b31 3b34 393b 3937 6d44 6973 6b20   .[1;49;97mDisk 
+00007100: 5573 6167 651b 5b30 6d20 2020 207c 2075  Usage.[0m    | u
+00007110: 4302 0000 207c 0a20 2020 20e2 9494 e294  C... |.    .....
+00007120: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00007130: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00007140: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00007150: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00007160: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00007170: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00007180: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00007190: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+000071a0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+000071b0: 80e2 9480 e294 80e2 9480 e294 980a 0a20  ............... 
+000071c0: 2020 20e2 948c e294 80e2 9480 e294 80e2     .............
+000071d0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+000071e0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+000071f0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00007200: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00007210: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00007220: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00007230: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00007240: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00007250: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00007260: 9480 e294 900a 2020 2020 7c20 4652 414d  ......    | FRAM
+00007270: 4557 4f52 4b20 494e 464f 7c20 4445 5343  EWORK INFO| DESC
+00007280: 5249 5054 494f 4e20 2020 2020 2020 2020  RIPTION         
+00007290: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+000072a0: 0a20 2020 207c 2d2d 2d2d 2d2d 2d2d 2d2d  .    |----------
+000072b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000072c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000072d0: 2d2d 2d2d 2d2d 2d2d 2d2d 7c0a 2020 2020  ----------|.    
+000072e0: 7c20 1b5b 313b 3439 3b39 376d 4e61 6d65  | .[1;49;97mName
+000072f0: 1b5b 306d 2020 2020 2020 2020 2020 7c20  .[0m          | 
+00007300: 1b5b 313b 3439 3b39 366d 5048 304d 4245  .[1;49;96mPH0MBE
+00007310: 521b 5b30 6d20 2020 2020 2020 2020 2020  R.[0m           
+00007320: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007330: 207c 0a20 2020 207c 201b 5b31 3b34 393b   |.    | .[1;49;
+00007340: 3937 6d56 6572 7369 6f6e 1b5b 306d 2020  97mVersion.[0m  
+00007350: 2020 2020 207c 2075 b301 0000 207c 0a20       | u.... |. 
+00007360: 2020 207c 201b 5b31 3b34 393b 3937 6d54     | .[1;49;97mT
+00007370: 7970 651b 5b30 6d20 2020 2020 2020 2020  ype.[0m         
+00007380: 207c 201b 5b31 3b34 393b 3936 6d4f 5349   | .[1;49;96mOSI
+00007390: 4e54 2046 7261 6d65 776f 726b 1b5b 306d  NT Framework.[0m
+000073a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000073b0: 2020 2020 7c0a 2020 2020 7c20 1b5b 313b      |.    | .[1;
+000073c0: 3439 3b39 376d 4465 7665 6c6f 7065 721b  49;97mDeveloper.
+000073d0: 5b30 6d20 2020 2020 7c20 1b5b 313b 3439  [0m     | .[1;49
+000073e0: 3b39 366d 7334 3172 346a 1b5b 306d 2020  ;96ms41r4j.[0m  
+000073f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007400: 2020 2020 2020 2020 2020 207c 0a20 2020             |.   
+00007410: 207c 201b 5b31 3b34 393b 3937 6d47 6974   | .[1;49;97mGit
+00007420: 6875 621b 5b30 6d20 2020 2020 2020 207c  hub.[0m        |
+00007430: 201b 5b31 3b34 393b 3936 6d68 7474 7073   .[1;49;96mhttps
+00007440: 3a2f 2f67 6974 6875 622e 636f 6d2f 7334  ://github.com/s4
+00007450: 3172 346a 2f70 686f 6d62 6572 1b5b 306d  1r4j/phomber.[0m
+00007460: 2020 7c0a 2020 2020 e294 94e2 9480 e294    |.    ........
+00007470: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00007480: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00007490: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+000074a0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+000074b0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+000074c0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+000074d0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+000074e0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+000074f0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00007500: 80e2 9480 e294 80e2 9498 0a20 2020 2075  ...........    u
+00007510: 3b08 0000 0a20 2020 20e2 948c e294 80e2  ;....    .......
+00007520: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00007530: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00007540: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00007550: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00007560: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00007570: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00007580: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00007590: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+000075a0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+000075b0: 9480 e294 80e2 9480 e294 900a 2020 2020  ............    
+000075c0: 7c20 434f 4d4d 414e 4453 2020 2020 2020  | COMMANDS      
+000075d0: 7c20 4445 5343 5249 5054 494f 4e20 2020  | DESCRIPTION   
+000075e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000075f0: 2020 2020 207c 0a20 2020 207c 2d2d 2d2d       |.    |----
+00007600: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00007610: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00007620: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00007630: 7c0a 2020 2020 7c20 2020 2020 2020 2020  |.    |         
+00007640: 2020 2020 2020 203c 4261 7369 6320 436f         <Basic Co
+00007650: 6d6d 616e 6473 3e20 2020 2020 2020 2020  mmands>         
+00007660: 2020 2020 2020 2020 2020 207c 0a20 2020             |.   
+00007670: 207c 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   |--------------
+00007680: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00007690: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000076a0: 2d2d 2d2d 2d2d 7c0a 2020 2020 7c20 1b5b  ------|.    | .[
+000076b0: 313b 3439 3b39 376d 6865 6c70 1b5b 306d  1;49;97mhelp.[0m
+000076c0: 2020 2020 2020 2020 2020 7c20 4469 7370            | Disp
+000076d0: 6c61 7920 7468 6973 2068 656c 7020 6d65  lay this help me
+000076e0: 6e75 2020 2020 2020 2020 2020 2020 207c  nu             |
+000076f0: 200a 2020 2020 7c20 1b5b 313b 3439 3b39   .    | .[1;49;9
+00007700: 376d 6578 6974 2f71 7569 741b 5b30 6d20  7mexit/quit.[0m 
+00007710: 2020 2020 7c20 4578 6974 2074 6865 2066      | Exit the f
+00007720: 7261 6d65 776f 726b 2020 2020 2020 2020  ramework        
+00007730: 2020 2020 2020 2020 207c 0a20 2020 207c           |.    |
+00007740: 201b 5b31 3b34 393b 3937 6d64 6f72 6b1b   .[1;49;97mdork.
+00007750: 5b30 6d20 2020 2020 2020 2020 207c 2053  [0m          | S
+00007760: 686f 7720 6120 7261 6e64 6f6d 2067 6f6f  how a random goo
+00007770: 676c 6520 646f 726b 2071 7565 7279 202a  gle dork query *
+00007780: 2020 7c20 200a 2020 2020 7c20 1b5b 313b    |  .    | .[1;
+00007790: 3439 3b39 376d 6578 701b 5b30 6d20 2020  49;97mexp.[0m   
+000077a0: 2020 2020 2020 2020 7c20 5368 6f77 2069          | Show i
+000077b0: 6e66 6f20 6162 6f75 7420 616c 6c20 6176  nfo about all av
+000077c0: 6169 6c61 626c 6520 2020 2020 207c 2020  ailable      |  
+000077d0: 2020 2020 200a 2020 2020 7c20 2020 2020       .    |     
+000077e0: 2020 2020 2020 2020 2020 7c20 6578 7072            | expr
+000077f0: 6573 7369 6f6e 7320 2020 2020 2020 2020  essions         
+00007800: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+00007810: 0a20 2020 207c 201b 5b31 3b34 393b 3937  .    | .[1;49;97
+00007820: 6d63 6865 636b 1b5b 306d 2020 2020 2020  mcheck.[0m      
+00007830: 2020 207c 2043 6865 636b 2069 6e74 6572     | Check inter
+00007840: 6e65 7420 636f 6e6e 6563 7469 6f6e 2020  net connection  
+00007850: 2020 2020 2020 2020 7c0a 2020 2020 7c20          |.    | 
+00007860: 1b5b 313b 3439 3b39 376d 636c 6561 721b  .[1;49;97mclear.
+00007870: 5b30 6d20 2020 2020 2020 2020 7c20 436c  [0m         | Cl
+00007880: 6561 7220 7363 7265 656e 2020 2020 2020  ear screen      
+00007890: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000078a0: 207c 0a20 2020 207c 201b 5b31 3b34 393b   |.    | .[1;49;
+000078b0: 3937 6d73 6176 651b 5b30 6d20 2020 2020  97msave.[0m     
+000078c0: 2020 2020 207c 2053 6176 6520 6f75 7470       | Save outp
+000078d0: 7574 206f 6620 7072 6576 696f 7573 2073  ut of previous s
+000078e0: 6361 6e6e 6572 2020 2020 7c0a 2020 2020  canner    |.    
+000078f0: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
+00007900: 7c20 636f 6d6d 616e 6420 696e 2061 2066  | command in a f
+00007910: 696c 6520 2020 2020 2020 2020 2020 2020  ile             
+00007920: 2020 2020 207c 0a20 2020 207c 201b 5b31       |.    | .[1
+00007930: 3b34 393b 3937 6d73 6865 6c6c 203c 636d  ;49;97mshell <cm
+00007940: 643e 1b5b 306d 2020 207c 2045 7865 6375  d>.[0m   | Execu
+00007950: 7465 206e 6174 6976 6520 7368 656c 6c2f  te native shell/
+00007960: 636d 6420 636f 6d6d 616e 6473 2020 7c0a  cmd commands  |.
+00007970: 2020 2020 7c20 1b5b 313b 3439 3b39 376d      | .[1;49;97m
+00007980: 696e 666f 1b5b 306d 2020 2020 2020 2020  info.[0m        
+00007990: 2020 7c20 5368 6f77 2069 6e66 6f20 6162    | Show info ab
+000079a0: 6f75 7420 6672 616d 6577 6f72 6b20 2620  out framework & 
+000079b0: 7379 7374 656d 207c 0a20 2020 207c 201b  system |.    | .
+000079c0: 5b31 3b34 393b 3937 6d63 6861 6e67 651b  [1;49;97mchange.
+000079d0: 5b30 6d20 2020 2020 2020 207c 2043 6861  [0m        | Cha
+000079e0: 6e67 6520 7573 6572 2063 6f6d 6d61 6e64  nge user command
+000079f0: 2069 6e70 7574 2063 6f6c 6f72 2020 2020   input color    
+00007a00: 7c0a 2020 2020 7c2d 2d2d 2d2d 2d2d 2d2d  |.    |---------
+00007a10: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00007a20: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00007a30: 2d2d 2d2d 2d2d 2d2d 2d2d 2d7c 0a20 2020  -----------|.   
+00007a40: 207c 2020 2020 2020 2020 2020 2020 2020   |              
+00007a50: 2020 203c 5363 616e 6e65 7220 436f 6d6d     <Scanner Comm
+00007a60: 616e 6473 3e20 2020 2020 2020 2020 2020  ands>           
+00007a70: 2020 2020 2020 7c0a 2020 2020 7c2d 2d2d        |.    |---
+00007a80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00007a90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00007aa0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00007ab0: 2d7c 0a20 2020 207c 201b 5b31 3b34 393b  -|.    | .[1;49;
+00007ac0: 3937 6d6e 756d 6265 721b 5b30 6d20 2020  97mnumber.[0m   
+00007ad0: 2020 2020 207c 2052 6576 6572 7365 2070       | Reverse p
+00007ae0: 686f 6e65 206e 756d 6265 7220 6c6f 6f6b  hone number look
+00007af0: 7570 202a 2020 2020 2020 7c0a 2020 2020  up *      |.    
+00007b00: 7c20 1b5b 313b 3439 3b39 376d 6970 1b5b  | .[1;49;97mip.[
+00007b10: 306d 2020 2020 2020 2020 2020 2020 7c20  0m            | 
+00007b20: 5265 7665 7273 6520 6970 2061 6464 7265  Reverse ip addre
+00007b30: 7373 206c 6f6f 6b75 7020 2a20 2020 2020  ss lookup *     
+00007b40: 2020 207c 0a20 2020 207c 201b 5b31 3b34     |.    | .[1;4
+00007b50: 393b 3937 6d6d 6163 1b5b 306d 2020 2020  9;97mmac.[0m    
+00007b60: 2020 2020 2020 207c 2052 6576 6572 7365         | Reverse
+00007b70: 206d 6163 2061 6464 7265 7373 206c 6f6f   mac address loo
+00007b80: 6b75 7020 2020 2020 2020 2020 7c0a 2020  kup         |.  
+00007b90: 2020 7c20 1b5b 313b 3439 3b39 376d 7768    | .[1;49;97mwh
+00007ba0: 6f69 731b 5b30 6d20 2020 2020 2020 2020  ois.[0m         
+00007bb0: 7c20 5265 7665 7273 6520 7768 6f69 7320  | Reverse whois 
+00007bc0: 6c6f 6f6b 7570 202a 2020 2020 2020 2020  lookup *        
+00007bd0: 2020 2020 207c 0a20 2020 207c 201b 5b31       |.    | .[1
+00007be0: 3b34 393b 3937 6d64 6e73 1b5b 306d 2020  ;49;97mdns.[0m  
+00007bf0: 2020 2020 2020 2020 207c 2052 6576 6572           | Rever
+00007c00: 7365 206f 7220 6e6f 726d 616c 2044 4e53  se or normal DNS
+00007c10: 206c 6f6f 6b75 7020 2020 2020 2020 7c0a   lookup       |.
+00007c20: 2020 2020 7c2d 2d2d 2d2d 2d2d 2d2d 2d2d      |-----------
+00007c30: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00007c40: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00007c50: 2d2d 2d2d 2d2d 2d2d 2d7c 0a20 2020 207c  ---------|.    |
+00007c60: 201b 5b31 3b34 393b 3931 6d4d 4f52 4520   .[1;49;91mMORE 
+00007c70: 5343 414e 4e45 5253 2043 4f4d 494e 4720  SCANNERS COMING 
+00007c80: 534f 4f4e 2c20 5448 4953 2049 5320 4120  SOON, THIS IS A 
+00007c90: 4245 5441 2056 4552 1b5b 306d 2020 2020  BETA VER.[0m    
+00007ca0: 2020 7c0a 2020 2020 e294 94e2 9480 e294    |.    ........
+00007cb0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00007cc0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00007cd0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00007ce0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00007cf0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00007d00: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00007d10: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00007d20: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00007d30: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00007d40: 80e2 9480 e294 80e2 9498 0a20 2020 2029  ...........    )
+00007d50: 057a 4e54 7970 6520 601b 5b37 3b34 393b  .zNType `.[7;49;
+00007d60: 3933 6d68 656c 7020 3c63 6f6d 6d61 6e64  93mhelp <command
+00007d70: 3e1b 5b30 6d1b 5b31 3b34 393b 3933 6d60  >.[0m.[1;49;93m`
+00007d80: 2074 6f20 7365 6520 6d6f 7265 2069 6e66   to see more inf
+00007d90: 6f20 6162 6f75 7420 6120 636f 6d6d 616e  o about a comman
+00007da0: 647a 3f55 7365 2060 1b5b 373b 3439 3b39  dz?Use `.[7;49;9
+00007db0: 336d 5461 621b 5b30 6d1b 5b31 3b34 393b  3mTab.[0m.[1;49;
+00007dc0: 3933 6d60 206b 6579 2074 6f20 6175 746f  93m` key to auto
+00007dd0: 2d63 6f6d 706c 6574 6520 636f 6d6d 616e  -complete comman
+00007de0: 6473 7a5d 5472 7920 7369 6c65 6e74 206d  dsz]Try silent m
+00007df0: 6f64 6520 6279 2075 7369 6e67 2060 1b5b  ode by using `.[
+00007e00: 373b 3439 3b39 336d 2d73 1b5b 306d 1b5b  7;49;93m-s.[0m.[
+00007e10: 313b 3439 3b39 336d 602f 601b 5b37 3b34  1;49;93m`/`.[7;4
+00007e20: 393b 3933 6d2d 2d73 696c 656e 741b 5b30  9;93m--silent.[0
+00007e30: 6d1b 5b31 3b34 393b 3933 6d60 2066 6c61  m.[1;49;93m` fla
+00007e40: 677a 3959 6f75 2063 616e 2061 6c73 6f20  gz9You can also 
+00007e50: 7573 6520 601b 5b37 3b34 393b 3933 6d43  use `.[7;49;93mC
+00007e60: 7472 6c2b 431b 5b30 6d1b 5b31 3b34 393b  trl+C.[0m.[1;49;
+00007e70: 3933 6d60 2074 6f20 6578 6974 7a4e 4465  93m` to exitzNDe
+00007e80: 7363 7269 7074 696f 6e73 2065 6e64 696e  scriptions endin
+00007e90: 6720 7769 7468 2060 1b5b 373b 3439 3b39  g with `.[7;49;9
+00007ea0: 336d 2a1b 5b30 6d1b 5b31 3b34 393b 3933  3m*.[0m.[1;49;93
+00007eb0: 6d60 206e 6565 6473 2069 6e74 6572 6e65  m` needs interne
+00007ec0: 7420 636f 6e6e 6563 7469 6f6e 7213 0000  t connectionr...
+00007ed0: 007a 0d74 6162 3a20 636f 6d70 6c65 7465  .z.tab: complete
+00007ee0: 7a0a 1b5b 313b 3439 3b39 306d 7a0a 1b5b  z..[1;49;90mz..[
+00007ef0: 313b 3439 3b39 376d 7a06 0a1b 5b30 6d5b  1;49;97mz...[0m[
+00007f00: 750e 0000 0040 7068 306d 6265 725d e2b8  u....@ph0mber]..
+00007f10: ba20 5b7a 045d 2024 2029 0272 ac00 0000  . [z.] $ ).r....
+00007f20: 72aa 0000 0072 0a00 0000 7a10 1b5b 313b  r....r....z..[1;
+00007f30: 3439 3b39 336d 2020 2020 3e20 e904 0000  49;93m    > ....
+00007f40: 00fa 0123 e905 0000 0061 2b01 0000 2020  ...#.....a+...  
+00007f50: 1b5b 313b 3439 3b39 336d 5b2b 5d20 436f  .[1;49;93m[+] Co
+00007f60: 6d6d 616e 6420 496e 666f 3a20 1b5b 313b  mmand Info: .[1;
+00007f70: 3439 3b39 336d 6865 6c70 0a0a 2020 2020  49;93mhelp..    
+00007f80: 1b5b 313b 3439 3b39 326d 3e20 4445 5343  .[1;49;92m> DESC
+00007f90: 5249 5054 494f 4e3a 201b 5b31 3b34 393b  RIPTION: .[1;49;
+00007fa0: 3937 6d57 6865 6e20 796f 7520 7479 7065  97mWhen you type
+00007fb0: 2060 6865 6c70 602c 2074 6865 2068 656c   `help`, the hel
+00007fc0: 7020 6d65 6e75 2077 696c 6c20 6265 2064  p menu will be d
+00007fd0: 6973 706c 6179 6564 0a20 2020 201b 5b31  isplayed.    .[1
+00007fe0: 3b34 393b 3932 6d3e 2053 594e 5441 583a  ;49;92m> SYNTAX:
+00007ff0: 201b 5b31 3b34 393b 3937 6d68 656c 7020   .[1;49;97mhelp 
+00008000: 1b5b 313b 3439 3b39 326d 4f52 201b 5b31  .[1;49;92mOR .[1
+00008010: 3b34 393b 3937 6d68 656c 7020 3c63 6f6d  ;49;97mhelp <com
+00008020: 6d61 6e64 3e0a 2020 2020 1b5b 313b 3439  mand>.    .[1;49
+00008030: 3b39 326d 3e20 4558 414d 504c 453a 201b  ;92m> EXAMPLE: .
+00008040: 5b31 3b34 393b 3937 6d68 656c 7020 1b5b  [1;49;97mhelp .[
+00008050: 313b 3439 3b39 326d 4f52 201b 5b31 3b34  1;49;92mOR .[1;4
+00008060: 393b 3937 6d68 656c 7020 6e75 6d62 6572  9;97mhelp number
+00008070: 0a20 2020 201b 5b30 6d72 0800 0000 720f  .    .[0mr....r.
+00008080: 0000 007a ee20 201b 5b31 3b34 393b 3933  ...z.  .[1;49;93
+00008090: 6d5b 2b5d 2043 6f6d 6d61 6e64 2049 6e66  m[+] Command Inf
+000080a0: 6f3a 201b 5b31 3b34 393b 3933 6d65 7869  o: .[1;49;93mexi
+000080b0: 742f 1b5b 313b 3439 3b39 336d 7175 6974  t/.[1;49;93mquit
+000080c0: 0a0a 2020 2020 1b5b 313b 3439 3b39 326d  ..    .[1;49;92m
+000080d0: 3e20 4445 5343 5249 5054 494f 4e3a 201b  > DESCRIPTION: .
+000080e0: 5b31 3b34 393b 3937 6d57 6865 6e20 796f  [1;49;97mWhen yo
+000080f0: 7520 7479 7065 2060 6578 6974 6020 6f72  u type `exit` or
+00008100: 2060 7175 6974 602c 2074 6865 2070 726f   `quit`, the pro
+00008110: 6772 616d 2077 696c 6c20 6265 2074 6572  gram will be ter
+00008120: 6d69 6e61 7465 640a 2020 2020 1b5b 313b  minated.    .[1;
+00008130: 3439 3b39 326d 3e20 5359 4e54 4158 3a20  49;92m> SYNTAX: 
+00008140: 1b5b 313b 3439 3b39 376d 6578 6974 201b  .[1;49;97mexit .
+00008150: 5b31 3b34 393b 3932 6d4f 5220 1b5b 313b  [1;49;92mOR .[1;
+00008160: 3439 3b39 376d 7175 6974 0a20 2020 201b  49;97mquit.    .
+00008170: 5b30 6d72 0600 0000 7ac7 2020 1b5b 313b  [0mr....z.  .[1;
+00008180: 3439 3b39 336d 5b2b 5d20 436f 6d6d 616e  49;93m[+] Comman
+00008190: 6420 496e 666f 3a20 1b5b 313b 3439 3b39  d Info: .[1;49;9
+000081a0: 336d 646f 726b 0a0a 2020 2020 1b5b 313b  3mdork..    .[1;
+000081b0: 3439 3b39 326d 3e20 4445 5343 5249 5054  49;92m> DESCRIPT
+000081c0: 494f 4e3a 201b 5b31 3b34 393b 3937 6d57  ION: .[1;49;97mW
+000081d0: 6865 6e20 796f 7520 7479 7065 2060 646f  hen you type `do
+000081e0: 726b 602c 2061 2072 616e 646f 6d20 676f  rk`, a random go
+000081f0: 6f67 6c65 2064 6f72 6b20 7175 6572 7920  ogle dork query 
+00008200: 7769 6c6c 2062 6520 6469 7370 6c61 7965  will be displaye
+00008210: 640a 2020 2020 1b5b 313b 3439 3b39 326d  d.    .[1;49;92m
+00008220: 3e20 5359 4e54 4158 3a20 1b5b 313b 3439  > SYNTAX: .[1;49
+00008230: 3b39 376d 646f 726b 0a20 2020 201b 5b30  ;97mdork.    .[0
+00008240: 6d72 0900 0000 7ace 2020 1b5b 313b 3439  mr....z.  .[1;49
+00008250: 3b39 336d 5b2b 5d20 436f 6d6d 616e 6420  ;93m[+] Command 
+00008260: 496e 666f 3a20 1b5b 313b 3439 3b39 336d  Info: .[1;49;93m
+00008270: 6578 700a 0a20 2020 201b 5b31 3b34 393b  exp..    .[1;49;
+00008280: 3932 6d3e 2044 4553 4352 4950 5449 4f4e  92m> DESCRIPTION
+00008290: 3a20 1b5b 313b 3439 3b39 376d 5768 656e  : .[1;49;97mWhen
+000082a0: 2079 6f75 2074 7970 6520 6065 7870 602c   you type `exp`,
+000082b0: 2069 6e66 6f20 6162 6f75 7420 616c 6c20   info about all 
+000082c0: 6176 6169 6c61 626c 6520 6578 7072 6573  available expres
+000082d0: 7369 6f6e 7320 7769 6c6c 2062 6520 6469  sions will be di
+000082e0: 7370 6c61 7965 640a 2020 2020 1b5b 313b  splayed.    .[1;
+000082f0: 3439 3b39 326d 3e20 5359 4e54 4158 3a20  49;92m> SYNTAX: 
+00008300: 1b5b 313b 3439 3b39 376d 6578 700a 2020  .[1;49;97mexp.  
+00008310: 2020 1b5b 306d 7204 0000 007a d020 201b    .[0mr....z.  .
+00008320: 5b31 3b34 393b 3933 6d5b 2b5d 2043 6f6d  [1;49;93m[+] Com
+00008330: 6d61 6e64 2049 6e66 6f3a 201b 5b31 3b34  mand Info: .[1;4
+00008340: 393b 3933 6d63 6865 636b 0a0a 2020 2020  9;93mcheck..    
+00008350: 1b5b 313b 3439 3b39 326d 3e20 4445 5343  .[1;49;92m> DESC
+00008360: 5249 5054 494f 4e3a 201b 5b31 3b34 393b  RIPTION: .[1;49;
+00008370: 3937 6d57 6865 6e20 796f 7520 7479 7065  97mWhen you type
+00008380: 2060 6368 6563 6b60 2c20 6974 2077 696c   `check`, it wil
+00008390: 6c20 6368 6563 6b20 666f 7220 696e 7465  l check for inte
+000083a0: 726e 6574 2063 6f6e 6e65 6374 696f 6e20  rnet connection 
+000083b0: 6176 6169 6c61 6269 6c69 7479 0a20 2020  availability.   
+000083c0: 201b 5b31 3b34 393b 3932 6d3e 2053 594e   .[1;49;92m> SYN
+000083d0: 5441 583a 201b 5b31 3b34 393b 3937 6d63  TAX: .[1;49;97mc
+000083e0: 6865 636b 0a20 2020 201b 5b30 6d72 0500  heck.    .[0mr..
+000083f0: 0000 7ab6 2020 1b5b 313b 3439 3b39 336d  ..z.  .[1;49;93m
+00008400: 5b2b 5d20 436f 6d6d 616e 6420 496e 666f  [+] Command Info
+00008410: 3a20 1b5b 313b 3439 3b39 336d 636c 6561  : .[1;49;93mclea
+00008420: 720a 0a20 2020 201b 5b31 3b34 393b 3932  r..    .[1;49;92
+00008430: 6d3e 2044 4553 4352 4950 5449 4f4e 3a20  m> DESCRIPTION: 
+00008440: 1b5b 313b 3439 3b39 376d 5768 656e 2079  .[1;49;97mWhen y
+00008450: 6f75 2074 7970 6520 6063 6c65 6172 602c  ou type `clear`,
+00008460: 2069 7420 7769 6c6c 2063 6c65 6172 2074   it will clear t
+00008470: 6865 2073 6372 6565 6e0a 2020 2020 1b5b  he screen.    .[
+00008480: 313b 3439 3b39 326d 3e20 5359 4e54 4158  1;49;92m> SYNTAX
+00008490: 3a20 1b5b 313b 3439 3b39 376d 636c 6561  : .[1;49;97mclea
+000084a0: 720a 2020 2020 1b5b 306d 7210 0000 007a  r.    .[0mr....z
+000084b0: ee20 201b 5b31 3b34 393b 3933 6d5b 2b5d  .  .[1;49;93m[+]
+000084c0: 2043 6f6d 6d61 6e64 2049 6e66 6f3a 201b   Command Info: .
+000084d0: 5b31 3b34 393b 3933 6d73 6176 650a 0a20  [1;49;93msave.. 
+000084e0: 2020 201b 5b31 3b34 393b 3932 6d3e 2044     .[1;49;92m> D
+000084f0: 4553 4352 4950 5449 4f4e 3a20 1b5b 313b  ESCRIPTION: .[1;
+00008500: 3439 3b39 376d 5768 656e 2079 6f75 2074  49;97mWhen you t
+00008510: 7970 6520 6073 6176 6560 2c20 6974 2077  ype `save`, it w
+00008520: 696c 6c20 7361 7665 2074 6865 206f 7574  ill save the out
+00008530: 7075 7420 6f66 2070 7265 7669 6f75 7320  put of previous 
+00008540: 636f 6d6d 616e 640a 2020 2020 1b5b 313b  command.    .[1;
+00008550: 3439 3b39 326d 3e20 5359 4e54 4158 3a20  49;92m> SYNTAX: 
+00008560: 1b5b 313b 3439 3b39 376d 7361 7665 0a20  .[1;49;97msave. 
+00008570: 2020 201b 5b31 3b34 393b 3932 6d3e 2045     .[1;49;92m> E
+00008580: 5841 4d50 4c45 3a20 1b5b 313b 3439 3b39  XAMPLE: .[1;49;9
+00008590: 376d 7361 7665 0a20 2020 201b 5b30 6d72  7msave.    .[0mr
+000085a0: 1100 0000 6101 0100 0020 201b 5b31 3b34  ....a....  .[1;4
+000085b0: 393b 3933 6d5b 2b5d 2043 6f6d 6d61 6e64  9;93m[+] Command
+000085c0: 2049 6e66 6f3a 201b 5b31 3b34 393b 3933   Info: .[1;49;93
+000085d0: 6d73 6865 6c6c 0a0a 2020 2020 1b5b 313b  mshell..    .[1;
+000085e0: 3439 3b39 326d 3e20 4445 5343 5249 5054  49;92m> DESCRIPT
+000085f0: 494f 4e3a 201b 5b31 3b34 393b 3937 6d57  ION: .[1;49;97mW
+00008600: 6865 6e20 796f 7520 7479 7065 2060 7368  hen you type `sh
+00008610: 656c 6c60 2c20 6974 2077 696c 6c20 6578  ell`, it will ex
+00008620: 6563 7574 6520 6769 7665 6e20 636f 6d6d  ecute given comm
+00008630: 616e 6420 696e 206e 6174 6976 6520 7368  and in native sh
+00008640: 656c 6c2f 636d 640a 2020 2020 1b5b 313b  ell/cmd.    .[1;
+00008650: 3439 3b39 326d 3e20 5359 4e54 4158 3a20  49;92m> SYNTAX: 
+00008660: 1b5b 313b 3439 3b39 376d 7368 656c 6c20  .[1;49;97mshell 
+00008670: 3c63 6d64 3e0a 2020 2020 1b5b 313b 3439  <cmd>.    .[1;49
+00008680: 3b39 326d 3e20 4558 414d 504c 453a 201b  ;92m> EXAMPLE: .
+00008690: 5b31 3b34 393b 3937 6d73 6865 6c6c 206c  [1;49;97mshell l
+000086a0: 730a 2020 2020 1b5b 306d 720b 0000 007a  s.    .[0mr....z
+000086b0: c520 201b 5b31 3b34 393b 3933 6d5b 2b5d  .  .[1;49;93m[+]
+000086c0: 2043 6f6d 6d61 6e64 2049 6e66 6f3a 201b   Command Info: .
+000086d0: 5b31 3b34 393b 3933 6d69 6e66 6f0a 0a20  [1;49;93minfo.. 
+000086e0: 2020 201b 5b31 3b34 393b 3932 6d3e 2044     .[1;49;92m> D
+000086f0: 4553 4352 4950 5449 4f4e 3a20 1b5b 313b  ESCRIPTION: .[1;
+00008700: 3439 3b39 376d 5768 656e 2079 6f75 2074  49;97mWhen you t
+00008710: 7970 6520 6069 6e66 6f60 2c20 6974 2077  ype `info`, it w
+00008720: 696c 6c20 7368 6f77 2069 6e66 6f20 6162  ill show info ab
+00008730: 6f75 7420 6672 616d 6577 6f72 6b20 2620  out framework & 
+00008740: 7379 7374 656d 0a20 2020 201b 5b31 3b34  system.    .[1;4
+00008750: 393b 3932 6d3e 2053 594e 5441 583a 201b  9;92m> SYNTAX: .
+00008760: 5b31 3b34 393b 3937 6d69 6e66 6f0a 2020  [1;49;97minfo.  
+00008770: 2020 1b5b 306d 7203 0000 0061 8a01 0000    .[0mr....a....
+00008780: 2020 1b5b 313b 3439 3b39 336d 5b2b 5d20    .[1;49;93m[+] 
+00008790: 436f 6d6d 616e 6420 496e 666f 3a20 1b5b  Command Info: .[
+000087a0: 313b 3439 3b39 336d 6368 616e 6765 0a0a  1;49;93mchange..
+000087b0: 2020 2020 1b5b 313b 3439 3b39 326d 3e20      .[1;49;92m> 
+000087c0: 4445 5343 5249 5054 494f 4e3a 201b 5b31  DESCRIPTION: .[1
+000087d0: 3b34 393b 3937 6d57 6865 6e20 796f 7520  ;49;97mWhen you 
+000087e0: 7479 7065 2060 6368 616e 6765 602c 2069  type `change`, i
+000087f0: 7420 7769 6c6c 2063 6861 6e67 6520 7573  t will change us
+00008800: 6572 2063 6f6d 6d61 6e64 2069 6e70 7574  er command input
+00008810: 2063 6f6c 6f72 0a20 2020 201b 5b31 3b34   color.    .[1;4
+00008820: 393b 3932 6d3e 204f 5054 494f 4e53 3a20  9;92m> OPTIONS: 
+00008830: 1b5b 313b 3439 3b39 376d 3020 2d3e 201b  .[1;49;97m0 -> .
+00008840: 5b31 3b34 393b 3930 6d42 6c61 636b 0a20  [1;49;90mBlack. 
+00008850: 2020 2020 2020 2020 2020 2020 2020 1b5b                .[
+00008860: 313b 3439 3b39 376d 3120 2d3e 2057 6869  1;49;97m1 -> Whi
+00008870: 7465 2020 2020 2020 2020 0a20 2020 201b  te        .    .
+00008880: 5b31 3b34 393b 3932 6d3e 2044 6566 6175  [1;49;92m> Defau
+00008890: 6c74 3a20 1b5b 313b 3439 3b39 376d 310a  lt: .[1;49;97m1.
+000088a0: 2020 2020 1b5b 313b 3439 3b39 326d 3e20      .[1;49;92m> 
+000088b0: 5359 4e54 4158 3a20 1b5b 313b 3439 3b39  SYNTAX: .[1;49;9
+000088c0: 376d 6368 616e 6765 203c 636f 6c6f 725f  7mchange <color_
+000088d0: 636f 6465 3e0a 2020 2020 1b5b 313b 3439  code>.    .[1;49
+000088e0: 3b39 326d 3e20 4558 414d 504c 453a 201b  ;92m> EXAMPLE: .
+000088f0: 5b31 3b34 393b 3937 6d63 6861 6e67 6520  [1;49;97mchange 
+00008900: 300a 2020 2020 1b5b 306d 720e 0000 0061  0.    .[0mr....a
+00008910: 3f01 0000 2020 1b5b 313b 3439 3b39 336d  ?...  .[1;49;93m
+00008920: 5b2b 5d20 436f 6d6d 616e 6420 496e 666f  [+] Command Info
+00008930: 3a20 1b5b 313b 3439 3b39 336d 6e75 6d62  : .[1;49;93mnumb
+00008940: 6572 0a0a 2020 2020 1b5b 313b 3439 3b39  er..    .[1;49;9
+00008950: 326d 3e20 4445 5343 5249 5054 494f 4e3a  2m> DESCRIPTION:
+00008960: 201b 5b31 3b34 393b 3937 6d57 6865 6e20   .[1;49;97mWhen 
+00008970: 796f 7520 7479 7065 2060 6e75 6d62 6572  you type `number
+00008980: 602c 2069 7420 7769 6c6c 2072 6576 6572  `, it will rever
+00008990: 7365 206c 6f6f 6b75 7020 7068 6f6e 6520  se lookup phone 
+000089a0: 6e75 6d62 6572 206f 7665 7220 696e 7465  number over inte
+000089b0: 726e 6574 2061 6e64 2073 686f 7720 7075  rnet and show pu
+000089c0: 626c 6963 2069 6e66 6f20 6173 736f 6369  blic info associ
+000089d0: 6174 6564 2077 6974 6820 6974 0a20 2020  ated with it.   
+000089e0: 201b 5b31 3b34 393b 3932 6d3e 2053 594e   .[1;49;92m> SYN
+000089f0: 5441 583a 201b 5b31 3b34 393b 3937 6d6e  TAX: .[1;49;97mn
+00008a00: 756d 6265 7220 3c70 686f 6e65 5f6e 756d  umber <phone_num
+00008a10: 6265 723e 0a20 2020 201b 5b31 3b34 393b  ber>.    .[1;49;
+00008a20: 3932 6d3e 2045 5841 4d50 4c45 3a20 1b5b  92m> EXAMPLE: .[
+00008a30: 313b 3439 3b39 376d 6e75 6d62 6572 202b  1;49;97mnumber +
+00008a40: 3132 3334 3536 3738 3930 0a20 2020 201b  1234567890.    .
+00008a50: 5b30 6d72 1200 0000 6105 0100 0020 201b  [0mr....a....  .
+00008a60: 5b31 3b34 393b 3933 6d5b 2b5d 2043 6f6d  [1;49;93m[+] Com
+00008a70: 6d61 6e64 2049 6e66 6f3a 201b 5b31 3b34  mand Info: .[1;4
+00008a80: 393b 3933 6d77 686f 6973 0a0a 2020 2020  9;93mwhois..    
+00008a90: 1b5b 313b 3439 3b39 326d 3e20 4445 5343  .[1;49;92m> DESC
+00008aa0: 5249 5054 494f 4e3a 201b 5b31 3b34 393b  RIPTION: .[1;49;
+00008ab0: 3937 6d57 6865 6e20 796f 7520 7479 7065  97mWhen you type
+00008ac0: 2060 7768 6f69 7360 2c20 6974 2077 696c   `whois`, it wil
+00008ad0: 6c20 7065 7266 6f72 6d20 7265 7665 7273  l perform revers
+00008ae0: 6520 7768 6f69 7320 6c6f 6f6b 7570 0a20  e whois lookup. 
+00008af0: 2020 201b 5b31 3b34 393b 3932 6d3e 2053     .[1;49;92m> S
+00008b00: 594e 5441 583a 201b 5b31 3b34 393b 3937  YNTAX: .[1;49;97
+00008b10: 6d77 686f 6973 203c 646f 6d61 696e 5f6e  mwhois <domain_n
+00008b20: 616d 653e 0a20 2020 201b 5b31 3b34 393b  ame>.    .[1;49;
+00008b30: 3932 6d3e 2045 5841 4d50 4c45 3a20 1b5b  92m> EXAMPLE: .[
+00008b40: 313b 3439 3b39 376d 7768 6f69 7320 6578  1;49;97mwhois ex
+00008b50: 616d 706c 652e 636f 6d0a 2020 2020 1b5b  ample.com.    .[
+00008b60: 306d 7207 0000 0061 6601 0000 2020 1b5b  0mr....af...  .[
+00008b70: 313b 3439 3b39 336d 5b2b 5d20 436f 6d6d  1;49;93m[+] Comm
+00008b80: 616e 6420 496e 666f 3a20 1b5b 313b 3439  and Info: .[1;49
+00008b90: 3b39 336d 646e 730a 0a20 2020 201b 5b31  ;93mdns..    .[1
+00008ba0: 3b34 393b 3932 6d3e 2044 4553 4352 4950  ;49;92m> DESCRIP
+00008bb0: 5449 4f4e 3a20 1b5b 313b 3439 3b39 376d  TION: .[1;49;97m
+00008bc0: 5768 656e 2079 6f75 2074 7970 6520 6064  When you type `d
+00008bd0: 6e73 602c 2069 7420 7769 6c6c 2070 6572  ns`, it will per
+00008be0: 666f 726d 2064 6e73 206c 6f6f 6b75 7020  form dns lookup 
+00008bf0: 666f 7220 6769 7665 6e20 646f 6d61 696e  for given domain
+00008c00: 206e 616d 6520 6f72 2072 6576 6572 7365   name or reverse
+00008c10: 2064 6e73 206c 6f6f 6b75 7020 666f 7220   dns lookup for 
+00008c20: 6769 7665 6e20 6970 2061 6464 7265 7373  given ip address
+00008c30: 0a20 2020 201b 5b31 3b34 393b 3932 6d3e  .    .[1;49;92m>
+00008c40: 2053 594e 5441 583a 201b 5b31 3b34 393b   SYNTAX: .[1;49;
+00008c50: 3937 6d64 6e73 203c 6970 5f61 6464 7265  97mdns <ip_addre
+00008c60: 7373 2f64 6f6d 6169 6e5f 6e61 6d65 3e0a  ss/domain_name>.
+00008c70: 2020 2020 1b5b 313b 3439 3b39 326d 3e20      .[1;49;92m> 
+00008c80: 4558 414d 504c 453a 201b 5b31 3b34 393b  EXAMPLE: .[1;49;
+00008c90: 3937 6d64 6e73 2031 3932 2e31 3638 2e31  97mdns 192.168.1
+00008ca0: 2e31 201b 5b31 3b34 393b 3932 6d4f 5220  .1 .[1;49;92mOR 
+00008cb0: 1b5b 313b 3439 3b39 376d 646e 7320 6578  .[1;49;97mdns ex
+00008cc0: 616d 706c 652e 636f 6d0a 2020 2020 1b5b  ample.com.    .[
+00008cd0: 306d 720c 0000 0061 2701 0000 2020 1b5b  0mr....a'...  .[
+00008ce0: 313b 3439 3b39 336d 5b2b 5d20 436f 6d6d  1;49;93m[+] Comm
+00008cf0: 616e 6420 496e 666f 3a20 1b5b 313b 3439  and Info: .[1;49
+00008d00: 3b39 336d 6970 0a0a 2020 2020 1b5b 313b  ;93mip..    .[1;
+00008d10: 3439 3b39 326d 3e20 4445 5343 5249 5054  49;92m> DESCRIPT
+00008d20: 494f 4e3a 201b 5b31 3b34 393b 3937 6d57  ION: .[1;49;97mW
+00008d30: 6865 6e20 796f 7520 7479 7065 2060 6970  hen you type `ip
+00008d40: 602c 2069 7420 7769 6c6c 2070 6572 666f  `, it will perfo
+00008d50: 726d 2061 6e20 6970 2061 6464 7265 7373  rm an ip address
+00008d60: 206c 6f6f 6b75 7020 6f76 6572 2069 6e74   lookup over int
+00008d70: 6572 6e65 7420 616e 6420 7368 6f77 2069  ernet and show i
+00008d80: 6e66 6f20 6162 6f75 7420 6769 7665 6e20  nfo about given 
+00008d90: 6970 2061 6464 7265 7373 0a20 2020 201b  ip address.    .
+00008da0: 5b31 3b34 393b 3932 6d3e 2053 594e 5441  [1;49;92m> SYNTA
+00008db0: 583a 201b 5b31 3b34 393b 3937 6d69 7020  X: .[1;49;97mip 
+00008dc0: 3c69 705f 6164 6472 6573 733e 0a20 2020  <ip_address>.   
+00008dd0: 201b 5b31 3b34 393b 3932 6d3e 2045 5841   .[1;49;92m> EXA
+00008de0: 4d50 4c45 3a20 1b5b 313b 3439 3b39 376d  MPLE: .[1;49;97m
+00008df0: 6970 2038 2e38 2e38 2e38 0a20 2020 201b  ip 8.8.8.8.    .
+00008e00: 5b30 6d72 0d00 0000 611e 0100 0020 201b  [0mr....a....  .
+00008e10: 5b31 3b34 393b 3933 6d5b 2b5d 2043 6f6d  [1;49;93m[+] Com
+00008e20: 6d61 6e64 2049 6e66 6f3a 201b 5b31 3b34  mand Info: .[1;4
+00008e30: 393b 3933 6d6d 6163 0a0a 2020 2020 1b5b  9;93mmac..    .[
+00008e40: 313b 3439 3b39 326d 3e20 4445 5343 5249  1;49;92m> DESCRI
+00008e50: 5054 494f 4e3a 201b 5b31 3b34 393b 3937  PTION: .[1;49;97
+00008e60: 6d57 6865 6e20 796f 7520 7479 7065 2060  mWhen you type `
+00008e70: 6d61 6360 2c20 6974 2077 696c 6c20 6c6f  mac`, it will lo
+00008e80: 6f6b 7570 2070 726f 6261 626c 6520 7665  okup probable ve
+00008e90: 6e64 6f72 2f6d 616e 7566 6163 7475 7265  ndor/manufacture
+00008ea0: 206f 6620 6769 7665 6e20 6d61 6320 6164   of given mac ad
+00008eb0: 6472 6573 730a 2020 2020 1b5b 313b 3439  dress.    .[1;49
+00008ec0: 3b39 326d 3e20 5359 4e54 4158 3a20 1b5b  ;92m> SYNTAX: .[
+00008ed0: 313b 3439 3b39 376d 6d61 6320 3c6d 6163  1;49;97mmac <mac
+00008ee0: 5f61 6464 7265 7373 3e0a 2020 2020 1b5b  _address>.    .[
+00008ef0: 313b 3439 3b39 326d 3e20 4558 414d 504c  1;49;92m> EXAMPL
+00008f00: 453a 201b 5b31 3b34 393b 3937 6d6d 6163  E: .[1;49;97mmac
+00008f10: 2066 663a 6666 3a66 663a 6666 3a66 663a   ff:ff:ff:ff:ff:
+00008f20: 6666 0a20 2020 201b 5b30 6de9 0300 0000  ff.    .[0m.....
+00008f30: 7a47 2020 2020 5b21 5d20 496e 7661 6c69  zG    [!] Invali
+00008f40: 6420 7375 622d 636f 6d6d 616e 6421 2054  d sub-command! T
+00008f50: 7970 6520 6068 656c 7060 2074 6f20 7365  ype `help` to se
+00008f60: 6520 616c 6c20 6176 6169 6c61 626c 6520  e all available 
+00008f70: 636f 6d6d 616e 6473 2e72 2c00 0000 722e  commands.r,...r.
+00008f80: 0000 007a 4320 2020 205b 215d 2049 6e76  ...zC    [!] Inv
+00008f90: 616c 6964 2063 6f6d 6d61 6e64 2120 5479  alid command! Ty
+00008fa0: 7065 2060 6865 6c70 6020 746f 2073 6565  pe `help` to see
+00008fb0: 2061 6c6c 2061 7661 696c 6162 6c65 2063   all available c
+00008fc0: 6f6d 6d61 6e64 732e 7a38 2020 2020 5b40  ommands.z8    [@
+00008fd0: 5d20 5468 616e 6b20 796f 7520 666f 7220  ] Thank you for 
+00008fe0: 7573 696e 6720 6050 4830 4d42 4552 6020  using `PH0MBER` 
+00008ff0: 6f73 696e 7420 6672 616d 6577 6f72 6b20  osint framework 
+00009000: 3a29 7a27 2020 2020 5b2b 5d20 4765 6e65  :)z'    [+] Gene
+00009010: 7261 7469 6e67 2072 616e 646f 6d20 646f  rating random do
+00009020: 726b 2071 7565 7279 2e2e 2e72 2300 0000  rk query...r#...
+00009030: 7227 0000 007a 0620 2020 203e 2029 0372  r'...z.    > ).r
+00009040: 2400 0000 7225 0000 0072 c600 0000 7a27  $...r%...r....z'
+00009050: 2020 2020 5b2b 5d20 4368 6563 6b69 6e67      [+] Checking
+00009060: 2069 6e74 6572 6e65 7420 636f 6e6e 6563   internet connec
+00009070: 7469 6f6e 2e2e 2e7a 1768 7474 7073 3a2f  tion...z.https:/
+00009080: 2f77 7777 2e67 6f6f 676c 652e 636f 6d2f  /www.google.com/
+00009090: 7a27 2020 2020 3e20 496e 7465 726e 6574  z'    > Internet
+000090a0: 2063 6f6e 6e65 6374 696f 6e20 6973 2061   connection is a
+000090b0: 7661 696c 6162 6c65 217a 1668 7474 7073  vailable!z.https
+000090c0: 3a2f 2f68 7474 7062 696e 2e6f 7267 2f69  ://httpbin.org/i
+000090d0: 70da 066f 7269 6769 6e7a 1068 7474 7073  p..originz.https
+000090e0: 3a2f 2f69 6465 6e74 2e6d 657a 1568 7474  ://ident.mez.htt
+000090f0: 7073 3a2f 2f61 7069 2e69 7069 6679 2e6f  ps://api.ipify.o
+00009100: 7267 467a 1920 2020 203e 2050 7562 6c69  rgFz.    > Publi
+00009110: 6320 4950 2061 6464 7265 7373 3a20 7a2b  c IP address: z+
+00009120: 2020 2020 3e20 496e 7465 726e 6574 2063      > Internet c
+00009130: 6f6e 6e65 6374 696f 6e20 6973 206e 6f74  onnection is not
+00009140: 2061 7661 696c 6162 6c65 217a 2120 2020   available!z!   
+00009150: 203e 204c 6f63 616c 2049 5020 6164 6472   > Local IP addr
+00009160: 6573 733a 2031 3237 2e30 2e30 2e31 72af  ess: 127.0.0.1r.
+00009170: 0000 0072 c500 0000 7a2c 2020 2020 5b2b  ...r....z,    [+
+00009180: 5d20 5361 7669 6e67 206f 7574 7075 7420  ] Saving output 
+00009190: 6f66 2070 7265 7669 6f75 7320 636f 6d6d  of previous comm
+000091a0: 616e 642e 2e2e 7a45 2020 2020 3e20 4e6f  and...zE    > No
+000091b0: 206f 7574 7075 7420 666f 756e 6421 2053   output found! S
+000091c0: 6176 6573 206f 7574 7075 7420 6f66 2070  aves output of p
+000091d0: 7265 7669 6f75 7320 7363 616e 6e65 7220  revious scanner 
+000091e0: 636f 6d6d 616e 6420 6f6e 6c79 2172 5300  command only!rS.
+000091f0: 0000 7a3b 2020 2020 3e20 4e6f 2063 6f6d  ..z;    > No com
+00009200: 6d61 6e64 2066 6f75 6e64 2120 5479 7065  mand found! Type
+00009210: 2060 6865 6c70 2073 6865 6c6c 6020 746f   `help shell` to
+00009220: 2073 6565 206d 6f72 6520 696e 666f 2ee9   see more info..
+00009230: 0600 0000 7a25 2020 2020 1b5b 373b 3439  ....z%    .[7;49
+00009240: 3b39 336d 5b2b 5d20 4578 6563 7574 696e  ;93m[+] Executin
+00009250: 6720 636f 6d6d 616e 643a 207a 051b 5b30  g command: z..[0
+00009260: 6d0a 7a20 3e20 436f 6d6d 616e 6420 6578  m.z > Command ex
+00009270: 6563 7574 6564 2073 7563 6365 7373 6675  ecuted successfu
+00009280: 6c6c 7921 2903 e907 0000 0072 2500 0000  lly!)......r%...
+00009290: 72c6 0000 007a 050a 2020 2020 2902 7228  r....z..    ).r(
+000092a0: 0000 0072 ab00 0000 7a1b 3e20 436f 6d6d  ...r....z.> Comm
+000092b0: 616e 6420 6578 6563 7574 696f 6e20 6661  and execution fa
+000092c0: 696c 6564 2129 0372 e300 0000 7225 0000  iled!).r....r%..
+000092d0: 0072 2d00 0000 7a3f 2020 2020 3e20 4e6f  .r-...z?    > No
+000092e0: 2063 6f6c 6f72 2063 6f64 6520 666f 756e   color code foun
+000092f0: 6421 2054 7970 6520 6068 656c 7020 6368  d! Type `help ch
+00009300: 616e 6765 6020 746f 2073 6565 206d 6f72  ange` to see mor
+00009310: 6520 696e 666f 2e72 e300 0000 da01 307a  e info.r......0z
+00009320: 2a20 2020 203e 2043 6f6c 6f72 2063 6861  *    > Color cha
+00009330: 6e67 6564 2073 7563 6365 7373 6675 6c6c  nged successfull
+00009340: 7920 746f 2042 4c41 434b 21da 0131 7a2a  y to BLACK!..1z*
+00009350: 2020 2020 3e20 436f 6c6f 7220 6368 616e      > Color chan
+00009360: 6765 6420 7375 6363 6573 7366 756c 6c79  ged successfully
+00009370: 2074 6f20 5748 4954 4521 7a40 2020 2020   to WHITE!z@    
+00009380: 5b21 5d20 496e 7661 6c69 6420 636f 6c6f  [!] Invalid colo
+00009390: 7220 636f 6465 2120 5479 7065 2060 6865  r code! Type `he
+000093a0: 6c70 2063 6861 6e67 6560 2074 6f20 7365  lp change` to se
+000093b0: 6520 6d6f 7265 2069 6e66 6f2e 7a40 2020  e more info.z@  
+000093c0: 2020 3e20 4e6f 2070 686f 6e65 206e 756d    > No phone num
+000093d0: 6265 7220 666f 756e 6421 2054 7970 6520  ber found! Type 
+000093e0: 6068 656c 7020 6e75 6d62 6572 6020 746f  `help number` to
+000093f0: 2073 6565 206d 6f72 6520 696e 666f 7a31   see more infoz1
+00009400: 2020 2020 5b2b 5d20 5065 7266 6f72 6d69      [+] Performi
+00009410: 6e67 2072 6576 6572 7365 2070 686f 6e65  ng reverse phone
+00009420: 206e 756d 6265 7220 6c6f 6f6b 7570 2e2e   number lookup..
+00009430: 2e7a 3a20 2020 203e 204e 6f20 6970 2061  .z:    > No ip a
+00009440: 6464 7265 7373 2066 6f75 6e64 2120 5479  ddress found! Ty
+00009450: 7065 2060 6865 6c70 2069 7060 2074 6f20  pe `help ip` to 
+00009460: 7365 6520 6d6f 7265 2069 6e66 6f7a 2f20  see more infoz/ 
+00009470: 2020 205b 2b5d 2050 6572 666f 726d 696e     [+] Performin
+00009480: 6720 7265 7665 7273 6520 6970 2061 6464  g reverse ip add
+00009490: 7265 7373 206c 6f6f 6b75 702e 2e2e 7a3c  ress lookup...z<
+000094a0: 2020 2020 3e20 4e6f 206d 6163 2061 6464      > No mac add
+000094b0: 7265 7373 2066 6f75 6e64 2120 5479 7065  ress found! Type
+000094c0: 2060 6865 6c70 206d 6163 6020 746f 2073   `help mac` to s
+000094d0: 6565 206d 6f72 6520 696e 666f 7a30 2020  ee more infoz0  
+000094e0: 2020 5b2b 5d20 5065 7266 6f72 6d69 6e67    [+] Performing
+000094f0: 2072 6576 6572 7365 206d 6163 2061 6464   reverse mac add
+00009500: 7265 7373 206c 6f6f 6b75 702e 2e2e 7a39  ress lookup...z9
+00009510: 2020 2020 3e20 4e6f 2064 6f6d 6169 6e20      > No domain 
+00009520: 666f 756e 6421 2054 7970 6520 6068 656c  found! Type `hel
+00009530: 7020 7768 6f69 7360 2074 6f20 7365 6520  p whois` to see 
+00009540: 6d6f 7265 2069 6e66 6f7a 2b20 2020 205b  more infoz+    [
+00009550: 2b5d 2050 6572 666f 726d 696e 6720 7265  +] Performing re
+00009560: 7665 7273 6520 646f 6d61 696e 206c 6f6f  verse domain loo
+00009570: 6b75 702e 2e2e 7a37 2020 2020 3e20 4e6f  kup...z7    > No
+00009580: 2064 6f6d 6169 6e20 666f 756e 6421 2054   domain found! T
+00009590: 7970 6520 6068 656c 7020 646e 7360 2074  ype `help dns` t
+000095a0: 6f20 7365 6520 6d6f 7265 2069 6e66 6f7a  o see more infoz
+000095b0: 2020 2020 205b 2b5d 2050 6572 666f 726d       [+] Perform
+000095c0: 696e 6720 646e 7320 6c6f 6f6b 7570 2e2e  ing dns lookup..
+000095d0: 2e29 2dda 0b73 696c 656e 745f 6d6f 6465  .)-..silent_mode
+000095e0: 723e 0000 0072 1800 0000 7219 0000 0072  r>...r....r....r
+000095f0: 4200 0000 72a2 0000 00da 0867 6574 6c6f  B...r......getlo
+00009600: 6769 6e72 4600 0000 7247 0000 0072 b300  ginrF...rG...r..
+00009610: 0000 da08 6e6f 6465 6e61 6d65 da07 7379  ....nodename..sy
+00009620: 736e 616d 65da 0670 7375 7469 6c5a 0e76  sname..psutilZ.v
+00009630: 6972 7475 616c 5f6d 656d 6f72 79da 0770  irtual_memory..p
+00009640: 6572 6365 6e74 5a0b 6370 755f 7065 7263  ercentZ.cpu_perc
+00009650: 656e 74da 0a64 6973 6b5f 7573 6167 65da  ent..disk_usage.
+00009660: 046a 6f69 6e72 3f00 0000 da07 6669 6e64  .joinr?.....find
+00009670: 616c 6cda 0475 7569 645a 0767 6574 6e6f  all..uuidZ.getno
+00009680: 6465 da07 6d61 6368 696e 65da 0872 6561  de..machine..rea
+00009690: 646c 696e 65da 0e70 6172 7365 5f61 6e64  dline..parse_and
+000096a0: 5f62 696e 645a 0d73 6574 5f63 6f6d 706c  _bindZ.set_compl
+000096b0: 6574 6572 72d7 0000 0072 4400 0000 723d  eterr....rD...r=
+000096c0: 0000 0072 4800 0000 da11 4b65 7962 6f61  ...rH.....Keyboa
+000096d0: 7264 496e 7465 7272 7570 7472 c400 0000  rdInterruptr....
+000096e0: 7216 0000 0072 1700 0000 727f 0000 0072  r....r....r....r
+000096f0: a600 0000 72cb 0000 0072 cc00 0000 72be  ....r....r....r.
+00009700: 0000 0072 b400 0000 724f 0000 0072 8400  ...r....rO...r..
+00009710: 0000 728d 0000 0072 9900 0000 729d 0000  ..r....r....r...
+00009720: 0029 2672 0900 0000 5a07 6372 745f 6578  .)&r....Z.crt_ex
+00009730: 705a 0865 7870 5f69 6e66 6fda 0475 7365  pZ.exp_info..use
+00009740: 72da 0868 6f73 746e 616d 6572 ba00 0000  r..hostnamer....
+00009750: 5a03 7261 6d5a 0363 7075 5a04 6469 736b  Z.ramZ.cpuZ.disk
+00009760: 5a07 7379 735f 6d61 63da 0461 7263 68da  Z.sys_mac..arch.
+00009770: 0376 6572 5a07 7379 7369 6e66 6f72 0a00  .verZ.sysinfor..
+00009780: 0000 5a04 7469 7073 72b7 0000 005a 0963  ..Z.tipsr....Z.c
+00009790: 6d64 5f63 6f6c 6f72 5a09 6372 745f 636f  md_colorZ.crt_co
+000097a0: 6c6f 72da 0363 6d64 5a03 7469 705a 0968  lor..cmdZ.tipZ.h
+000097b0: 656c 705f 6865 6c70 5a09 6578 6974 5f68  elp_helpZ.exit_h
+000097c0: 656c 705a 0964 6f72 6b5f 6865 6c70 5a08  elpZ.dork_helpZ.
+000097d0: 6578 705f 6865 6c70 5a0a 6368 6563 6b5f  exp_helpZ.check_
+000097e0: 6865 6c70 5a0a 636c 6561 725f 6865 6c70  helpZ.clear_help
+000097f0: 5a09 7361 7665 5f68 656c 705a 0a73 6865  Z.save_helpZ.she
+00009800: 6c6c 5f68 656c 705a 0969 6e66 6f5f 6865  ll_helpZ.info_he
+00009810: 6c70 5a0b 6368 616e 6765 5f68 656c 705a  lpZ.change_helpZ
+00009820: 0b6e 756d 6265 725f 6865 6c70 5a0a 7768  .number_helpZ.wh
+00009830: 6f69 735f 6865 6c70 5a08 646e 735f 6865  ois_helpZ.dns_he
+00009840: 6c70 5a07 6970 5f68 656c 705a 086d 6163  lpZ.ip_helpZ.mac
+00009850: 5f68 656c 705a 0970 7562 6c69 635f 6970  _helpZ.public_ip
+00009860: 5a08 6578 6563 5f63 6d64 da06 6f75 7470  Z.exec_cmd..outp
+00009870: 7574 721b 0000 0072 1b00 0000 721c 0000  utr....r....r...
+00009880: 00da 0e63 6f6e 7472 6f6c 5f63 656e 7465  ...control_cente
+00009890: 725f 0300 0073 2a02 0000 0005 2609 0807  r_...s*.....&...
+000098a0: 0802 040f 3001 3401 3401 3801 3401 3c01  ....0.4.4.8.4.<.
+000098b0: 5401 3402 1c02 0204 02fc 0405 02fb 0406  T.4.............
+000098c0: 02fa 0407 02f9 0408 02f8 040a 02f6 040b  ................
+000098d0: 02f5 040c 02f4 0413 02ed 081a 041f 0808  ................
+000098e0: 0405 0a01 0a03 0801 0805 2802 0a01 0801  ..........(.....
+000098f0: 0401 0801 0a01 1401 1201 1201 0c01 0a01  ................
+00009900: 0801 0405 0c01 1401 0801 0404 0c01 0a01  ................
+00009910: 0801 0404 0c01 0a01 0801 0404 0c01 0a01  ................
+00009920: 0801 0404 0c01 0a01 0801 0404 0c01 0a01  ................
+00009930: 0801 0405 0c01 1201 0801 0405 0a01 0a01  ................
+00009940: 0801 0404 0a01 0a01 0801 0408 0a01 0a01  ................
+00009950: 0801 0405 0a01 0a01 0801 0405 0a01 0a01  ................
+00009960: 0801 0405 0a01 0a01 0801 0405 0a01 0a01  ................
+00009970: 0801 0405 0a02 0801 1202 0801 1001 0803  ................
+00009980: 1401 2202 0801 0a01 0801 0401 1201 1a01  ..".............
+00009990: 0a01 0801 0401 0c01 0a01 1201 0201 0a01  ................
+000099a0: 1001 0201 1601 0601 0201 1001 0601 0201  ................
+000099b0: 1001 0601 1601 0601 1601 0c01 0601 1001  ................
+000099c0: 1001 0e01 0801 0a01 0801 0401 1e01 0a01  ................
+000099d0: 1201 0a01 1001 0a02 0a01 0a02 0801 0801  ................
+000099e0: 0a01 0801 0401 1401 1201 1201 0c01 1001  ................
+000099f0: 0802 0a01 0a01 1201 0a02 1201 0a02 0801  ................
+00009a00: 1001 0801 0a01 0801 0401 0c01 0a01 0801  ................
+00009a10: 0401 1401 1201 1201 0c01 0a01 0801 0801  ................
+00009a20: 1201 0a01 0801 0801 1202 0801 1202 0801  ................
+00009a30: 1001 0803 0a01 0801 1401 1201 0401 1201  ................
+00009a40: 0c01 1201 0a01 0a02 0801 0602 0801 1401  ................
+00009a50: 0a01 0801 1401 1201 0401 1201 0c01 1201  ................
+00009a60: 0a01 0a02 0801 0602 0801 1401 0a01 0801  ................
+00009a70: 1401 1201 0401 1201 0c01 1201 0a01 0a02  ................
+00009a80: 0801 0602 0801 1401 0a01 0801 1401 1201  ................
+00009a90: 0401 1201 0c01 1201 0a01 0a02 0801 0602  ................
+00009aa0: 0801 1201 0a01 0801 1201 1201 0401 1201  ................
+00009ab0: 0c01 1201 0a01 0a02 0801 0602 0801 1204  ................
+00009ac0: 0801 1003 72fa 0000 0063 0000 0000 0000  ....r....c......
+00009ad0: 0000 0000 0000 0000 0000 0b00 0000 4300  ..............C.
+00009ae0: 0000 73a0 0000 007a 2474 006a 0164 0119  ..s....z$t.j.d..
+00009af0: 0064 026b 0273 1e74 006a 0164 0119 0064  .d.k.s.t.j.d...d
+00009b00: 036b 0272 2264 0461 0257 006e 1204 0074  .k.r"d.a.W.n...t
+00009b10: 0379 3601 0001 0001 0059 006e 0230 0074  .y6......Y.n.0.t
+00009b20: 0273 4274 0483 0001 007a 0a74 0583 0001  .sBt.....z.t....
+00009b30: 0057 006e 4e04 0074 0679 9a01 0001 0001  .W.nN..t.y......
+00009b40: 0074 0783 0001 0074 0273 9074 0864 0564  .t.....t.s.t.d.d
+00009b50: 0164 0674 09a0 0a64 0764 0867 02a1 0167  .d.t...d.d.g...g
+00009b60: 0364 0464 0464 0464 0464 098d 0601 0074  .d.d.d.d.d.....t
+00009b70: 0b83 0001 006e 0674 0783 0001 0059 006e  .....n.t.....Y.n
+00009b80: 0230 0064 0053 0029 0a4e 7224 0000 007a  .0.d.S.).Nr$...z
+00009b90: 022d 737a 082d 2d73 696c 656e 7454 7a26  .-sz.--silentTz&
+00009ba0: 5b23 5d20 5465 726d 696e 6174 696e 6720  [#] Terminating 
+00009bb0: 6050 4830 4d42 4552 6020 6672 616d 6577  `PH0MBER` framew
+00009bc0: 6f72 6b2e 2e2e 7225 0000 0072 2d00 0000  ork...r%...r-...
+00009bd0: 7226 0000 0029 0572 2800 0000 7229 0000  r&...).r(...r)..
+00009be0: 0072 a900 0000 72a8 0000 0072 aa00 0000  .r....r....r....
+00009bf0: 290c da03 7379 73da 0461 7267 7672 e600  )...sys..argvr..
+00009c00: 0000 da0a 496e 6465 7845 7272 6f72 72cd  ....IndexErrorr.
+00009c10: 0000 0072 fa00 0000 72f3 0000 0072 4800  ...r....r....rH.
+00009c20: 0000 723e 0000 0072 1800 0000 7219 0000  ..r>...r....r...
+00009c30: 0072 0800 0000 721b 0000 0072 1b00 0000  .r....r....r....
+00009c40: 721b 0000 0072 1c00 0000 da04 6d61 696e  r....r......main
+00009c50: 2605 0000 731c 0000 0000 0502 011c 0108  &...s...........
+00009c60: 010c 0106 030a 0302 010a 010c 0106 0104  ................
+00009c70: 0124 0108 0172 fe00 0000 2923 7216 0000  .$...r....)#r...
+00009c80: 0072 a200 0000 72fb 0000 0072 1800 0000  .r....r....r....
+00009c90: 72b0 0000 0072 f100 0000 723f 0000 0072  r....r....r?...r
+00009ca0: ef00 0000 729a 0000 0072 ea00 0000 72c2  ....r....r....r.
+00009cb0: 0000 0072 3c00 0000 5a11 6d61 635f 7665  ...r<...Z.mac_ve
+00009cc0: 6e64 6f72 5f6c 6f6f 6b75 7072 0200 0000  ndor_lookupr....
+00009cd0: 7212 0000 005a 0c64 6e73 2e72 6573 6f6c  r....Z.dns.resol
+00009ce0: 7665 7272 0700 0000 72d3 0000 00da 0865  verr....r......e
+00009cf0: 6c65 6d65 6e74 7372 3d00 0000 72b4 0000  lementsr=...r...
+00009d00: 0072 e600 0000 721d 0000 0072 4f00 0000  .r....r....rO...
+00009d10: 7284 0000 0072 8d00 0000 7299 0000 0072  r....r....r....r
+00009d20: 9d00 0000 723e 0000 0072 be00 0000 72c4  ....r>...r....r.
+00009d30: 0000 0072 cd00 0000 72d7 0000 0072 fa00  ...r....r....r..
+00009d40: 0000 72fe 0000 0072 1b00 0000 721b 0000  ..r....r....r...
+00009d50: 0072 1b00 0000 721c 0000 00da 083c 6d6f  .r....r......<mo
+00009d60: 6475 6c65 3e20 0000 0073 4a00 0000 0801  dule> ...sJ.....
+00009d70: 0801 0801 0801 0801 0801 0801 0801 0801  ................
+00009d80: 0801 0801 0801 0c01 0801 0804 0c01 0401  ................
+00009d90: 0401 0405 080a 087f 000e 087f 007f 0066  ...............f
+00009da0: 082c 084b 0838 2420 082b 081c 080a 080a  .,.K.8$ .+......
+00009db0: 087f 007f 007f 004a                      .......J
```

## Comparing `phomber/phomberv3_beta.py` & `phomber/phomberv3.0.2_beta.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 #!/usr/bin/python3
 
 #==============================================================================#
 #                                                                              #
-# [prog]   : Ph0mber                                                           #
-# [ver]    : 3.0 beta                                                          #
-# [desc]   : Multi-porpose osint framework for gathering information           #
+# [prog]   : PH0MBER                                                           #
+# [ver]    : 3.0.2 beta                                                        #
+# [desc]   : An open source infomation grathering & reconnaissance framework!  #
 # [dev]    : @s41r4j                                                           #
-# [github] : https://github.com/s41r4j/phomber                                 #
 # [license]: GNU GPLv3                                                         #
+# [github] : https://github.com/s41r4j/phomber                                 #
+# [pypi]   : https://pypi.org/project/phomber/                                 #
 #                                                                              #
 #==============================================================================#
 
 #==============================================================================#
 #                                                                              #
 #   [!] Legal/Ethical disclaimer:                                              #
 #                                                                              #
@@ -31,31 +32,38 @@
 import requests      # Default
 import os            # Default
 import sys           # Default
 import random        # Default
 import time          # Default
 import readline      # Default
 import re            # Default
+import uuid          # Default
+import socket        # Default
 import psutil        # pip install psutil
 import bs4           # pip install beautifulsoup4
 import phonenumbers  # pip install phonenumbers
+from mac_vendor_lookup import MacLookup # pip install mac-vendor-lookup
+import whois         # pip install python-whois
+import dns.resolver  # pip install dnspython
 
 
 # ------------------------ Global variables ------------------------ #
-avaliable_commands = ['help', 'exit', 'quit', 'dork', 'exp', 'check', 'clear', 'save', 'shell', 'info', 'change', 'number', 'ip']
+avaliable_commands = elements = ['change', 'check', 'clear', 'dork', 'dns', 'exit', 'exp', 'help', 'info', 'ip', 'mac', 'number', 'quit', 'save', 'shell', 'whois']
 prv_op = ''
+full_cmd = ''
 silent_mode = False
 
-
 # ------------------------ Scanner functions ------------------------ #
+
 # Check internet connection
-def check_connection(url):
+def check_connection():
     # Checking internet connection
+    urls = ['https://google.com', 'https://bing.com']
     try:
-        requests.get(url, timeout=10)
+        requests.get(random.choice(urls), timeout=10)
         return True
     except:
         return False
 
 # Reverse phone number lookup
 def number_lookup(phone_number):
     # Importing modules
@@ -65,29 +73,27 @@
     
     # Global variables
     global prv_op
     prv_op = '' # Resetting previous output
 
     # Information gathering about the number
     printit(f'    [+] Grathering information about \33[1;49;96m{phone_number}\33[1;49;93m...', coledt=[1, 49, 93], space_down=True)
-    prv_op += f'\n    \33[1;49;93m[#] Reverse phone number lookup for \33[1;49;96m{phone_number}\33[1;49;93m:\033[0m'+'\n'
+    prv_op += f'\n    \33[1;49;93m[#] Reverse phone number lookup for \33[1;49;96m{phone_number}\33[1;49;93m:\033[0m'+'\n\n'
 
     # Check if the number is valid or not (regex)
     if not re.match(r'^\+[1-9]\d{1,14}$', phone_number):
         printit('    > Invalid phone number format! (Example: +44xxxxxxxxxx)', coledt=[1, 49, 91])
-        prv_op += '    > Invalid phone number format! (Example: +44xxxxxxxxxx)'+'\n'
         return False
     
     # Country code check
     try:
         # Phone number format: (+Countrycode)xxxxxxxxxx
         phone_number_details = phonenumbers.parse(phone_number)
     except phonenumbers.phonenumberutil.NumberParseException:
         printit('    > Missing Country Code! (Example: +91, +44, +1)', coledt=[1, 49, 91])
-        prv_op += '    > Missing Country Code! (Example: +91, +44, +1)'+'\n'
         return False
 
     # extract country_code & only_number from "Country Code: xx National Number: xxxxxxxxxx"
     country_code = str(phone_number_details).split('Country Code:', 1)[1].split('National Number:', 1)[0].strip()
     only_number = str(phone_number_details).split('Country Code:', 1)[1].split('National Number:', 1)[1].strip()
     
     # Validating a phone number
@@ -130,14 +136,16 @@
         phone_number = str(phone_number)+' '*int(30-len(str(phone_number)))
         only_number = str(only_number)+' '*int(30-len(str(only_number)))
         r_format = str(r_format)+' '*int(30-len(str(r_format)))
         
         # Printing information
         final_output = f'''
     ┌──────────────────────────────────────────────────────┐
+    | Scanned Phone Number: \33[1;49;96m{phone_number}\033[0m |
+    |------------------------------------------------------|
     | INFORMATION         | DESCRIPTION                    |
     |------------------------------------------------------|
     | \33[1;49;97mPossible\033[0m            | {possible} |
     | \33[1;49;97mValid\033[0m               | {valid} |
     |------------------------------------------------------|
     | \33[1;49;97mCountry Code\033[0m        | {country_code} |
     | \33[1;49;97mCountry\033[0m             | {country} |
@@ -168,23 +176,29 @@
     \33[1;49;93m[+] Google Dork Queries:
 
     \33[1;49;92m> https://www.google.com/search?q={only_number.strip()}
     \033[0m'''
         print(google_dork_queries)
         prv_op += google_dork_queries+'\n'
 
+        # Scanning social media platforms
+        printit(f'    [+] Scanning social media platforms:', coledt=[1, 49, 93], space_down=True)
+
         return True
         
     else:
         # Reconfiguring variables
         possible = str(possible)+' '*int(30-len(str(possible)))
         valid = str(valid)+' '*int(30-len(str(valid)))
+        phone_number = str(phone_number)+' '*int(30-len(str(phone_number)))
 
         final_output = f'''
     ┌──────────────────────────────────────────────────────┐
+    | Scanned Phone Number: \33[1;49;96m{phone_number}\033[0m |
+    |------------------------------------------------------|
     | INFORMATION         | DESCRIPTION                    |
     |------------------------------------------------------|
     | \33[1;49;97mPossible\033[0m            | {possible} |
     | \33[1;49;97mValid\033[0m               | {valid} |
     └──────────────────────────────────────────────────────┘
         '''
         print(final_output)
@@ -195,28 +209,26 @@
 def ip_lookup(ip_address):
     # Global variables
     global prv_op
     prv_op = '' # Resetting previous output
     
     # Checking internet connection
     printit(f'    [+] Verifying internet connection...', coledt=[1, 49, 93], space_down=True)
-    if not check_connection('https://www.google.com'):
+    if not check_connection():
         printit('    > Internet connection not available!', coledt=[1, 49, 91], space_down=True)
-        prv_op += '\n    \33[1;49;91m> Internet connection not available!\033[0m'+'\n'
         return False
 
     # Information gathering about the ip address
     printit(f'    [+] Grathering information about \33[1;49;96m{ip_address}\33[1;49;93m...', coledt=[1, 49, 93], space_down=True)
-    prv_op += f'    \33[1;49;93m[#] Reverse ip address lookup for \33[1;49;96m{ip_address}\33[1;49;93m:\033[0m'+'\n'
+    prv_op += f'    \33[1;49;93m[#] Reverse ip address lookup for \33[1;49;96m{ip_address}\33[1;49;93m:\033[0m'+'\n\n'
 
     # Check if the ip address is valid or not (regex) [add IPv6 support]
     if not re.match(r'^\d{1,3}\.\d{1,3}\.\d{1,3}\.\d{1,3}$', ip_address) :
         printit('    > Invalid ip address format! (Example: 8.8.8.8)', coledt=[1, 49, 91])
-        prv_op += '   \33[1;49;91m> Invalid ip address format! (Example: 8.8.8.8)\033[0m'+'\n'
-        return 
+        return False
 
     # IP address lookup APIs
     ip_addresses = [f'http://ip-api.com/json/{ip_address}', f'https://ipapi.co/{ip_address}/json/', f'http://ipwho.is/{ip_address}']
     ip_address = str(ip_address)+' '*int(30-len(str(ip_address)))
 
     # Headers
     headers = {
@@ -264,15 +276,14 @@
             longitude = str(longitude)+' '*int(30-len(str(longitude)))
             ip = str(ip)+' '*int(30-len(str(ip)))
             
             # Printing information
             final_output = f'''
     ┌──────────────────────────────────────────────────────┐
     | Scanned IP Address: \33[1;49;96m{ip_address}\033[0m   |
-    | Server code name  : \33[1;49;96mreverse-ip-lookup-server-1\033[0m       |
     |------------------------------------------------------|
     | INFORMATION         | DESCRIPTION                    |
     |------------------------------------------------------|
     | \33[1;49;97mCountry\033[0m             | {country} |
     | \33[1;49;97mCountry Code\033[0m        | {countryCode} |
     | \33[1;49;97mRegion\033[0m              | {region} |
     | \33[1;49;97mRegion Code\033[0m         | {regionCode} |
@@ -291,15 +302,14 @@
             prv_op += final_output+'\n'
 
         except Exception as e:
             print(e)
             final_output = f'''
     ┌──────────────────────────────────────────────────────┐
     | Scanned IP Address: \33[1;49;96m{ip_address}\033[0m   |
-    | Server code name  : \33[1;49;96mreverse-ip-lookup-server-1\033[0m       |
     |------------------------------------------------------|
     | \33[1;49;91mFailed to Fetch information from this server!\033[0m        |
     └──────────────────────────────────────────────────────┘
     '''
             print(final_output)
             prv_op += final_output+'\n'
 
@@ -371,15 +381,14 @@
             asn = str(asn)+' '*int(30-len(str(asn)))
             org = str(org)+' '*int(30-len(str(org)))
             
             # Printing information
             final_output = f'''
     ┌──────────────────────────────────────────────────────┐
     | Scanned IP Address: \33[1;49;96m{ip_address}\033[0m   |
-    | Server code name  : \33[1;49;96mreverse-ip-lookup-server-2\033[0m       |
     |------------------------------------------------------|
     | INFORMATION         | DESCRIPTION                    |
     |------------------------------------------------------|
     | \33[1;49;97mIP Type\033[0m             | {version} |
     | \33[1;49;97mNetwork\033[0m             | {network} |
     |------------------------------------------------------|
     | \33[1;49;97mCountry\033[0m             | {country} |
@@ -414,15 +423,14 @@
             print(final_output)
             prv_op += final_output+'\n'
 
         except:
             final_output = f'''
     ┌──────────────────────────────────────────────────────┐
     | Scanned IP Address: \33[1;49;96m{ip_address}\033[0m   |
-    | Server code name  : \33[1;49;96mreverse-ip-lookup-server-2\033[0m       |
     |------------------------------------------------------|
     | \33[1;49;91mFailed to Fetch information from this server!\033[0m        |
     └──────────────────────────────────────────────────────┘
     '''
             print(final_output)
             prv_op += final_output+'\n'
 
@@ -498,15 +506,14 @@
             timezone_utc = str(timezone_utc)+' '*int(30-len(str(timezone_utc)))
             timezone_current_time = str(timezone_current_time)+' '*int(30-len(str(timezone_current_time)))
                     
             # Printing information
             final_output = f'''
     ┌──────────────────────────────────────────────────────┐
     | Scanned IP Address: \33[1;49;96m{ip_address}\033[0m   |
-    | Server code name  : \33[1;49;96mreverse-ip-lookup-server-3\033[0m       |
     |------------------------------------------------------|
     | INFORMATION         | DESCRIPTION                    |
     |------------------------------------------------------|
     | \33[1;49;97mIP Type\033[0m             | {ip_type} |
     |------------------------------------------------------|
     | \33[1;49;97mCountry\033[0m             | {country} |
     | \33[1;49;97mCountry Code\033[0m        | {country_code} |
@@ -541,24 +548,196 @@
             print(final_output)
             prv_op += final_output+'\n'
 
         except:
             final_output = f'''
     ┌──────────────────────────────────────────────────────┐
     | Scanned IP Address: \33[1;49;96m{ip_address}\033[0m   |
-    | Server code name  : \33[1;49;96mreverse-ip-lookup-server-3\033[0m       |
     |------------------------------------------------------|
     | \33[1;49;91mFailed to Fetch information from this server!\033[0m        |
     └──────────────────────────────────────────────────────┘
     '''
             print(final_output)
             prv_op += final_output+'\n'
 
     return True
 
+# Reverse mac address lookup
+def mac_lookup(mac_address):
+    # https://api.macvendors.com/<mac_address>
+    
+    # Global variables
+    global prv_op
+    prv_op = '' # Resetting previous output
+
+    # Information gathering about the mac address
+    printit(f'    [+] Grathering information about \33[1;49;96m{mac_address}\33[1;49;93m...', coledt=[1, 49, 93], space_down=True)
+    prv_op += f'    \33[1;49;93m[#] Reverse mac address lookup for \33[1;49;96m{mac_address}\33[1;49;93m:\033[0m'+'\n\n'
+
+    # Check if the mac address is valid or not (regex)
+    if not re.match(r'^([0-9A-Fa-f]{2}[:-]){5}([0-9A-Fa-f]{2})$', mac_address) :
+        printit('    > Invalid mac address format! (Example: 00:00:00:00:00:00)', coledt=[1, 49, 91])
+        return False
+
+    # Getting mac address vendor
+    try:
+        vendor = MacLookup().lookup(mac_address)
+        bol_val = True
+    except KeyError:
+        vendor = '\33[1;49;91mNot Found\033[0m'
+        bol_val = False
+
+    # Reconfiguring variables
+    mac_address = str(mac_address)+' '*int(31-len(str(mac_address)))
+    vendor = str(vendor)+' '*int(36-len(str(vendor)))
+
+    # Printing information
+    final_output = f'''
+    ┌──────────────────────────────────────────────────────┐
+    | Scanned MAC Address: \33[1;49;96m{mac_address}\033[0m |
+    |------------------------------------------------------|
+    | INFORMATION   | DESCRIPTION                          |
+    |------------------------------------------------------|
+    | \33[1;49;97mVendor\033[0m        | {vendor} |
+    └──────────────────────────────────────────────────────┘
+    '''
+    print(final_output)
+    prv_op += final_output+'\n'
+
+    return bol_val
+
+# Reverse whois lookup
+def whois_lookup(domain):
+    # Global variables
+    global prv_op
+    prv_op = '' # Resetting previous output
+
+    # Checking internet connection
+    printit(f'    [+] Verifying internet connection...', coledt=[1, 49, 93], space_down=True)
+    if not check_connection():
+        printit('    > Internet connection not available!', coledt=[1, 49, 91], space_down=True)
+        return False
+
+    # Information gathering about the domain
+    printit(f'    [+] Grathering information about \33[1;49;96m{domain}\33[1;49;93m...', coledt=[1, 49, 93], space_down=True)
+    prv_op += f'    \33[1;49;93m[#] Reverse whois lookup for \33[1;49;96m{domain}\33[1;49;93m:\033[0m'+'\n\n'
+
+    # Domain validation (regex)
+    if not re.match(r'^([a-zA-Z0-9]+(-[a-zA-Z0-9]+)*\.)+[a-zA-Z]{2,}$', domain) :
+        printit('    > Invalid domain format! (Example: example.com)', coledt=[1, 49, 91])
+        return False
+
+    # Getting whois information
+    try:
+        whois_info = whois.whois(domain)
+        bol_val = True
+    except:
+        bol_val = False
+
+    # Reconfiguring variables
+    domain = str(domain)+' '*int(36-len(str(domain)))
+
+    # Printing information
+    final_output = f'''
+    ┌──────────────────────────────────────────────────────┐
+    | Scanned Domain: \33[1;49;96m{domain}\033[0m |
+    |------------------------------------------------------|
+    | INFORMATION   | DESCRIPTION                          |
+    |------------------------------------------------------|'''
+
+    # If whois information is available
+    if bol_val:
+        # Loop through whois information & add it to the final output
+        for key, value in whois_info.items():
+            # Filtering out some keys
+            if key == 'status': continue
+            if key == 'expiration_date': key = 'expiry_date'
+            if key == 'registrant_postal_code': key = 'postal_code'
+
+            # Reconfiguring variables
+            key = key.replace('_', ' ').capitalize()
+
+            # Adding formatted information to the final output
+            if type(value) == list:
+                key = str(key)+' '*int(13-len(str(key)))
+                value_1 = str(value[0])+' '*int(36-len(str(value[0])))
+                final_output += f'''\n    | \33[1;49;97m{key}\033[0m | {value_1} |'''
+                if len(value) > 1:
+                    for i in range(1, len(value)):
+                        value_2 = str(value[i])+' '*int(36-len(str(value[i])))
+                        final_output += f'''\n    |               | {value_2} |'''
+            else:
+                key = str(key)+' '*int(13-len(str(key)))
+                value = str(value)+' '*int(36-len(str(value)))
+                final_output += f'''\n    | \33[1;49;97m{key}\033[0m | {value} |'''            
+    else:
+        final_output += f'''\n    | \33[1;49;97mInformation\033[0m   | \33[1;49;91mNot Found\033[0m{' '*int(36-len('Not Found'))} |'''
+
+    # Add the last part of the final output
+    final_output += f'''\n    └──────────────────────────────────────────────────────┘'''
+
+    print(final_output)
+    prv_op += final_output+'\n'
+
+    return bol_val
+
+# Reverse domain lookup
+def dns_lookup(ip_or_domain):
+    # Global variables
+    global prv_op
+    prv_op = '' # Resetting previous output
+
+    # Checking internet connection
+    printit(f'    [+] Verifying internet connection...', coledt=[1, 49, 93], space_down=True)
+    if not check_connection():
+        printit('    > Internet connection not available!', coledt=[1, 49, 91], space_down=True)
+        return False
+
+    # Information gathering about the domain    
+    printit(f'    [+] Grathering information about \33[1;49;96m{ip_or_domain}\33[1;49;93m...', coledt=[1, 49, 93], space_down=True)
+
+    # Validating ip address or domain name (regex)
+    if re.match(r'^([a-zA-Z0-9]+(-[a-zA-Z0-9]+)*\.)+[a-zA-Z]{2,}$', ip_or_domain):
+        prv_op += f'    \33[1;49;93m[#] DNS lookup for \33[1;49;96m{ip_or_domain}\33[1;49;93m:\033[0m'+'\n\n'
+        domain = ip_or_domain + ' '*int(36-len(ip_or_domain))
+        final_output_scanned = f'    | Scanned Domain: \33[1;49;96m{domain}\033[0m |'
+        try:
+            ip = socket.gethostbyname(ip_or_domain)
+            ip = str(ip)+' '*int(36-len(str(ip)))
+        except:
+            ip = '\33[1;49;91mNot Found\033[0m' + ' '*int(36-len('Not Found'))
+    elif re.match(r'^([0-9]{1,3}\.){3}[0-9]{1,3}$', ip_or_domain):
+        prv_op += f'    \33[1;49;93m[#] Reverse DNS lookup for \33[1;49;96m{ip_or_domain}\33[1;49;93m:\033[0m'+'\n\n'
+        ip = ip_or_domain + ' '*int(36-len(ip_or_domain))
+        final_output_scanned = f'    | Scanned IP: \33[1;49;96m{ip}\033[0m     |'
+        try:
+            domain = socket.gethostbyaddr(ip_or_domain)[0]
+            domain = str(domain)+' '*int(36-len(str(domain)))
+        except:
+            domain = '\33[1;49;91mNot Found\033[0m' + ' '*int(36-len('Not Found'))
+    else:
+        printit('    > Invalid ip address or domain name!', coledt=[1, 49, 91], space_down=True)
+        return False
+
+    # Expcepts: socket.gaierror, socket.herror
+
+    # Printing information
+    final_output_remaining = f'''
+    |------------------------------------------------------|
+    | INFORMATION   | DESCRIPTION                          |
+    |------------------------------------------------------|
+    | \33[1;49;97mIP\033[0m            | {ip} |
+    | \33[1;49;97mDomain\033[0m        | {domain} |
+    └──────────────────────────────────────────────────────┘
+    '''
+
+    print('\n    ┌──────────────────────────────────────────────────────┐\n'+final_output_scanned+final_output_remaining)
+    prv_op += '\n    ┌──────────────────────────────────────────────────────┐'+'\n'+final_output_scanned+final_output_remaining
+
+    return True
 
 # --------------------------- Basic functions ------------------------ #
 
 def printit(text, center='', line_up=False, line_down=False, space_up=False, space_down=False, coledt=[0, 0, 0], normaltxt_start='', normaltxt_end='', hide=False, verbose_mode=False, input_mode=False):
     if not hide or verbose_mode:
         # get terminal width
         width = os.get_terminal_size().columns
@@ -573,46 +752,63 @@
             new_width = int((width - len(text))/2)
             print(center*new_width, end='')
             print(f'\33[{coledt[0]};{coledt[1]};{coledt[2]}m', end='')
             if input_mode: input_var = input(text)
             else: print(str(text), end='')
             print('\033[0m', end='')
             print(center*new_width)
+        else:
+            print(f'\33[{coledt[0]};{coledt[1]};{coledt[2]}m', end='')
+            if input_mode: input_var = input(text)
+            else: print(str(text), end='')
+            print('\033[0m', end='')
 
         print(normaltxt_end, end='')
 
         if line_down: print('⸺'*width)
         if space_down: print()
 
         if input_mode: return input_var
 
 def save_output(prv_cmd):
     try:
-        filename = prv_cmd+'_'+str(time.strftime("%d-%m-%Y_%H-%M-%S"))+'.txt'
+        filename = prv_cmd+'_ph0mber_'+str(time.strftime("%d-%m-%Y_%H-%M-%S"))+'.txt'
         pwd = os.getcwd()
         os_name = os.uname()
         path = pwd+'/'+filename
 
         file_save_info = f'''
     \33[1;49;93m[#] Output File Name: \33[1;49;97m{filename}\033[0m
     \33[1;49;93m[#] Output File Path: \33[1;49;97m{path}\033[0m
         '''
         print(file_save_info)
+    
+        header = f'''
+    \33[1;49;93m[@] Osint framework: \33[1;49;96mPH0MBER
+    \33[1;49;93m[@] Github: \33[1;49;96mhttps://github.com/s41r4j/phomber
+
+    \33[1;49;93m[#] Output File Name: \33[1;49;97m{filename}
+    \33[1;49;93m[#] Output File Path: \33[1;49;97m{path}
+    \33[1;49;93m[#] Date: \33[1;49;97m{str(time.strftime("%d-%m-%Y"))}
+    \33[1;49;93m[#] Time: \33[1;49;97m{str(time.strftime("%H:%M:%S"))}
+
+    \33[1;49;93m[#] Command Executed: \33[1;49;96m{full_cmd.strip()}\n'''
 
         with open(path, 'w') as f:
+            f.write(header)
             f.write(prv_op)
     
         printit(f'    [+] Excute following commands to view output:', coledt=[1, 49, 93], space_down=True, space_up=True)
         
         if os_name == 'nt':
-            exe_cmd = f'''    \33[1;49;92m> shell more {path}\033[0m
-    \33[1;49;92m> shell type {path}\033[0m'''
+            exe_cmd = f'''    \33[1;49;93m> \33[1;49;92mshell more {filename}\033[0m
+    \33[1;49;93m> \33[1;49;92mshell type {filename}\033[0m'''
         else:
-            exe_cmd = f'''    \33[1;49;92m> shell cat {path}\033[0m
-    \33[1;49;92m> shell less {path}\033[0m'''
+            exe_cmd = f'''    \33[1;49;93m> \33[1;49;92mshell cat {filename}\033[0m
+    \33[1;49;93m> \33[1;49;92mshell less {filename}\033[0m'''
         print(exe_cmd)
 
         return True
     except:
         printit(f'    [!] Output could not be saved!', coledt=[1, 49, 91], space_down=True)
         return False
 
@@ -704,91 +900,107 @@
     # Variables
     user = '\33[1;49;96m'+str(os.getlogin())+'\033[0m'+ ' '*int(34-len(str(os.getlogin())))
     hostname = '\33[1;49;96m'+str(os.uname().nodename)+'\033[0m'+' '*int(34-len(str(os.uname().nodename)))
     os_name = '\33[1;49;96m'+str(os.uname().sysname)+'\033[0m'+' '*int(34-len(str(os.uname().sysname)))
     ram = '\33[1;49;96m'+str(psutil.virtual_memory().percent)+"%"+'\033[0m'+' '*int(33-len(str(psutil.virtual_memory().percent)))
     cpu = '\33[1;49;96m'+str(psutil.cpu_percent())+"%"+'\033[0m'+' '*int(32-len(str(psutil.cpu_percent())))
     disk = '\33[1;49;96m'+str(psutil.disk_usage('/').percent)+"%"+'\033[0m'+' '*int(33-len(str(psutil.disk_usage('/').percent)))
+    sys_mac = '\33[1;49;96m'+str(':'.join(re.findall('..', '%012x' % uuid.getnode())))+'\033[0m'+' '*int(34-len(str(':'.join(re.findall('..', '%012x' % uuid.getnode())))))
+    arch = '\33[1;49;96m'+str(os.uname().machine)+'\033[0m'+' '*int(34-len(str(os.uname().machine)))
 
-    ver = '\33[1;49;96m3.0 beta\033[0m'+' '*int(34-len(str(3.0)))
+    ver = '\33[1;49;96m3.0.2 (beta)\033[0m'+' '*int(34-len(str('3.0.2 (beta)')))
 
     sysinfo = f'''
     ┌────────────────────────────────────────────────────┐
     | SYSTEM INFO   | DESCRIPTION                        |
     |----------------------------------------------------|
     | \33[1;49;97mUser\033[0m          | {user} |
     | \33[1;49;97mHostname\033[0m      | {hostname} |
     | \33[1;49;97mOS\033[0m            | {os_name} |
+    | \33[1;49;97mArchitecture\033[0m  | {arch} |
+    | \33[1;49;97mSystem MAC\033[0m    | {sys_mac} |
+    |----------------------------------------------------|
     | \33[1;49;97mRAM Usage\033[0m     | {ram} |
     | \33[1;49;97mCPU Usage\033[0m     | {cpu} |
     | \33[1;49;97mDisk Usage\033[0m    | {disk} |
     └────────────────────────────────────────────────────┘
 
     ┌────────────────────────────────────────────────────┐
     | FRAMEWORK INFO| DESCRIPTION                        |
     |----------------------------------------------------|
     | \33[1;49;97mName\033[0m          | \33[1;49;96mPH0MBER\033[0m                            |
     | \33[1;49;97mVersion\033[0m       | {ver} |
-    | \33[1;49;97mType\033[0m          | \33[1;49;96mOSINT\033[0m                              |
-    | \33[1;49;97mAuthor\033[0m        | \33[1;49;96ms41r4j\033[0m                             |
+    | \33[1;49;97mType\033[0m          | \33[1;49;96mOSINT Framework\033[0m                    |
+    | \33[1;49;97mDeveloper\033[0m     | \33[1;49;96ms41r4j\033[0m                             |
     | \33[1;49;97mGithub\033[0m        | \33[1;49;96mhttps://github.com/s41r4j/phomber\033[0m  |
     └────────────────────────────────────────────────────┘
     '''
 
     help = '''
     ┌────────────────────────────────────────────────────┐
     | COMMANDS      | DESCRIPTION                        |
     |----------------------------------------------------|
     |                <Basic Commands>                    |
     |----------------------------------------------------|
     | \33[1;49;97mhelp\033[0m          | Display this help menu             | 
     | \33[1;49;97mexit/quit\033[0m     | Exit the framework                 |
-    | \33[1;49;97mdork\033[0m          | Show a random google dork query    |  
+    | \33[1;49;97mdork\033[0m          | Show a random google dork query *  |  
     | \33[1;49;97mexp\033[0m           | Show info about all available      |       
     |               | expressions                        |
     | \33[1;49;97mcheck\033[0m         | Check internet connection          |
     | \33[1;49;97mclear\033[0m         | Clear screen                       |
     | \33[1;49;97msave\033[0m          | Save output of previous scanner    |
     |               | command in a file                  |
     | \33[1;49;97mshell <cmd>\033[0m   | Execute native shell/cmd commands  |
     | \33[1;49;97minfo\033[0m          | Show info about framework & system |
     | \33[1;49;97mchange\033[0m        | Change user command input color    |
     |----------------------------------------------------|
     |                 <Scanner Commands>                 |
     |----------------------------------------------------|
-    | \33[1;49;97mnumber\033[0m        | Reverse phone number lookup        |
-    | \33[1;49;97mip\033[0m            | Reverse ip address lookup          |
+    | \33[1;49;97mnumber\033[0m        | Reverse phone number lookup *      |
+    | \33[1;49;97mip\033[0m            | Reverse ip address lookup *        |
+    | \33[1;49;97mmac\033[0m           | Reverse mac address lookup         |
+    | \33[1;49;97mwhois\033[0m         | Reverse whois lookup *             |
+    | \33[1;49;97mdns\033[0m           | Reverse or normal DNS lookup       |
+    |----------------------------------------------------|
     | \33[1;49;91mMORE SCANNERS COMING SOON, THIS IS A BETA VER\033[0m      |
     └────────────────────────────────────────────────────┘
+    '''
 
-    \33[1;49;93m> Type `help <command>` to see more info about a command\033[0m
-    \33[1;49;93m> Use `Tab` key to auto-complete commands\033[0m
-    \33[1;49;93m> Try silent mode by using `-s`/`--silent` flag\033[0m'''
+    tips = ['Type `\33[7;49;93mhelp <command>\033[0m\33[1;49;93m` to see more info about a command',
+            'Use `\33[7;49;93mTab\033[0m\33[1;49;93m` key to auto-complete commands',
+            'Try silent mode by using `\33[7;49;93m-s\033[0m\33[1;49;93m`/`\33[7;49;93m--silent\033[0m\33[1;49;93m` flag',
+            'You can also use `\33[7;49;93mCtrl+C\033[0m\33[1;49;93m` to exit',
+            'Descriptions ending with `\33[7;49;93m*\033[0m\33[1;49;93m` needs internet connection'
+            ]
 
     # Previous command
     prv_cmd = ''
-    global prv_op
+    global prv_op 
+    global full_cmd
 
     # Setting up auto-complete
     readline.parse_and_bind('tab: complete')
     readline.set_completer(completer)
 
     # Command prompt color
     cmd_color = ['\33[1;49;90m', '\33[1;49;97m']
     crt_color = cmd_color[1]
 
     # Control center loop
     while True:
         # [user@phomber]⸺[:D] $
-        cmd = (printit(f'\n[{user.strip()}@ph0mber]⸺ [{crt_exp}] $ {crt_color}', input_mode=True, space_up=True)).strip()
+        cmd = (printit(f'\n\033[0m[{user.strip()}@ph0mber]⸺ [{crt_exp}] $ {crt_color}', input_mode=True, space_up=True)).strip()
 
         if cmd == 'help':
             crt_exp = exp[1]
             prv_op = ''
             print(help)
+            tip = random.choice(tips)
+            print(f'\33[1;49;93m    > {tip}\033[0m')
         elif cmd[:4] == 'help':
             if (cmd+'#')[4] == ' ':
                 cmd = cmd[5:]
                 if cmd == 'help':
                     crt_exp = exp[1]
                     help_help = '''  \33[1;49;93m[+] Command Info: \33[1;49;93mhelp\n
     \33[1;49;92m> DESCRIPTION: \33[1;49;97mWhen you type `help`, the help menu will be displayed
@@ -864,46 +1076,63 @@
     \33[1;49;92m> SYNTAX: \33[1;49;97mchange <color_code>
     \33[1;49;92m> EXAMPLE: \33[1;49;97mchange 0
     \033[0m'''
                     print(change_help)
                 elif cmd == 'number':
                     crt_exp = exp[1]
                     number_help = '''  \33[1;49;93m[+] Command Info: \33[1;49;93mnumber\n
-    \33[1;49;92m> DESCRIPTION: \33[1;49;97mWhen you type `number`, it will perform reverse phone number lookup
+    \33[1;49;92m> DESCRIPTION: \33[1;49;97mWhen you type `number`, it will reverse lookup phone number over internet and show public info associated with it
     \33[1;49;92m> SYNTAX: \33[1;49;97mnumber <phone_number>
     \33[1;49;92m> EXAMPLE: \33[1;49;97mnumber +1234567890
     \033[0m'''
                     print(number_help)
-                elif cmd == 'email':
+                elif cmd == 'whois':
+                    crt_exp = exp[1]
+                    whois_help = '''  \33[1;49;93m[+] Command Info: \33[1;49;93mwhois\n
+    \33[1;49;92m> DESCRIPTION: \33[1;49;97mWhen you type `whois`, it will perform reverse whois lookup
+    \33[1;49;92m> SYNTAX: \33[1;49;97mwhois <domain_name>
+    \33[1;49;92m> EXAMPLE: \33[1;49;97mwhois example.com
+    \033[0m'''
+                    print(whois_help)
+                elif cmd == 'dns':
                     crt_exp = exp[1]
-                    email_help = f'''  \33[1;49;93m[+] Command Info: \33[1;49;93memail\n
-    \33[1;49;92m> DESCRIPTION: \33[1;49;97mWhen you type `email`, it will perform reverse email lookup
-    \33[1;49;92m> SYNTAX: \33[1;49;97memail <email_address>
-    \33[1;49;92m> EXAMPLE: \33[1;49;97memail {user.strip()}\33[1;49;96m@gmail.com
+                    dns_help = '''  \33[1;49;93m[+] Command Info: \33[1;49;93mdns\n
+    \33[1;49;92m> DESCRIPTION: \33[1;49;97mWhen you type `dns`, it will perform dns lookup for given domain name or reverse dns lookup for given ip address
+    \33[1;49;92m> SYNTAX: \33[1;49;97mdns <ip_address/domain_name>
+    \33[1;49;92m> EXAMPLE: \33[1;49;97mdns 192.168.1.1 \33[1;49;92mOR \33[1;49;97mdns example.com
     \033[0m'''
-                    print(email_help)
+                    print(dns_help)
                 elif cmd == 'ip':
                     crt_exp = exp[1]
                     ip_help = '''  \33[1;49;93m[+] Command Info: \33[1;49;93mip\n
-    \33[1;49;92m> DESCRIPTION: \33[1;49;97mWhen you type `ip`, it will perform reverse ip address lookup
+    \33[1;49;92m> DESCRIPTION: \33[1;49;97mWhen you type `ip`, it will perform an ip address lookup over internet and show info about given ip address
     \33[1;49;92m> SYNTAX: \33[1;49;97mip <ip_address>
     \33[1;49;92m> EXAMPLE: \33[1;49;97mip 8.8.8.8
     \033[0m'''
                     print(ip_help)
+                elif cmd == 'mac':
+                    crt_exp = exp[1]
+                    mac_help = '''  \33[1;49;93m[+] Command Info: \33[1;49;93mmac\n
+    \33[1;49;92m> DESCRIPTION: \33[1;49;97mWhen you type `mac`, it will lookup probable vendor/manufacture of given mac address
+    \33[1;49;92m> SYNTAX: \33[1;49;97mmac <mac_address>
+    \33[1;49;92m> EXAMPLE: \33[1;49;97mmac ff:ff:ff:ff:ff:ff
+    \033[0m'''
+                    print(mac_help)
                 else:
                     crt_exp = exp[3]
                     printit('    [!] Invalid sub-command! Type `help` to see all available commands.', coledt=[1, 49, 91])
             else:
                 crt_exp = exp[3]
                 printit('    [!] Invalid command! Type `help` to see all available commands.', coledt=[1, 49, 91])
             prv_op = ''
 
         # Basic commands
         elif cmd == 'exit' or cmd == 'quit':
-            printit('    [@] Thank you for using `PH0MBER` osint framework :)', coledt=[1, 49, random.choice([92, 96, 97])])
+            if not silent_mode: printit('    [@] Thank you for using `PH0MBER` osint framework :)', coledt=[1, 49, random.choice([92, 96, 97])])
+            # printit('    [@] Support this project: https://www.buymeacoffee.com/s41r4j', coledt=[1, 49, random.choice([92, 97])])
             raise KeyboardInterrupt
         elif cmd == 'dork':
             crt_exp = exp[1]
             prv_op = ''
             printit('    [+] Generating random dork query...', coledt=[1, 49, 93], space_down=True)
             printit('    > '+dork_query(), coledt=[1, 49, 92])
         elif cmd == 'exp':
@@ -959,15 +1188,15 @@
                 print(exec_cmd)
             
                 output = os.system(cmd)
                 if output == 0:
                     printit('> Command executed successfully!', coledt=[7, 49, 92], normaltxt_start='\n    ')
                     crt_exp = exp[0]
                 else:
-                    printit('\n    > Command execution failed!', coledt=[1, 49, 91])
+                    printit('> Command execution failed!', coledt=[7, 49, 91], normaltxt_start='\n    ')
                     crt_exp = exp[3]
             else:
                 crt_exp = exp[3]
                 printit('    [!] Invalid command! Type `help` to see all available commands.', coledt=[1, 49, 91])
             prv_op = ''
         elif cmd == 'info':
             crt_exp = exp[1]
@@ -997,35 +1226,87 @@
             prv_op = ''
 
         # Scanner commands
         elif cmd == 'number':
             crt_exp = exp[2]
             printit('    > No phone number found! Type `help number` to see more info', coledt=[1, 49, 91])
         elif cmd[:6] == 'number':
+            full_cmd = cmd
             if (cmd+'#')[6]  == ' ':
                 cmd = cmd[7:]
                 printit('    [+] Performing reverse phone number lookup...', coledt=[1, 49, 93], space_down=True)
                 if number_lookup(cmd):
                     crt_exp = exp[4]
                 else:
                     crt_exp = exp[3]
+                    prv_op = ''
             else:
                 crt_exp = exp[3]
                 printit('    [!] Invalid command! Type `help` to see all available commands.', coledt=[1, 49, 91])
         elif cmd == 'ip':
             crt_exp = exp[2]
             printit('    > No ip address found! Type `help ip` to see more info', coledt=[1, 49, 91])
         elif cmd[:2] == 'ip':
+            full_cmd = cmd
             if (cmd+'#')[2]  == ' ':
                 cmd = cmd[3:]
                 printit('    [+] Performing reverse ip address lookup...', coledt=[1, 49, 93], space_down=True)
                 if ip_lookup(cmd):
                     crt_exp = exp[4]
                 else:
                     crt_exp = exp[3]
+                    prv_op = ''
+            else:
+                crt_exp = exp[3]
+                printit('    [!] Invalid command! Type `help` to see all available commands.', coledt=[1, 49, 91])
+        elif cmd == 'mac':
+            crt_exp = exp[2]
+            printit('    > No mac address found! Type `help mac` to see more info', coledt=[1, 49, 91])
+        elif cmd[:3] == 'mac':
+            full_cmd = cmd
+            if (cmd+'#')[3]  == ' ':
+                cmd = cmd[4:]
+                printit('    [+] Performing reverse mac address lookup...', coledt=[1, 49, 93], space_down=True)
+                if mac_lookup(cmd):
+                    crt_exp = exp[4]
+                else:
+                    crt_exp = exp[3]
+                    prv_op = ''
+            else:
+                crt_exp = exp[3]
+                printit('    [!] Invalid command! Type `help` to see all available commands.', coledt=[1, 49, 91])
+        elif cmd == 'whois':
+            crt_exp = exp[2]
+            printit('    > No domain found! Type `help whois` to see more info', coledt=[1, 49, 91])
+        elif cmd[:5] == 'whois':
+            full_cmd = cmd
+            if (cmd+'#')[5]  == ' ':
+                cmd = cmd[6:]
+                printit('    [+] Performing reverse domain lookup...', coledt=[1, 49, 93], space_down=True)
+                if whois_lookup(cmd):
+                    crt_exp = exp[4]
+                else:
+                    crt_exp = exp[3]
+                    prv_op = ''
+            else:
+                crt_exp = exp[3]
+                printit('    [!] Invalid command! Type `help` to see all available commands.', coledt=[1, 49, 91])
+        elif cmd == 'dns':
+            crt_exp = exp[2]
+            printit('    > No domain found! Type `help dns` to see more info', coledt=[1, 49, 91])
+        elif cmd[:3] == 'dns':
+            full_cmd = cmd
+            if (cmd+'#')[3]  == ' ':
+                cmd = cmd[4:]
+                printit('    [+] Performing dns lookup...', coledt=[1, 49, 93], space_down=True)
+                if dns_lookup(cmd):
+                    crt_exp = exp[4]
+                else:
+                    crt_exp = exp[3]
+                    prv_op = ''
             else:
                 crt_exp = exp[3]
                 printit('    [!] Invalid command! Type `help` to see all available commands.', coledt=[1, 49, 91])
 
         # If command is not available
         else:
             crt_exp = exp[3]
@@ -1052,10 +1333,9 @@
     try:
         control_center()
     except KeyboardInterrupt:
         print()
         if not silent_mode:
             printit('[#] Terminating `PH0MBER` framework...', coledt=[1, 49, random.choice([91, 93])], space_down=True, line_down=True, line_up=True, space_up=True)
             exit()
+        else: print()
 
-# if __name__ == '__main__':
-#     main()
```

## Comparing `phomber/__pycache__/phomberv3_beta.cpython-39.pyc` & `phomber/__pycache__/phomberv3.0.2_beta.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Sun May 21 12:37:31 2023 UTC, .py size: 55263 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 12% similar despite different names*

```diff
@@ -1,2092 +1,2525 @@
-00000000: 610d 0d0a 0000 0000 8b10 6a64 dfd7 0000  a.........jd....
+00000000: 610d 0d0a 0000 0000 4dff 7a64 610d 0100  a.......M.zda...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 000b 0000 0040 0000 0073 d000 0000 6400  .....@...s....d.
+00000020: 000b 0000 0040 0000 0073 1c01 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6401 6c03 5a03 6400  d.l.Z.d.d.l.Z.d.
 00000050: 6401 6c04 5a04 6400 6401 6c05 5a05 6400  d.l.Z.d.d.l.Z.d.
 00000060: 6401 6c06 5a06 6400 6401 6c07 5a07 6400  d.l.Z.d.d.l.Z.d.
-00000070: 6401 6c08 5a08 6400 6401 6c09 5a09 6700  d.l.Z.d.d.l.Z.g.
-00000080: 6402 a201 5a0a 6403 610b 6404 610c 6405  d...Z.d.a.d.a.d.
-00000090: 6406 8400 5a0d 6407 6408 8400 5a0e 6409  d...Z.d.d...Z.d.
-000000a0: 640a 8400 5a0f 6403 6404 6404 6404 6404  d...Z.d.d.d.d.d.
-000000b0: 6700 640b a201 6403 6403 6404 6404 6404  g.d...d.d.d.d.d.
-000000c0: 660b 640c 640d 8401 5a10 640e 640f 8400  f.d.d...Z.d.d...
-000000d0: 5a11 6410 6411 8400 5a12 6412 6413 8400  Z.d.d...Z.d.d...
-000000e0: 5a13 6414 6415 8400 5a14 6416 6417 8400  Z.d.d...Z.d.d...
-000000f0: 5a15 6418 6419 8400 5a16 6401 5300 291a  Z.d.d...Z.d.S.).
-00000100: e900 0000 004e 290d da04 6865 6c70 da04  .....N)...help..
-00000110: 6578 6974 da04 7175 6974 da04 646f 726b  exit..quit..dork
-00000120: da03 6578 70da 0563 6865 636b da05 636c  ..exp..check..cl
-00000130: 6561 72da 0473 6176 65da 0573 6865 6c6c  ear..save..shell
-00000140: da04 696e 666f da06 6368 616e 6765 da06  ..info..change..
-00000150: 6e75 6d62 6572 da02 6970 da00 4663 0100  number..ip..Fc..
-00000160: 0000 0000 0000 0000 0000 0100 0000 0600  ................
-00000170: 0000 4300 0000 7328 0000 007a 1474 006a  ..C...s(...z.t.j
-00000180: 017c 0064 0164 028d 0201 0057 0064 0353  .|.d.d.....W.d.S
-00000190: 0001 0001 0001 0059 0064 0453 0030 0064  .......Y.d.S.0.d
-000001a0: 0053 0029 054e e90a 0000 0029 01da 0774  .S.).N.....)...t
-000001b0: 696d 656f 7574 5446 2902 da08 7265 7175  imeoutTF)...requ
-000001c0: 6573 7473 da03 6765 7429 01da 0375 726c  ests..get)...url
-000001d0: a900 7215 0000 00fa 3662 7569 6c64 2f62  ..r.....6build/b
-000001e0: 6469 7374 2e6c 696e 7578 2d78 3836 5f36  dist.linux-x86_6
-000001f0: 342f 6567 672f 7068 6f6d 6265 722f 7068  4/egg/phomber/ph
-00000200: 6f6d 6265 7276 335f 6265 7461 2e70 79da  omberv3_beta.py.
-00000210: 1063 6865 636b 5f63 6f6e 6e65 6374 696f  .check_connectio
-00000220: 6e33 0000 0073 0a00 0000 0002 0201 0e01  n3...s..........
-00000230: 0601 0601 7217 0000 0063 0100 0000 0000  ....r....c......
-00000240: 0000 0000 0000 1400 0000 1500 0000 4300  ..............C.
-00000250: 0000 733e 0400 0064 0164 026c 006d 017d  ..s>...d.d.l.m.}
-00000260: 0101 0064 0164 036c 006d 027d 0201 0064  ...d.d.l.m.}...d
-00000270: 0164 046c 006d 037d 0301 0064 0561 0474  .d.l.m.}...d.a.t
-00000280: 0564 067c 009b 0064 079d 0367 0064 08a2  .d.|...d...g.d..
-00000290: 0164 0964 0a8d 0301 0074 0464 0b7c 009b  .d.d.....t.d.|..
-000002a0: 0064 0c9d 0364 0d17 0037 0061 0474 06a0  .d...d...7.a.t..
-000002b0: 0764 0e7c 00a1 0273 7e74 0564 0f67 0064  .d.|...s~t.d.g.d
-000002c0: 10a2 0164 118d 0201 0074 0464 1237 0061  ...d.....t.d.7.a
-000002d0: 0464 1353 007a 0e74 00a0 087c 00a1 017d  .d.S.z.t...|...}
-000002e0: 0457 006e 3004 0074 006a 096a 0a79 bc01  .W.n0..t.j.j.y..
-000002f0: 0001 0001 0074 0564 1467 0064 10a2 0164  .....t.d.g.d...d
-00000300: 118d 0201 0074 0464 1537 0061 0459 0064  .....t.d.7.a.Y.d
-00000310: 1353 0030 0074 0b7c 0483 01a0 0c64 1664  .S.0.t.|.....d.d
-00000320: 17a1 0264 1719 00a0 0c64 1864 17a1 0264  ...d.....d.d...d
-00000330: 0119 00a0 0da1 007d 0574 0b7c 0483 01a0  .......}.t.|....
-00000340: 0c64 1664 17a1 0264 1719 00a0 0c64 1864  .d.d...d.....d.d
-00000350: 17a1 0264 1719 00a0 0da1 007d 0674 00a0  ...d.......}.t..
-00000360: 0e7c 04a1 017d 0774 00a0 0f7c 04a1 017d  .|...}.t...|...}
-00000370: 087c 0790 0372 d07c 0890 0372 d074 00a0  .|...r.|...r.t..
-00000380: 087c 0064 19a1 027d 0974 00a0 107c 04a1  .|.d...}.t...|..
-00000390: 017d 0a7c 03a0 117c 0964 1aa1 027d 0b74  .}.|...|.d...}.t
-000003a0: 00a0 087c 0064 1ba1 027d 0c7c 02a0 127c  ...|.d...}.|...|
-000003b0: 0c64 1aa1 027d 0d74 0b7c 01a0 137c 04a1  .d...}.t.|...|..
-000003c0: 0183 017d 0e7c 0ea0 1464 1c64 05a1 02a0  ...}.|...d.d....
-000003d0: 1464 1d64 05a1 02a0 1464 1e64 05a1 02a0  .d.d.....d.d....
-000003e0: 1464 1f64 05a1 02a0 1464 2064 05a1 02a0  .d.d.....d d....
-000003f0: 1464 2164 05a1 02a0 1464 2264 05a1 027d  .d!d.....d"d...}
-00000400: 0f74 00a0 157c 0474 006a 166a 17a1 02a0  .t...|.t.j.j....
-00000410: 1464 2364 05a1 027d 1074 0b7c 0883 0164  .d#d...}.t.|...d
-00000420: 2274 1864 2474 1974 0b7c 0883 0183 0118  "t.d$t.t.|......
-00000430: 0083 0114 0017 007d 0874 0b7c 0783 0164  .......}.t.|...d
-00000440: 2274 1864 2474 1974 0b7c 0783 0183 0118  "t.d$t.t.|......
-00000450: 0083 0114 0017 007d 0774 0b7c 0583 0164  .......}.t.|...d
-00000460: 2274 1864 2474 1974 0b7c 0583 0183 0118  "t.d$t.t.|......
-00000470: 0083 0114 0017 007d 0574 0b7c 0b83 0164  .......}.t.|...d
-00000480: 2274 1864 2474 1974 0b7c 0b83 0183 0118  "t.d$t.t.|......
-00000490: 0083 0114 0017 007d 0b74 0b7c 0a83 0164  .......}.t.|...d
-000004a0: 2274 1864 2474 1974 0b7c 0a83 0183 0118  "t.d$t.t.|......
-000004b0: 0083 0114 0017 007d 0a74 0b7c 0d83 0164  .......}.t.|...d
-000004c0: 2274 1864 2474 1974 0b7c 0d83 0183 0118  "t.d$t.t.|......
-000004d0: 0083 0114 0017 007d 0d74 0b7c 0f83 0164  .......}.t.|...d
-000004e0: 2274 1864 2474 1974 0b7c 0f83 0183 0118  "t.d$t.t.|......
-000004f0: 0083 0114 0017 007d 0f74 0b7c 0083 0164  .......}.t.|...d
-00000500: 2274 1864 2474 1974 0b7c 0083 0183 0118  "t.d$t.t.|......
-00000510: 0083 0114 0017 007d 0074 0b7c 0683 0164  .......}.t.|...d
-00000520: 2274 1864 2474 1974 0b7c 0683 0183 0118  "t.d$t.t.|......
-00000530: 0083 0114 0017 007d 0674 0b7c 1083 0164  .......}.t.|...d
-00000540: 2274 1864 2474 1974 0b7c 1083 0183 0118  "t.d$t.t.|......
-00000550: 0083 0114 0017 007d 1064 257c 089b 0064  .......}.d%|...d
-00000560: 267c 079b 0064 277c 059b 0064 287c 0b9b  &|...d'|...d(|..
-00000570: 0064 297c 0a9b 0064 2a7c 0d9b 0064 2b7c  .d)|...d*|...d+|
-00000580: 0f9b 0064 2c7c 009b 0064 2d7c 069b 0064  ...d,|...d-|...d
-00000590: 2e7c 109b 0064 2f9d 157d 1174 1a7c 1183  .|...d/..}.t.|..
-000005a0: 0101 0074 047c 1164 0d17 0037 0061 0464  ...t.|.d...7.a.d
-000005b0: 307c 00a0 0da1 009b 0064 317c 0aa0 0da1  0|.......d1|....
-000005c0: 009b 0064 327c 06a0 0da1 009b 0064 337c  ...d2|.......d3|
-000005d0: 0aa0 0da1 00a0 1ba1 009b 0064 327c 06a0  ...........d2|..
-000005e0: 0da1 009b 0064 349d 0b7d 1274 1a7c 1283  .....d4..}.t.|..
-000005f0: 0101 0074 047c 1264 0d17 0037 0061 0464  ...t.|.d...7.a.d
-00000600: 357c 06a0 0da1 009b 0064 349d 037d 1374  5|.......d4..}.t
-00000610: 1a7c 1383 0101 0074 047c 1364 0d17 0037  .|.....t.|.d...7
-00000620: 0061 0464 0953 0074 0b7c 0883 0164 2274  .a.d.S.t.|...d"t
-00000630: 1864 2474 1974 0b7c 0883 0183 0118 0083  .d$t.t.|........
-00000640: 0114 0017 007d 0874 0b7c 0783 0164 2274  .....}.t.|...d"t
-00000650: 1864 2474 1974 0b7c 0783 0183 0118 0083  .d$t.t.|........
-00000660: 0114 0017 007d 0764 257c 089b 0064 267c  .....}.d%|...d&|
-00000670: 079b 0064 2f9d 057d 1174 1a7c 1183 0101  ...d/..}.t.|....
-00000680: 0074 047c 1164 0d17 0037 0061 0464 1353  .t.|.d...7.a.d.S
-00000690: 0064 0053 0029 364e 7201 0000 0029 01da  .d.S.)6Nr....)..
-000006a0: 0874 696d 657a 6f6e 6529 01da 0763 6172  .timezone)...car
-000006b0: 7269 6572 2901 da08 6765 6f63 6f64 6572  rier)...geocoder
-000006c0: 720f 0000 00fa 2f20 2020 205b 2b5d 2047  r...../    [+] G
-000006d0: 7261 7468 6572 696e 6720 696e 666f 726d  rathering inform
-000006e0: 6174 696f 6e20 6162 6f75 7420 1b5b 313b  ation about .[1;
-000006f0: 3439 3b39 366d fa0d 1b5b 313b 3439 3b39  49;96m...[1;49;9
-00000700: 336d 2e2e 2ea9 03e9 0100 0000 e931 0000  3m...........1..
-00000710: 00e9 5d00 0000 54a9 02da 0663 6f6c 6564  ..]...T....coled
-00000720: 74da 0a73 7061 6365 5f64 6f77 6e7a 3d0a  t..space_downz=.
-00000730: 2020 2020 1b5b 313b 3439 3b39 336d 5b23      .[1;49;93m[#
-00000740: 5d20 5265 7665 7273 6520 7068 6f6e 6520  ] Reverse phone 
-00000750: 6e75 6d62 6572 206c 6f6f 6b75 7020 666f  number lookup fo
-00000760: 7220 1b5b 313b 3439 3b39 366d fa0f 1b5b  r .[1;49;96m...[
-00000770: 313b 3439 3b39 336d 3a1b 5b30 6dda 010a  1;49;93m:.[0m...
-00000780: 7a11 5e5c 2b5b 312d 395d 5c64 7b31 2c31  z.^\+[1-9]\d{1,1
-00000790: 347d 247a 3b20 2020 203e 2049 6e76 616c  4}$z;    > Inval
-000007a0: 6964 2070 686f 6e65 206e 756d 6265 7220  id phone number 
-000007b0: 666f 726d 6174 2120 2845 7861 6d70 6c65  format! (Example
-000007c0: 3a20 2b34 3478 7878 7878 7878 7878 7829  : +44xxxxxxxxxx)
-000007d0: a903 721e 0000 0072 1f00 0000 e95b 0000  ..r....r.....[..
-000007e0: 00a9 0172 2200 0000 7a3c 2020 2020 3e20  ...r"...z<    > 
-000007f0: 496e 7661 6c69 6420 7068 6f6e 6520 6e75  Invalid phone nu
-00000800: 6d62 6572 2066 6f72 6d61 7421 2028 4578  mber format! (Ex
-00000810: 616d 706c 653a 202b 3434 7878 7878 7878  ample: +44xxxxxx
-00000820: 7878 7878 290a 467a 3320 2020 203e 204d  xxxx).Fz3    > M
-00000830: 6973 7369 6e67 2043 6f75 6e74 7279 2043  issing Country C
-00000840: 6f64 6521 2028 4578 616d 706c 653a 202b  ode! (Example: +
-00000850: 3931 2c20 2b34 342c 202b 3129 7a34 2020  91, +44, +1)z4  
-00000860: 2020 3e20 4d69 7373 696e 6720 436f 756e    > Missing Coun
-00000870: 7472 7920 436f 6465 2120 2845 7861 6d70  try Code! (Examp
-00000880: 6c65 3a20 2b39 312c 202b 3434 2c20 2b31  le: +91, +44, +1
-00000890: 290a 7a0d 436f 756e 7472 7920 436f 6465  ).z.Country Code
-000008a0: 3a72 1e00 0000 7a10 4e61 7469 6f6e 616c  :r....z.National
-000008b0: 204e 756d 6265 723a 5a02 4348 da02 656e   Number:Z.CH..en
-000008c0: 5a02 524f fa01 5bfa 015d fa01 27fa 0128  Z.RO..[..]..'..(
-000008d0: fa01 29fa 012c fa01 207a 0474 656c 3ae9  ..)..,.. z.tel:.
-000008e0: 1e00 0000 7552 0100 000a 2020 2020 e294  ....uR....    ..
-000008f0: 8ce2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00000900: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00000910: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00000920: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00000930: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00000940: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00000950: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00000960: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00000970: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00000980: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00000990: e294 80e2 9490 0a20 2020 207c 2049 4e46  .......    | INF
-000009a0: 4f52 4d41 5449 4f4e 2020 2020 2020 2020  ORMATION        
-000009b0: 207c 2044 4553 4352 4950 5449 4f4e 2020   | DESCRIPTION  
-000009c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000009d0: 2020 7c0a 2020 2020 7c2d 2d2d 2d2d 2d2d    |.    |-------
-000009e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000009f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000a00: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d7c  ---------------|
-00000a10: 0a20 2020 207c 201b 5b31 3b34 393b 3937  .    | .[1;49;97
-00000a20: 6d50 6f73 7369 626c 651b 5b30 6d20 2020  mPossible.[0m   
-00000a30: 2020 2020 2020 2020 207c 207a 2d20 7c0a           | z- |.
-00000a40: 2020 2020 7c20 1b5b 313b 3439 3b39 376d      | .[1;49;97m
-00000a50: 5661 6c69 641b 5b30 6d20 2020 2020 2020  Valid.[0m       
-00000a60: 2020 2020 2020 2020 7c20 7a6a 207c 0a20          | zj |. 
-00000a70: 2020 207c 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d     |------------
-00000a80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000a90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000aa0: 2d2d 2d2d 2d2d 2d2d 2d2d 7c0a 2020 2020  ----------|.    
-00000ab0: 7c20 1b5b 313b 3439 3b39 376d 436f 756e  | .[1;49;97mCoun
-00000ac0: 7472 7920 436f 6465 1b5b 306d 2020 2020  try Code.[0m    
-00000ad0: 2020 2020 7c20 7a2d 207c 0a20 2020 207c      | z- |.    |
-00000ae0: 201b 5b31 3b34 393b 3937 6d43 6f75 6e74   .[1;49;97mCount
-00000af0: 7279 1b5b 306d 2020 2020 2020 2020 2020  ry.[0m          
-00000b00: 2020 207c 20fa 2d20 7c0a 2020 2020 7c20     | .- |.    | 
-00000b10: 1b5b 313b 3439 3b39 376d 5265 6769 6f6e  .[1;49;97mRegion
-00000b20: 2043 6f64 651b 5b30 6d20 2020 2020 2020   Code.[0m       
-00000b30: 2020 7c20 7a2d 207c 0a20 2020 207c 201b    | z- |.    | .
-00000b40: 5b31 3b34 393b 3937 6d53 6572 7669 6365  [1;49;97mService
-00000b50: 2050 726f 7669 6465 721b 5b30 6d20 2020   Provider.[0m   
-00000b60: 207c 20fa 2d20 7c0a 2020 2020 7c20 1b5b   | .- |.    | .[
-00000b70: 313b 3439 3b39 376d 5469 6d65 7a6f 6e65  1;49;97mTimezone
-00000b80: 1b5b 306d 2020 2020 2020 2020 2020 2020  .[0m            
-00000b90: 7c20 7a6a 207c 0a20 2020 207c 2d2d 2d2d  | zj |.    |----
-00000ba0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000bb0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000bc0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000bd0: 2d2d 7c0a 2020 2020 7c20 1b5b 313b 3439  --|.    | .[1;49
-00000be0: 3b39 376d 496e 7465 726e 6174 696f 6e61  ;97mInternationa
-00000bf0: 6c20 466f 726d 6174 1b5b 306d 7c20 7a2d  l Format.[0m| z-
-00000c00: 207c 0a20 2020 207c 201b 5b31 3b34 393b   |.    | .[1;49;
-00000c10: 3937 6d4e 6174 696f 6e61 6c20 466f 726d  97mNational Form
-00000c20: 6174 1b5b 306d 2020 2020 207c 207a 2d20  at.[0m     | z- 
-00000c30: 7c0a 2020 2020 7c20 1b5b 313b 3439 3b39  |.    | .[1;49;9
-00000c40: 376d 5246 4333 3936 3620 466f 726d 6174  7mRFC3966 Format
-00000c50: 1b5b 306d 2020 2020 2020 7c20 75b8 0000  .[0m      | u...
-00000c60: 0020 7c0a 2020 2020 e294 94e2 9480 e294  . |.    ........
-00000c70: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00000c80: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00000c90: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00000ca0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00000cb0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00000cc0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00000cd0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00000ce0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00000cf0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00000d00: 80e2 9480 e294 80e2 9480 e294 80e2 9498  ................
-00000d10: 0a20 2020 2020 2020 207a 2b0a 2020 2020  .        z+.    
-00000d20: 1b5b 313b 3439 3b39 336d 5b2b 5d20 5365  .[1;49;93m[+] Se
-00000d30: 6172 6368 696e 6720 666f 7220 1b5b 313b  arching for .[1;
-00000d40: 3439 3b39 366d 7a74 1b5b 313b 3439 3b39  49;96mzt.[1;49;9
-00000d50: 336d 206f 6e20 7661 7269 6f75 7320 706c  3m on various pl
-00000d60: 6174 666f 726d 733a 0a0a 2020 2020 1b5b  atforms:..    .[
-00000d70: 313b 3439 3b39 326d 3e20 6874 7470 733a  1;49;92m> https:
-00000d80: 2f2f 7777 772e 6970 7175 616c 6974 7973  //www.ipqualitys
-00000d90: 636f 7265 2e63 6f6d 2f72 6576 6572 7365  core.com/reverse
-00000da0: 2d70 686f 6e65 2d6e 756d 6265 722d 6c6f  -phone-number-lo
-00000db0: 6f6b 7570 2f6c 6f6f 6b75 702f fa01 2f7a  okup/lookup/../z
-00000dc0: 290a 2020 2020 3e20 6874 7470 733a 2f2f  ).    > https://
-00000dd0: 7777 772e 7472 7565 6361 6c6c 6572 2e63  www.truecaller.c
-00000de0: 6f6d 2f73 6561 7263 682f 7a09 0a20 2020  om/search/z..   
-00000df0: 201b 5b30 6d7a 590a 2020 2020 1b5b 313b   .[0mzY.    .[1;
-00000e00: 3439 3b39 336d 5b2b 5d20 476f 6f67 6c65  49;93m[+] Google
-00000e10: 2044 6f72 6b20 5175 6572 6965 733a 0a0a   Dork Queries:..
-00000e20: 2020 2020 1b5b 313b 3439 3b39 326d 3e20      .[1;49;92m> 
-00000e30: 6874 7470 733a 2f2f 7777 772e 676f 6f67  https://www.goog
-00000e40: 6c65 2e63 6f6d 2f73 6561 7263 683f 713d  le.com/search?q=
-00000e50: 291c da0c 7068 6f6e 656e 756d 6265 7273  )...phonenumbers
-00000e60: 7218 0000 0072 1900 0000 721a 0000 00da  r....r....r.....
-00000e70: 0670 7276 5f6f 70da 0770 7269 6e74 6974  .prv_op..printit
-00000e80: da02 7265 da05 6d61 7463 68da 0570 6172  ..re..match..par
-00000e90: 7365 5a0f 7068 6f6e 656e 756d 6265 7275  seZ.phonenumberu
-00000ea0: 7469 6c5a 144e 756d 6265 7250 6172 7365  tilZ.NumberParse
-00000eb0: 4578 6365 7074 696f 6eda 0373 7472 da05  Exception..str..
-00000ec0: 7370 6c69 74da 0573 7472 6970 5a0f 6973  split..stripZ.is
-00000ed0: 5f76 616c 6964 5f6e 756d 6265 725a 1269  _valid_numberZ.i
-00000ee0: 735f 706f 7373 6962 6c65 5f6e 756d 6265  s_possible_numbe
-00000ef0: 725a 1672 6567 696f 6e5f 636f 6465 5f66  rZ.region_code_f
-00000f00: 6f72 5f6e 756d 6265 725a 1664 6573 6372  or_numberZ.descr
-00000f10: 6970 7469 6f6e 5f66 6f72 5f6e 756d 6265  iption_for_numbe
-00000f20: 725a 0f6e 616d 655f 666f 725f 6e75 6d62  rZ.name_for_numb
-00000f30: 6572 5a15 7469 6d65 5f7a 6f6e 6573 5f66  erZ.time_zones_f
-00000f40: 6f72 5f6e 756d 6265 72da 0772 6570 6c61  or_number..repla
-00000f50: 6365 5a0d 666f 726d 6174 5f6e 756d 6265  ceZ.format_numbe
-00000f60: 725a 1150 686f 6e65 4e75 6d62 6572 466f  rZ.PhoneNumberFo
-00000f70: 726d 6174 5a07 5246 4333 3936 36da 0369  rmatZ.RFC3966..i
-00000f80: 6e74 da03 6c65 6eda 0570 7269 6e74 da05  nt..len..print..
-00000f90: 6c6f 7765 7229 145a 0c70 686f 6e65 5f6e  lower).Z.phone_n
-00000fa0: 756d 6265 7272 1800 0000 7219 0000 0072  umberr....r....r
-00000fb0: 1a00 0000 5a14 7068 6f6e 655f 6e75 6d62  ....Z.phone_numb
-00000fc0: 6572 5f64 6574 6169 6c73 da0c 636f 756e  er_details..coun
-00000fd0: 7472 795f 636f 6465 5a0b 6f6e 6c79 5f6e  try_codeZ.only_n
-00000fe0: 756d 6265 725a 0576 616c 6964 da08 706f  umberZ.valid..po
-00000ff0: 7373 6962 6c65 5a0e 636f 756e 7274 795f  ssibleZ.counrty_
-00001000: 6e75 6d62 6572 da0b 7265 6769 6f6e 5f63  number..region_c
-00001010: 6f64 65da 0763 6f75 6e74 7279 5a0e 7365  ode..countryZ.se
-00001020: 7276 6963 655f 6e75 6d62 6572 5a10 7365  rvice_numberZ.se
-00001030: 7276 6963 655f 7072 6f76 6964 6572 5a1b  rvice_providerZ.
-00001040: 7469 6d65 7a6f 6e65 5f64 6574 6169 6c73  timezone_details
-00001050: 5f75 6e66 696c 7465 7265 645a 1074 696d  _unfilteredZ.tim
-00001060: 657a 6f6e 655f 6465 7461 696c 735a 0872  ezone_detailsZ.r
-00001070: 5f66 6f72 6d61 74da 0c66 696e 616c 5f6f  _format..final_o
-00001080: 7574 7075 745a 126f 6e6c 696e 655f 6672  utputZ.online_fr
-00001090: 6565 5f6c 6f6f 6b75 705a 1367 6f6f 676c  ee_lookupZ.googl
-000010a0: 655f 646f 726b 5f71 7565 7269 6573 7215  e_dork_queriesr.
-000010b0: 0000 0072 1500 0000 7216 0000 00da 0d6e  ...r....r......n
-000010c0: 756d 6265 725f 6c6f 6f6b 7570 3c00 0000  umber_lookup<...
-000010d0: 73b6 0000 0000 020c 010c 010c 0404 031a  s...............
-000010e0: 0114 030c 0110 0108 0104 0302 020e 0110  ................
-000010f0: 0110 0108 0108 0324 0124 030a 030a 020c  .......$.$......
-00001100: 020c 030a 030c 030c 030c 030e 013c 0318  .............<..
-00001110: 0320 0120 0120 0120 0120 0120 0120 0120  . . . . . . . . 
-00001120: 0120 0120 0302 0402 fc04 0502 fb04 0702  . . ............
-00001130: f904 0802 f804 0902 f704 0a02 f604 0b02  ................
-00001140: f504 0d02 f304 0e02 f204 0f02 f108 1208  ................
-00001150: 010c 0302 0106 ff04 0306 fd04 0306 fd04  ................
-00001160: 040a fc04 0306 fd08 0608 010c 0302 0306  ................
-00001170: fd08 0508 010c 0204 0420 0120 0202 0402  ......... . ....
-00001180: fc04 0502 fb08 0808 010c 0172 4800 0000  ...........rH...
-00001190: 6301 0000 0000 0000 0000 0000 0036 0000  c............6..
-000011a0: 0037 0000 0043 0000 0073 280f 0000 6401  .7...C...s(...d.
-000011b0: 6100 7401 6402 6700 6403 a201 6404 6405  a.t.d.g.d...d.d.
-000011c0: 8d03 0100 7402 6406 8301 733c 7401 6407  ....t.d...s<t.d.
-000011d0: 6700 6408 a201 6404 6405 8d03 0100 7400  g.d...d.d.....t.
-000011e0: 6409 3700 6100 640a 5300 7401 640b 7c00  d.7.a.d.S.t.d.|.
-000011f0: 9b00 640c 9d03 6700 6403 a201 6404 6405  ..d...g.d...d.d.
-00001200: 8d03 0100 7400 640d 7c00 9b00 640e 9d03  ....t.d.|...d...
-00001210: 640f 1700 3700 6100 7403 a004 6410 7c00  d...7.a.t...d.|.
-00001220: a102 7392 7401 6411 6700 6408 a201 6412  ..s.t.d.g.d...d.
-00001230: 8d02 0100 7400 6413 3700 6100 6400 5300  ....t.d.7.a.d.S.
-00001240: 6414 7c00 9b00 9d02 6415 7c00 9b00 6416  d.|.....d.|...d.
-00001250: 9d03 6417 7c00 9b00 9d02 6703 7d01 7405  ..d.|.....g.}.t.
-00001260: 7c00 8301 6418 7406 6419 7407 7405 7c00  |...d.t.d.t.t.|.
-00001270: 8301 8301 1800 8301 1400 1700 7d00 641a  ............}.d.
-00001280: 641b 6901 7d02 7408 a009 6700 641c a201  d.i.}.t...g.d...
-00001290: a101 7d03 7c03 641d 6b02 9003 72cc 9002  ..}.|.d.k...r...
-000012a0: 7a86 740a 6a0b 7c01 641d 1900 641e 7c02  z.t.j.|.d...d.|.
-000012b0: 641f 8d03 7d04 7c04 a00c a100 7d05 7c04  d...}.|.....}.|.
-000012c0: 6a0d 6420 6b02 9001 728c 7c05 6421 1900  j.d k...r.|.d!..
-000012d0: 6422 6b02 9001 728c 7c05 6423 1900 7d06  d"k...r.|.d#..}.
-000012e0: 7c05 6424 1900 7d07 7c05 6425 1900 7d08  |.d$..}.|.d%..}.
-000012f0: 7c05 6426 1900 7d09 7c05 6427 1900 7d0a  |.d&..}.|.d'..}.
-00001300: 7c05 6428 1900 7d0b 7c05 6429 1900 7d0c  |.d(..}.|.d)..}.
-00001310: 7c05 642a 1900 7d0d 7c05 642b 1900 7d0e  |.d*..}.|.d+..}.
-00001320: 7c05 642c 1900 7d0f 7c05 642d 1900 7d10  |.d,..}.|.d-..}.
-00001330: 7c05 642e 1900 7d11 6e08 740e 642f 8301  |.d...}.n.t.d/..
-00001340: 8201 7405 7c06 8301 6418 7406 6419 7407  ..t.|...d.t.d.t.
-00001350: 7405 7c06 8301 8301 1800 8301 1400 1700  t.|.............
-00001360: 7d06 7405 7c07 8301 6418 7406 6419 7407  }.t.|...d.t.d.t.
-00001370: 7405 7c07 8301 8301 1800 8301 1400 1700  t.|.............
-00001380: 7d07 7405 7c08 8301 6418 7406 6419 7407  }.t.|...d.t.d.t.
-00001390: 7405 7c08 8301 8301 1800 8301 1400 1700  t.|.............
-000013a0: 7d08 7405 7c09 8301 6418 7406 6419 7407  }.t.|...d.t.d.t.
-000013b0: 7405 7c09 8301 8301 1800 8301 1400 1700  t.|.............
-000013c0: 7d09 7405 7c0a 8301 6418 7406 6419 7407  }.t.|...d.t.d.t.
-000013d0: 7405 7c0a 8301 8301 1800 8301 1400 1700  t.|.............
-000013e0: 7d0a 7405 7c0b 8301 6418 7406 6419 7407  }.t.|...d.t.d.t.
-000013f0: 7405 7c0b 8301 8301 1800 8301 1400 1700  t.|.............
-00001400: 7d0b 7405 7c0c 8301 6418 7406 6419 7407  }.t.|...d.t.d.t.
-00001410: 7405 7c0c 8301 8301 1800 8301 1400 1700  t.|.............
-00001420: 7d0c 7405 7c0d 8301 6418 7406 6419 7407  }.t.|...d.t.d.t.
-00001430: 7405 7c0d 8301 8301 1800 8301 1400 1700  t.|.............
-00001440: 7d0d 7405 7c0e 8301 6418 7406 6419 7407  }.t.|...d.t.d.t.
-00001450: 7405 7c0e 8301 8301 1800 8301 1400 1700  t.|.............
-00001460: 7d0e 7405 7c0f 8301 6418 7406 6419 7407  }.t.|...d.t.d.t.
-00001470: 7405 7c0f 8301 8301 1800 8301 1400 1700  t.|.............
-00001480: 7d0f 7405 7c10 8301 6418 7406 6419 7407  }.t.|...d.t.d.t.
-00001490: 7405 7c10 8301 8301 1800 8301 1400 1700  t.|.............
-000014a0: 7d10 7405 7c11 8301 6418 7406 6419 7407  }.t.|...d.t.d.t.
-000014b0: 7405 7c11 8301 8301 1800 8301 1400 1700  t.|.............
-000014c0: 7d11 6430 7c00 9b00 6431 7c06 9b00 6432  }.d0|...d1|...d2
-000014d0: 7c07 9b00 6433 7c08 9b00 6434 7c09 9b00  |...d3|...d4|...
-000014e0: 6435 7c0a 9b00 6436 7c0e 9b00 6437 7c0d  d5|...d6|...d7|.
-000014f0: 9b00 6438 7c0f 9b00 6439 7c10 9b00 643a  ..d8|...d9|...d:
-00001500: 7c0b 9b00 643b 7c0c 9b00 643c 9d19 7d12  |...d;|...d<..}.
-00001510: 740f 7c12 8301 0100 7400 7c12 640f 1700  t.|.....t.|.d...
-00001520: 3700 6100 5700 6e4e 0400 740e 9003 79c6  7.a.W.nN..t...y.
-00001530: 0100 7d13 0100 7a34 740f 7c13 8301 0100  ..}...z4t.|.....
-00001540: 6430 7c00 9b00 643d 9d03 7d12 740f 7c12  d0|...d=..}.t.|.
-00001550: 8301 0100 7400 7c12 640f 1700 3700 6100  ....t.|.d...7.a.
-00001560: 5700 5900 6400 7d13 7e13 6e0a 6400 7d13  W.Y.d.}.~.n.d.}.
-00001570: 7e13 3000 3000 900b 6e58 7c03 643e 6b02  ~.0.0...nX|.d>k.
-00001580: 9009 7234 9005 7a2a 740a 6a0b 7c01 643e  ..r4..z*t.j.|.d>
-00001590: 1900 641e 7c02 641f 8d03 7d04 7c04 a00c  ..d.|.d...}.|...
-000015a0: a100 7d05 7c04 6a0d 6420 6b02 9004 72dc  ..}.|.j.d k...r.
-000015b0: 7c05 643f 1900 7d11 7c05 6440 1900 7d14  |.d?..}.|.d@..}.
-000015c0: 7c05 6441 1900 7d15 7c05 6427 1900 7d0a  |.dA..}.|.d'..}.
-000015d0: 7c05 6426 1900 7d08 7c05 6442 1900 7d16  |.d&..}.|.dB..}.
-000015e0: 7c05 6443 1900 7d06 7c05 6443 1900 7d17  |.dC..}.|.dC..}.
-000015f0: 7c05 6444 1900 7d18 7c05 6445 1900 7d19  |.dD..}.|.dE..}.
-00001600: 7c05 6446 1900 7d1a 7c05 6447 1900 7d1b  |.dF..}.|.dG..}.
-00001610: 7c05 6448 1900 7d1c 7c05 6449 1900 7d1d  |.dH..}.|.dI..}.
-00001620: 7c05 644a 1900 7d0e 7c05 644b 1900 7d0f  |.dJ..}.|.dK..}.
-00001630: 7c05 644c 1900 7d10 7c05 642a 1900 7d0d  |.dL..}.|.d*..}.
-00001640: 7c05 644d 1900 7d1e 7c05 644e 1900 7d1f  |.dM..}.|.dN..}.
-00001650: 7c05 644f 1900 7d20 7c05 6450 1900 7d21  |.dO..} |.dP..}!
-00001660: 7c05 6451 1900 7d22 7c05 6452 1900 7d23  |.dQ..}"|.dR..}#
-00001670: 7c05 6453 1900 7d24 7c05 6454 1900 7d25  |.dS..}$|.dT..}%
-00001680: 7c05 6429 1900 7d0c 6e08 740e 6455 8301  |.d)..}.n.t.dU..
-00001690: 8201 7405 7c11 8301 6418 7406 6419 7407  ..t.|...d.t.d.t.
-000016a0: 7405 7c11 8301 8301 1800 8301 1400 1700  t.|.............
-000016b0: 7d11 7405 7c14 8301 6418 7406 6419 7407  }.t.|...d.t.d.t.
-000016c0: 7405 7c14 8301 8301 1800 8301 1400 1700  t.|.............
-000016d0: 7d14 7405 7c15 8301 6418 7406 6419 7407  }.t.|...d.t.d.t.
-000016e0: 7405 7c15 8301 8301 1800 8301 1400 1700  t.|.............
-000016f0: 7d15 7405 7c0a 8301 6418 7406 6419 7407  }.t.|...d.t.d.t.
-00001700: 7405 7c0a 8301 8301 1800 8301 1400 1700  t.|.............
-00001710: 7d0a 7405 7c08 8301 6418 7406 6419 7407  }.t.|...d.t.d.t.
-00001720: 7405 7c08 8301 8301 1800 8301 1400 1700  t.|.............
-00001730: 7d08 7405 7c16 8301 6418 7406 6419 7407  }.t.|...d.t.d.t.
-00001740: 7405 7c16 8301 8301 1800 8301 1400 1700  t.|.............
-00001750: 7d16 7405 7c06 8301 6418 7406 6419 7407  }.t.|...d.t.d.t.
-00001760: 7405 7c06 8301 8301 1800 8301 1400 1700  t.|.............
-00001770: 7d06 7405 7c17 8301 6418 7406 6419 7407  }.t.|...d.t.d.t.
-00001780: 7405 7c17 8301 8301 1800 8301 1400 1700  t.|.............
-00001790: 7d17 7405 7c18 8301 6418 7406 6419 7407  }.t.|...d.t.d.t.
-000017a0: 7405 7c18 8301 8301 1800 8301 1400 1700  t.|.............
-000017b0: 7d18 7405 7c19 8301 6418 7406 6419 7407  }.t.|...d.t.d.t.
-000017c0: 7405 7c19 8301 8301 1800 8301 1400 1700  t.|.............
-000017d0: 7d19 7405 7c1a 8301 6418 7406 6419 7407  }.t.|...d.t.d.t.
-000017e0: 7405 7c1a 8301 8301 1800 8301 1400 1700  t.|.............
-000017f0: 7d1a 7405 7c1b 8301 6418 7406 6419 7407  }.t.|...d.t.d.t.
-00001800: 7405 7c1b 8301 8301 1800 8301 1400 1700  t.|.............
-00001810: 7d1b 7405 7c1c 8301 6418 7406 6419 7407  }.t.|...d.t.d.t.
-00001820: 7405 7c1c 8301 8301 1800 8301 1400 1700  t.|.............
-00001830: 7d1c 7405 7c1d 8301 6418 7406 6419 7407  }.t.|...d.t.d.t.
-00001840: 7405 7c1d 8301 8301 1800 8301 1400 1700  t.|.............
-00001850: 7d1d 7405 7c0e 8301 6418 7406 6419 7407  }.t.|...d.t.d.t.
-00001860: 7405 7c0e 8301 8301 1800 8301 1400 1700  t.|.............
-00001870: 7d0e 7405 7c0f 8301 6418 7406 6419 7407  }.t.|...d.t.d.t.
-00001880: 7405 7c0f 8301 8301 1800 8301 1400 1700  t.|.............
-00001890: 7d0f 7405 7c10 8301 6418 7406 6419 7407  }.t.|...d.t.d.t.
-000018a0: 7405 7c10 8301 8301 1800 8301 1400 1700  t.|.............
-000018b0: 7d10 7405 7c0d 8301 6418 7406 6419 7407  }.t.|...d.t.d.t.
-000018c0: 7405 7c0d 8301 8301 1800 8301 1400 1700  t.|.............
-000018d0: 7d0d 7405 7c1e 8301 6418 7406 6419 7407  }.t.|...d.t.d.t.
-000018e0: 7405 7c1e 8301 8301 1800 8301 1400 1700  t.|.............
-000018f0: 7d1e 7405 7c1f 8301 6418 7406 6419 7407  }.t.|...d.t.d.t.
-00001900: 7405 7c1f 8301 8301 1800 8301 1400 1700  t.|.............
-00001910: 7d1f 7405 7c20 8301 6418 7406 6419 7407  }.t.| ..d.t.d.t.
-00001920: 7405 7c20 8301 8301 1800 8301 1400 1700  t.| ............
-00001930: 7d20 7405 7c21 8301 6418 7406 6419 7407  } t.|!..d.t.d.t.
-00001940: 7405 7c21 8301 8301 1800 8301 1400 1700  t.|!............
-00001950: 7d21 7405 7c22 8301 6418 7406 6419 7407  }!t.|"..d.t.d.t.
-00001960: 7405 7c22 8301 8301 1800 8301 1400 1700  t.|"............
-00001970: 7d22 7405 7c23 8301 6418 7406 6419 7407  }"t.|#..d.t.d.t.
-00001980: 7405 7c23 8301 8301 1800 8301 1400 1700  t.|#............
-00001990: 7d23 7405 7c24 8301 6418 7406 6419 7407  }#t.|$..d.t.d.t.
-000019a0: 7405 7c24 8301 8301 1800 8301 1400 1700  t.|$............
-000019b0: 7d24 7405 7c25 8301 6418 7406 6419 7407  }$t.|%..d.t.d.t.
-000019c0: 7405 7c25 8301 8301 1800 8301 1400 1700  t.|%............
-000019d0: 7d25 7405 7c0c 8301 6418 7406 6419 7407  }%t.|...d.t.d.t.
-000019e0: 7405 7c0c 8301 8301 1800 8301 1400 1700  t.|.............
-000019f0: 7d0c 6430 7c00 9b00 6456 7c15 9b00 6457  }.d0|...dV|...dW
-00001a00: 7c14 9b00 6458 7c06 9b00 6459 7c17 9b00  |...dX|...dY|...
-00001a10: 6432 7c18 9b00 645a 7c19 9b00 645b 7c1a  d2|...dZ|...d[|.
-00001a20: 9b00 6433 7c08 9b00 6434 7c16 9b00 6435  ..d3|...d4|...d5
-00001a30: 7c0a 9b00 645c 7c1b 9b00 645d 7c1f 9b00  |...d\|...d]|...
-00001a40: 645e 7c1c 9b00 645f 7c1d 9b00 6460 7c23  d^|...d_|...d`|#
-00001a50: 9b00 6461 7c24 9b00 6462 7c22 9b00 6463  ..da|$..db|"..dc
-00001a60: 7c20 9b00 6464 7c21 9b00 6436 7c0e 9b00  | ..dd|!..d6|...
-00001a70: 6438 7c0f 9b00 6439 7c10 9b00 6437 7c0d  d8|...d9|...d7|.
-00001a80: 9b00 6465 7c1e 9b00 6466 7c25 9b00 6467  ..de|...df|%..dg
-00001a90: 7c0c 9b00 643c 9d37 7d12 740f 7c12 8301  |...d<.7}.t.|...
-00001aa0: 0100 7400 7c12 640f 1700 3700 6100 5700  ..t.|.d...7.a.W.
-00001ab0: 6e2c 0100 0100 0100 6430 7c00 9b00 6468  n,......d0|...dh
-00001ac0: 9d03 7d12 740f 7c12 8301 0100 7400 7c12  ..}.t.|.....t.|.
-00001ad0: 640f 1700 3700 6100 5900 6e02 3000 9005  d...7.a.Y.n.0...
-00001ae0: 6ef0 7c03 6469 6b02 900f 7224 9005 7ab6  n.|.dik...r$..z.
-00001af0: 740a 6a0b 7c01 6469 1900 641e 7c02 641f  t.j.|.di..d.|.d.
-00001b00: 8d03 7d04 7c04 a00c a100 7d05 7c04 6a0d  ..}.|.....}.|.j.
-00001b10: 6420 6b02 900a 7296 7c05 6422 1900 6404  d k...r.|.d"..d.
-00001b20: 6b02 900a 7296 7c05 643f 1900 7d11 7c05  k...r.|.d?..}.|.
-00001b30: 646a 1900 7d26 7c05 646b 1900 7d27 7c05  dj..}&|.dk..}'|.
-00001b40: 6448 1900 7d1c 7c05 6423 1900 7d06 7c05  dH..}.|.d#..}.|.
-00001b50: 6444 1900 7d18 7c05 6426 1900 7d08 7c05  dD..}.|.d&..}.|.
-00001b60: 6442 1900 7d16 7c05 6427 1900 7d0a 7c05  dB..}.|.d'..}.|.
-00001b70: 644b 1900 7d0f 7c05 644c 1900 7d10 7c05  dK..}.|.dL..}.|.
-00001b80: 646c 1900 7d28 7c05 644a 1900 7d0e 7c05  dl..}(|.dJ..}.|.
-00001b90: 646d 1900 7d29 7c05 646e 1900 7d2a 7c05  dm..})|.dn..}*|.
-00001ba0: 646f 1900 7d2b 7c05 6470 1900 6471 1900  do..}+|.dp..dq..
-00001bb0: 7d2c 7c05 6470 1900 6472 1900 7d2d 7c05  },|.dp..dr..}-|.
-00001bc0: 6470 1900 6473 1900 7d2e 7c05 6474 1900  dp..ds..}.|.dt..
-00001bd0: 6454 1900 7d25 7c05 6474 1900 6429 1900  dT..}%|.dt..d)..
-00001be0: 7d0c 7c05 6474 1900 6428 1900 7d0b 7c05  }.|.dt..d(..}.|.
-00001bf0: 6474 1900 6475 1900 7d2f 7c05 642a 1900  dt..du..}/|.d*..
-00001c00: 6476 1900 7d30 7c05 642a 1900 6477 1900  dv..}0|.d*..dw..
-00001c10: 7d31 7c05 642a 1900 6478 1900 7d32 7c05  }1|.d*..dx..}2|.
-00001c20: 642a 1900 6479 1900 7d33 7c05 642a 1900  d*..dy..}3|.d*..
-00001c30: 647a 1900 7d34 7c05 642a 1900 647b 1900  dz..}4|.d*..d{..
-00001c40: 7d35 6e08 740e 647c 8301 8201 7405 7c11  }5n.t.d|....t.|.
-00001c50: 8301 6418 7406 6419 7407 7405 7c11 8301  ..d.t.d.t.t.|...
-00001c60: 8301 1800 8301 1400 1700 7d11 7405 7c26  ..........}.t.|&
-00001c70: 8301 6418 7406 6419 7407 7405 7c26 8301  ..d.t.d.t.t.|&..
-00001c80: 8301 1800 8301 1400 1700 7d26 7405 7c27  ..........}&t.|'
-00001c90: 8301 6418 7406 6419 7407 7405 7c27 8301  ..d.t.d.t.t.|'..
-00001ca0: 8301 1800 8301 1400 1700 7d27 7405 7c1c  ..........}'t.|.
-00001cb0: 8301 6418 7406 6419 7407 7405 7c1c 8301  ..d.t.d.t.t.|...
-00001cc0: 8301 1800 8301 1400 1700 7d1c 7405 7c06  ..........}.t.|.
-00001cd0: 8301 6418 7406 6419 7407 7405 7c06 8301  ..d.t.d.t.t.|...
-00001ce0: 8301 1800 8301 1400 1700 7d06 7405 7c18  ..........}.t.|.
-00001cf0: 8301 6418 7406 6419 7407 7405 7c18 8301  ..d.t.d.t.t.|...
-00001d00: 8301 1800 8301 1400 1700 7d18 7405 7c08  ..........}.t.|.
-00001d10: 8301 6418 7406 6419 7407 7405 7c08 8301  ..d.t.d.t.t.|...
-00001d20: 8301 1800 8301 1400 1700 7d08 7405 7c16  ..........}.t.|.
-00001d30: 8301 6418 7406 6419 7407 7405 7c16 8301  ..d.t.d.t.t.|...
-00001d40: 8301 1800 8301 1400 1700 7d16 7405 7c0a  ..........}.t.|.
-00001d50: 8301 6418 7406 6419 7407 7405 7c0a 8301  ..d.t.d.t.t.|...
-00001d60: 8301 1800 8301 1400 1700 7d0a 7405 7c0f  ..........}.t.|.
-00001d70: 8301 6418 7406 6419 7407 7405 7c0f 8301  ..d.t.d.t.t.|...
-00001d80: 8301 1800 8301 1400 1700 7d0f 7405 7c10  ..........}.t.|.
-00001d90: 8301 6418 7406 6419 7407 7405 7c10 8301  ..d.t.d.t.t.|...
-00001da0: 8301 1800 8301 1400 1700 7d10 7405 7c28  ..........}.t.|(
-00001db0: 8301 6418 7406 6419 7407 7405 7c28 8301  ..d.t.d.t.t.|(..
-00001dc0: 8301 1800 8301 1400 1700 7d28 7405 7c0e  ..........}(t.|.
-00001dd0: 8301 6418 7406 6419 7407 7405 7c0e 8301  ..d.t.d.t.t.|...
-00001de0: 8301 1800 8301 1400 1700 7d0e 7405 7c29  ..........}.t.|)
-00001df0: 8301 6418 7406 6419 7407 7405 7c29 8301  ..d.t.d.t.t.|)..
-00001e00: 8301 1800 8301 1400 1700 7d29 7405 7c2a  ..........})t.|*
-00001e10: 8301 6418 7406 6419 7407 7405 7c2a 8301  ..d.t.d.t.t.|*..
-00001e20: 8301 1800 8301 1400 1700 7d2a 7405 7c2b  ..........}*t.|+
-00001e30: 8301 6418 7406 6419 7407 7405 7c2b 8301  ..d.t.d.t.t.|+..
-00001e40: 8301 1800 8301 1400 1700 7d2b 7405 7c2c  ..........}+t.|,
-00001e50: 8301 6418 7406 6419 7407 7405 7c2c 8301  ..d.t.d.t.t.|,..
-00001e60: 8301 1800 8301 1400 1700 7d2c 7405 7c2d  ..........},t.|-
-00001e70: 8301 6418 7406 6419 7407 7405 7c2d 8301  ..d.t.d.t.t.|-..
-00001e80: 8301 1800 8301 1400 1700 7d2d 7405 7c2e  ..........}-t.|.
-00001e90: 8301 6418 7406 6419 7407 7405 7c2e 8301  ..d.t.d.t.t.|...
-00001ea0: 8301 1800 8301 1400 1700 7d2e 7405 7c25  ..........}.t.|%
-00001eb0: 8301 6418 7406 6419 7407 7405 7c25 8301  ..d.t.d.t.t.|%..
-00001ec0: 8301 1800 8301 1400 1700 7d25 7405 7c0c  ..........}%t.|.
-00001ed0: 8301 6418 7406 6419 7407 7405 7c0c 8301  ..d.t.d.t.t.|...
-00001ee0: 8301 1800 8301 1400 1700 7d0c 7405 7c0b  ..........}.t.|.
-00001ef0: 8301 6418 7406 6419 7407 7405 7c0b 8301  ..d.t.d.t.t.|...
-00001f00: 8301 1800 8301 1400 1700 7d0b 7405 7c2f  ..........}.t.|/
-00001f10: 8301 6418 7406 6419 7407 7405 7c2f 8301  ..d.t.d.t.t.|/..
-00001f20: 8301 1800 8301 1400 1700 7d2f 7405 7c30  ..........}/t.|0
-00001f30: 8301 6418 7406 6419 7407 7405 7c30 8301  ..d.t.d.t.t.|0..
-00001f40: 8301 1800 8301 1400 1700 7d30 7405 7c31  ..........}0t.|1
-00001f50: 8301 6418 7406 6419 7407 7405 7c31 8301  ..d.t.d.t.t.|1..
-00001f60: 8301 1800 8301 1400 1700 7d31 7405 7c32  ..........}1t.|2
-00001f70: 8301 6418 7406 6419 7407 7405 7c32 8301  ..d.t.d.t.t.|2..
-00001f80: 8301 1800 8301 1400 1700 7d32 7405 7c33  ..........}2t.|3
-00001f90: 8301 6418 7406 6419 7407 7405 7c33 8301  ..d.t.d.t.t.|3..
-00001fa0: 8301 1800 8301 1400 1700 7d33 7405 7c34  ..........}3t.|4
-00001fb0: 8301 6418 7406 6419 7407 7405 7c34 8301  ..d.t.d.t.t.|4..
-00001fc0: 8301 1800 8301 1400 1700 7d34 7405 7c35  ..........}4t.|5
-00001fd0: 8301 6418 7406 6419 7407 7405 7c35 8301  ..d.t.d.t.t.|5..
-00001fe0: 8301 1800 8301 1400 1700 7d35 6430 7c00  ..........}5d0|.
-00001ff0: 9b00 647d 7c26 9b00 6458 7c06 9b00 6432  ..d}|&..dX|...d2
-00002000: 7c18 9b00 6433 7c08 9b00 6434 7c16 9b00  |...d3|...d4|...
-00002010: 6435 7c0a 9b00 647e 7c2a 9b00 647f 7c27  d5|...d~|*..d.|'
-00002020: 9b00 645e 7c1c 9b00 645f 7c28 9b00 6480  ..d^|...d_|(..d.
-00002030: 7c2b 9b00 6481 7c2e 9b00 6436 7c0e 9b00  |+..d.|...d6|...
-00002040: 645d 7c29 9b00 6438 7c0f 9b00 6439 7c10  d]|)..d8|...d9|.
-00002050: 9b00 6482 7c30 9b00 6483 7c31 9b00 6484  ..d.|0..d.|1..d.
-00002060: 7c32 9b00 6485 7c33 9b00 6486 7c34 9b00  |2..d.|3..d.|4..
-00002070: 6487 7c35 9b00 6466 7c25 9b00 6467 7c0b  d.|5..df|%..dg|.
-00002080: 9b00 6488 7c2f 9b00 643c 9d35 7d12 740f  ..d.|/..d<.5}.t.
-00002090: 7c12 8301 0100 7400 7c12 640f 1700 3700  |.....t.|.d...7.
-000020a0: 6100 5700 6e2c 0100 0100 0100 6430 7c00  a.W.n,......d0|.
-000020b0: 9b00 6489 9d03 7d12 740f 7c12 8301 0100  ..d...}.t.|.....
-000020c0: 7400 7c12 640f 1700 3700 6100 5900 6e02  t.|.d...7.a.Y.n.
-000020d0: 3000 6404 5300 298a 4e72 0f00 0000 7a28  0.d.S.).Nr....z(
-000020e0: 2020 2020 5b2b 5d20 5665 7269 6679 696e      [+] Verifyin
-000020f0: 6720 696e 7465 726e 6574 2063 6f6e 6e65  g internet conne
-00002100: 6374 696f 6e2e 2e2e 721d 0000 0054 7221  ction...r....Tr!
-00002110: 0000 007a 1668 7474 7073 3a2f 2f77 7777  ...z.https://www
-00002120: 2e67 6f6f 676c 652e 636f 6d7a 2820 2020  .google.comz(   
-00002130: 203e 2049 6e74 6572 6e65 7420 636f 6e6e   > Internet conn
-00002140: 6563 7469 6f6e 206e 6f74 2061 7661 696c  ection not avail
-00002150: 6162 6c65 2172 2600 0000 7a38 0a20 2020  able!r&...z8.   
-00002160: 201b 5b31 3b34 393b 3931 6d3e 2049 6e74   .[1;49;91m> Int
-00002170: 6572 6e65 7420 636f 6e6e 6563 7469 6f6e  ernet connection
-00002180: 206e 6f74 2061 7661 696c 6162 6c65 211b   not available!.
-00002190: 5b30 6d0a 4672 1b00 0000 721c 0000 007a  [0m.Fr....r....z
-000021a0: 3a20 2020 201b 5b31 3b34 393b 3933 6d5b  :    .[1;49;93m[
-000021b0: 235d 2052 6576 6572 7365 2069 7020 6164  #] Reverse ip ad
-000021c0: 6472 6573 7320 6c6f 6f6b 7570 2066 6f72  dress lookup for
-000021d0: 201b 5b31 3b34 393b 3936 6d72 2400 0000   .[1;49;96mr$...
-000021e0: 7225 0000 007a 245e 5c64 7b31 2c33 7d5c  r%...z$^\d{1,3}\
-000021f0: 2e5c 647b 312c 337d 5c2e 5c64 7b31 2c33  .\d{1,3}\.\d{1,3
-00002200: 7d5c 2e5c 647b 312c 337d 247a 3320 2020  }\.\d{1,3}$z3   
-00002210: 203e 2049 6e76 616c 6964 2069 7020 6164   > Invalid ip ad
-00002220: 6472 6573 7320 666f 726d 6174 2120 2845  dress format! (E
-00002230: 7861 6d70 6c65 3a20 382e 382e 382e 3829  xample: 8.8.8.8)
-00002240: 7228 0000 007a 4120 2020 1b5b 313b 3439  r(...zA   .[1;49
-00002250: 3b39 316d 3e20 496e 7661 6c69 6420 6970  ;91m> Invalid ip
-00002260: 2061 6464 7265 7373 2066 6f72 6d61 7421   address format!
-00002270: 2028 4578 616d 706c 653a 2038 2e38 2e38   (Example: 8.8.8
-00002280: 2e38 291b 5b30 6d0a 7a17 6874 7470 3a2f  .8).[0m.z.http:/
-00002290: 2f69 702d 6170 692e 636f 6d2f 6a73 6f6e  /ip-api.com/json
-000022a0: 2f7a 1168 7474 7073 3a2f 2f69 7061 7069  /z.https://ipapi
-000022b0: 2e63 6f2f 7a06 2f6a 736f 6e2f 7a10 6874  .co/z./json/z.ht
-000022c0: 7470 3a2f 2f69 7077 686f 2e69 732f 7230  tp://ipwho.is/r0
-000022d0: 0000 0072 3100 0000 fa0a 5573 6572 2d41  ...r1.....User-A
-000022e0: 6765 6e74 7a44 4d6f 7a69 6c6c 612f 352e  gentzDMozilla/5.
-000022f0: 3020 2858 3131 3b20 4c69 6e75 7820 7838  0 (X11; Linux x8
-00002300: 365f 3634 3b20 7276 3a38 392e 3029 2047  6_64; rv:89.0) G
-00002310: 6563 6b6f 2f32 3031 3030 3130 3120 4669  ecko/20100101 Fi
-00002320: 7265 666f 782f 3839 2e30 2903 7201 0000  refox/89.0).r...
-00002330: 0072 1e00 0000 e902 0000 0072 0100 0000  .r.........r....
-00002340: 7210 0000 0029 0272 1100 0000 da07 6865  r....).r......he
-00002350: 6164 6572 73e9 c800 0000 da06 7374 6174  aders.......stat
-00002360: 7573 da07 7375 6363 6573 7372 4600 0000  us..successrF...
-00002370: da0b 636f 756e 7472 7943 6f64 655a 0a72  ..countryCodeZ.r
-00002380: 6567 696f 6e4e 616d 65da 0672 6567 696f  egionName..regio
-00002390: 6eda 0463 6974 79da 0369 7370 da03 6f72  n..city..isp..or
-000023a0: 6772 1800 0000 da03 7a69 705a 036c 6174  gr......zipZ.lat
-000023b0: 5a03 6c6f 6eda 0571 7565 7279 7a20 7265  Z.lon..queryz re
-000023c0: 7665 7273 652d 6970 2d6c 6f6f 6b75 702d  verse-ip-lookup-
-000023d0: 7365 7276 6572 2d31 2d65 7272 6f72 75d2  server-1-erroru.
-000023e0: 0000 000a 2020 2020 e294 8ce2 9480 e294  ....    ........
-000023f0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00002400: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00002410: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00002420: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00002430: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00002440: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00002450: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00002460: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00002470: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00002480: 80e2 9480 e294 80e2 9480 e294 80e2 9490  ................
-00002490: 0a20 2020 207c 2053 6361 6e6e 6564 2049  .    | Scanned I
-000024a0: 5020 4164 6472 6573 733a 201b 5b31 3b34  P Address: .[1;4
-000024b0: 393b 3936 6d61 3501 0000 1b5b 306d 2020  9;96ma5....[0m  
-000024c0: 207c 0a20 2020 207c 2053 6572 7665 7220   |.    | Server 
-000024d0: 636f 6465 206e 616d 6520 203a 201b 5b31  code name  : .[1
-000024e0: 3b34 393b 3936 6d72 6576 6572 7365 2d69  ;49;96mreverse-i
-000024f0: 702d 6c6f 6f6b 7570 2d73 6572 7665 722d  p-lookup-server-
-00002500: 311b 5b30 6d20 2020 2020 2020 7c0a 2020  1.[0m       |.  
-00002510: 2020 7c2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d    |-------------
-00002520: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000070: 6401 6c08 5a08 6400 6401 6c09 5a09 6400  d.l.Z.d.d.l.Z.d.
+00000080: 6401 6c0a 5a0a 6400 6401 6c0b 5a0b 6400  d.l.Z.d.d.l.Z.d.
+00000090: 6402 6c0c 6d0d 5a0d 0100 6400 6401 6c0e  d.l.m.Z...d.d.l.
+000000a0: 5a0e 6400 6401 6c0f 5a10 6700 6403 a201  Z.d.d.l.Z.g.d...
+000000b0: 0400 5a11 5a12 6404 6113 6404 6114 6405  ..Z.Z.d.a.d.a.d.
+000000c0: 6115 6406 6407 8400 5a16 6408 6409 8400  a.d.d...Z.d.d...
+000000d0: 5a17 640a 640b 8400 5a18 640c 640d 8400  Z.d.d...Z.d.d...
+000000e0: 5a19 640e 640f 8400 5a1a 6410 6411 8400  Z.d.d...Z.d.d...
+000000f0: 5a1b 6404 6405 6405 6405 6405 6700 6412  Z.d.d.d.d.d.g.d.
+00000100: a201 6404 6404 6405 6405 6405 660b 6413  ..d.d.d.d.d.f.d.
+00000110: 6414 8401 5a1c 6415 6416 8400 5a1d 6417  d...Z.d.d...Z.d.
+00000120: 6418 8400 5a1e 6419 641a 8400 5a1f 641b  d...Z.d.d...Z.d.
+00000130: 641c 8400 5a20 641d 641e 8400 5a21 641f  d...Z d.d...Z!d.
+00000140: 6420 8400 5a22 6401 5300 2921 e900 0000  d ..Z"d.S.)!....
+00000150: 004e 2901 da09 4d61 634c 6f6f 6b75 7029  .N)...MacLookup)
+00000160: 10da 0663 6861 6e67 65da 0563 6865 636b  ...change..check
+00000170: da05 636c 6561 72da 0464 6f72 6bda 0364  ..clear..dork..d
+00000180: 6e73 da04 6578 6974 da03 6578 70da 0468  ns..exit..exp..h
+00000190: 656c 70da 0469 6e66 6fda 0269 70da 036d  elp..info..ip..m
+000001a0: 6163 da06 6e75 6d62 6572 da04 7175 6974  ac..number..quit
+000001b0: da04 7361 7665 da05 7368 656c 6cda 0577  ..save..shell..w
+000001c0: 686f 6973 da00 4663 0000 0000 0000 0000  hois..Fc........
+000001d0: 0000 0000 0100 0000 0600 0000 4300 0000  ............C...
+000001e0: 7336 0000 0064 0164 0267 027d 007a 1a74  s6...d.d.g.}.z.t
+000001f0: 006a 0174 02a0 037c 00a1 0164 0364 048d  .j.t...|...d.d..
+00000200: 0201 0057 0064 0553 0001 0001 0001 0059  ...W.d.S.......Y
+00000210: 0064 0653 0030 0064 0053 0029 074e 7a12  .d.S.0.d.S.).Nz.
+00000220: 6874 7470 733a 2f2f 676f 6f67 6c65 2e63  https://google.c
+00000230: 6f6d 7a10 6874 7470 733a 2f2f 6269 6e67  omz.https://bing
+00000240: 2e63 6f6d e90a 0000 0029 01da 0774 696d  .com.....)...tim
+00000250: 656f 7574 5446 2904 da08 7265 7175 6573  eoutTF)...reques
+00000260: 7473 da03 6765 74da 0672 616e 646f 6dda  ts..get..random.
+00000270: 0663 686f 6963 6529 01da 0475 726c 73a9  .choice)...urls.
+00000280: 0072 1b00 0000 fa3a 6275 696c 642f 6264  .r.....:build/bd
+00000290: 6973 742e 6c69 6e75 782d 7838 365f 3634  ist.linux-x86_64
+000002a0: 2f65 6767 2f70 686f 6d62 6572 2f70 686f  /egg/phomber/pho
+000002b0: 6d62 6572 7633 2e30 2e32 5f62 6574 612e  mberv3.0.2_beta.
+000002c0: 7079 da10 6368 6563 6b5f 636f 6e6e 6563  py..check_connec
+000002d0: 7469 6f6e 3a00 0000 730c 0000 0000 0208  tion:...s.......
+000002e0: 0102 0114 0106 0106 0172 1d00 0000 6301  .........r....c.
+000002f0: 0000 0000 0000 0000 0000 0014 0000 0017  ................
+00000300: 0000 0043 0000 0073 6c04 0000 6401 6402  ...C...sl...d.d.
+00000310: 6c00 6d01 7d01 0100 6401 6403 6c00 6d02  l.m.}...d.d.l.m.
+00000320: 7d02 0100 6401 6404 6c00 6d03 7d03 0100  }...d.d.l.m.}...
+00000330: 6405 6104 7405 6406 7c00 9b00 6407 9d03  d.a.t.d.|...d...
+00000340: 6700 6408 a201 6409 640a 8d03 0100 7404  g.d...d.d.....t.
+00000350: 640b 7c00 9b00 640c 9d03 640d 1700 3700  d.|...d...d...7.
+00000360: 6104 7406 a007 640e 7c00 a102 7376 7405  a.t...d.|...svt.
+00000370: 640f 6700 6410 a201 6411 8d02 0100 6412  d.g.d...d.....d.
+00000380: 5300 7a0e 7400 a008 7c00 a101 7d04 5700  S.z.t...|...}.W.
+00000390: 6e28 0400 7400 6a09 6a0a 79ac 0100 0100  n(..t.j.j.y.....
+000003a0: 0100 7405 6413 6700 6410 a201 6411 8d02  ..t.d.g.d...d...
+000003b0: 0100 5900 6412 5300 3000 740b 7c04 8301  ..Y.d.S.0.t.|...
+000003c0: a00c 6414 6415 a102 6415 1900 a00c 6416  ..d.d...d.....d.
+000003d0: 6415 a102 6401 1900 a00d a100 7d05 740b  d...d.......}.t.
+000003e0: 7c04 8301 a00c 6414 6415 a102 6415 1900  |.....d.d...d...
+000003f0: a00c 6416 6415 a102 6415 1900 a00d a100  ..d.d...d.......
+00000400: 7d06 7400 a00e 7c04 a101 7d07 7400 a00f  }.t...|...}.t...
+00000410: 7c04 a101 7d08 7c07 9003 72d8 7c08 9003  |...}.|...r.|...
+00000420: 72d8 7400 a008 7c00 6417 a102 7d09 7400  r.t...|.d...}.t.
+00000430: a010 7c04 a101 7d0a 7c03 a011 7c09 6418  ..|...}.|...|.d.
+00000440: a102 7d0b 7400 a008 7c00 6419 a102 7d0c  ..}.t...|.d...}.
+00000450: 7c02 a012 7c0c 6418 a102 7d0d 740b 7c01  |...|.d...}.t.|.
+00000460: a013 7c04 a101 8301 7d0e 7c0e a014 641a  ..|.....}.|...d.
+00000470: 6405 a102 a014 641b 6405 a102 a014 641c  d.....d.d.....d.
+00000480: 6405 a102 a014 641d 6405 a102 a014 641e  d.....d.d.....d.
+00000490: 6405 a102 a014 641f 6405 a102 a014 6420  d.....d.d.....d 
+000004a0: 6405 a102 7d0f 7400 a015 7c04 7400 6a16  d...}.t...|.t.j.
+000004b0: 6a17 a102 a014 6421 6405 a102 7d10 740b  j.....d!d...}.t.
+000004c0: 7c08 8301 6420 7418 6422 7419 740b 7c08  |...d t.d"t.t.|.
+000004d0: 8301 8301 1800 8301 1400 1700 7d08 740b  ............}.t.
+000004e0: 7c07 8301 6420 7418 6422 7419 740b 7c07  |...d t.d"t.t.|.
+000004f0: 8301 8301 1800 8301 1400 1700 7d07 740b  ............}.t.
+00000500: 7c05 8301 6420 7418 6422 7419 740b 7c05  |...d t.d"t.t.|.
+00000510: 8301 8301 1800 8301 1400 1700 7d05 740b  ............}.t.
+00000520: 7c0b 8301 6420 7418 6422 7419 740b 7c0b  |...d t.d"t.t.|.
+00000530: 8301 8301 1800 8301 1400 1700 7d0b 740b  ............}.t.
+00000540: 7c0a 8301 6420 7418 6422 7419 740b 7c0a  |...d t.d"t.t.|.
+00000550: 8301 8301 1800 8301 1400 1700 7d0a 740b  ............}.t.
+00000560: 7c0d 8301 6420 7418 6422 7419 740b 7c0d  |...d t.d"t.t.|.
+00000570: 8301 8301 1800 8301 1400 1700 7d0d 740b  ............}.t.
+00000580: 7c0f 8301 6420 7418 6422 7419 740b 7c0f  |...d t.d"t.t.|.
+00000590: 8301 8301 1800 8301 1400 1700 7d0f 740b  ............}.t.
+000005a0: 7c00 8301 6420 7418 6422 7419 740b 7c00  |...d t.d"t.t.|.
+000005b0: 8301 8301 1800 8301 1400 1700 7d00 740b  ............}.t.
+000005c0: 7c06 8301 6420 7418 6422 7419 740b 7c06  |...d t.d"t.t.|.
+000005d0: 8301 8301 1800 8301 1400 1700 7d06 740b  ............}.t.
+000005e0: 7c10 8301 6420 7418 6422 7419 740b 7c10  |...d t.d"t.t.|.
+000005f0: 8301 8301 1800 8301 1400 1700 7d10 6423  ............}.d#
+00000600: 7c00 9b00 6424 7c08 9b00 6425 7c07 9b00  |...d$|...d%|...
+00000610: 6426 7c05 9b00 6427 7c0b 9b00 6428 7c0a  d&|...d'|...d(|.
+00000620: 9b00 6429 7c0d 9b00 642a 7c0f 9b00 642b  ..d)|...d*|...d+
+00000630: 7c00 9b00 642c 7c06 9b00 642d 7c10 9b00  |...d,|...d-|...
+00000640: 642e 9d17 7d11 741a 7c11 8301 0100 7404  d...}.t.|.....t.
+00000650: 7c11 642f 1700 3700 6104 6430 7c00 a00d  |.d/..7.a.d0|...
+00000660: a100 9b00 6431 7c0a a00d a100 9b00 6432  ....d1|.......d2
+00000670: 7c06 a00d a100 9b00 6433 7c0a a00d a100  |.......d3|.....
+00000680: a01b a100 9b00 6432 7c06 a00d a100 9b00  ......d2|.......
+00000690: 6434 9d0b 7d12 741a 7c12 8301 0100 7404  d4..}.t.|.....t.
+000006a0: 7c12 642f 1700 3700 6104 6435 7c06 a00d  |.d/..7.a.d5|...
+000006b0: a100 9b00 6434 9d03 7d13 741a 7c13 8301  ....d4..}.t.|...
+000006c0: 0100 7404 7c13 642f 1700 3700 6104 7405  ..t.|.d/..7.a.t.
+000006d0: 6436 6700 6408 a201 6409 640a 8d03 0100  d6g.d...d.d.....
+000006e0: 6409 5300 740b 7c08 8301 6420 7418 6422  d.S.t.|...d t.d"
+000006f0: 7419 740b 7c08 8301 8301 1800 8301 1400  t.t.|...........
+00000700: 1700 7d08 740b 7c07 8301 6420 7418 6422  ..}.t.|...d t.d"
+00000710: 7419 740b 7c07 8301 8301 1800 8301 1400  t.t.|...........
+00000720: 1700 7d07 740b 7c00 8301 6420 7418 6422  ..}.t.|...d t.d"
+00000730: 7419 740b 7c00 8301 8301 1800 8301 1400  t.t.|...........
+00000740: 1700 7d00 6423 7c00 9b00 6424 7c08 9b00  ..}.d#|...d$|...
+00000750: 6425 7c07 9b00 642e 9d07 7d11 741a 7c11  d%|...d...}.t.|.
+00000760: 8301 0100 7404 7c11 642f 1700 3700 6104  ....t.|.d/..7.a.
+00000770: 6412 5300 6400 5300 2937 4e72 0100 0000  d.S.d.S.)7Nr....
+00000780: 2901 da08 7469 6d65 7a6f 6e65 2901 da07  )...timezone)...
+00000790: 6361 7272 6965 7229 01da 0867 656f 636f  carrier)...geoco
+000007a0: 6465 7272 1300 0000 fa2f 2020 2020 5b2b  derr...../    [+
+000007b0: 5d20 4772 6174 6865 7269 6e67 2069 6e66  ] Grathering inf
+000007c0: 6f72 6d61 7469 6f6e 2061 626f 7574 201b  ormation about .
+000007d0: 5b31 3b34 393b 3936 6dfa 0d1b 5b31 3b34  [1;49;96m...[1;4
+000007e0: 393b 3933 6d2e 2e2e a903 e901 0000 00e9  9;93m...........
+000007f0: 3100 0000 e95d 0000 0054 a902 da06 636f  1....]...T....co
+00000800: 6c65 6474 da0a 7370 6163 655f 646f 776e  ledt..space_down
+00000810: 7a3d 0a20 2020 201b 5b31 3b34 393b 3933  z=.    .[1;49;93
+00000820: 6d5b 235d 2052 6576 6572 7365 2070 686f  m[#] Reverse pho
+00000830: 6e65 206e 756d 6265 7220 6c6f 6f6b 7570  ne number lookup
+00000840: 2066 6f72 201b 5b31 3b34 393b 3936 6dfa   for .[1;49;96m.
+00000850: 0f1b 5b31 3b34 393b 3933 6d3a 1b5b 306d  ..[1;49;93m:.[0m
+00000860: fa02 0a0a 7a11 5e5c 2b5b 312d 395d 5c64  ....z.^\+[1-9]\d
+00000870: 7b31 2c31 347d 247a 3b20 2020 203e 2049  {1,14}$z;    > I
+00000880: 6e76 616c 6964 2070 686f 6e65 206e 756d  nvalid phone num
+00000890: 6265 7220 666f 726d 6174 2120 2845 7861  ber format! (Exa
+000008a0: 6d70 6c65 3a20 2b34 3478 7878 7878 7878  mple: +44xxxxxxx
+000008b0: 7878 7829 a903 7224 0000 0072 2500 0000  xxx)..r$...r%...
+000008c0: e95b 0000 00a9 0172 2800 0000 467a 3320  .[.....r(...Fz3 
+000008d0: 2020 203e 204d 6973 7369 6e67 2043 6f75     > Missing Cou
+000008e0: 6e74 7279 2043 6f64 6521 2028 4578 616d  ntry Code! (Exam
+000008f0: 706c 653a 202b 3931 2c20 2b34 342c 202b  ple: +91, +44, +
+00000900: 3129 7a0d 436f 756e 7472 7920 436f 6465  1)z.Country Code
+00000910: 3a72 2400 0000 7a10 4e61 7469 6f6e 616c  :r$...z.National
+00000920: 204e 756d 6265 723a 5a02 4348 da02 656e   Number:Z.CH..en
+00000930: 5a02 524f fa01 5bfa 015d fa01 27fa 0128  Z.RO..[..]..'..(
+00000940: fa01 29fa 012c fa01 207a 0474 656c 3ae9  ..)..,.. z.tel:.
+00000950: 1e00 0000 75d4 0000 000a 2020 2020 e294  ....u.....    ..
+00000960: 8ce2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00000970: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00000980: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00000990: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+000009a0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+000009b0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+000009c0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+000009d0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+000009e0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+000009f0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00000a00: e294 80e2 9490 0a20 2020 207c 2053 6361  .......    | Sca
+00000a10: 6e6e 6564 2050 686f 6e65 204e 756d 6265  nned Phone Numbe
+00000a20: 723a 201b 5b31 3b34 393b 3936 6d7a e81b  r: .[1;49;96mz..
+00000a30: 5b30 6d20 7c0a 2020 2020 7c2d 2d2d 2d2d  [0m |.    |-----
+00000a40: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000a50: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000a60: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000a70: 2d7c 0a20 2020 207c 2049 4e46 4f52 4d41  -|.    | INFORMA
+00000a80: 5449 4f4e 2020 2020 2020 2020 207c 2044  TION         | D
+00000a90: 4553 4352 4950 5449 4f4e 2020 2020 2020  ESCRIPTION      
+00000aa0: 2020 2020 2020 2020 2020 2020 2020 7c0a                |.
+00000ab0: 2020 2020 7c2d 2d2d 2d2d 2d2d 2d2d 2d2d      |-----------
+00000ac0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000ad0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000ae0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d7c 0a20 2020  -----------|.   
+00000af0: 207c 201b 5b31 3b34 393b 3937 6d50 6f73   | .[1;49;97mPos
+00000b00: 7369 626c 651b 5b30 6d20 2020 2020 2020  sible.[0m       
+00000b10: 2020 2020 207c 207a 2d20 7c0a 2020 2020       | z- |.    
+00000b20: 7c20 1b5b 313b 3439 3b39 376d 5661 6c69  | .[1;49;97mVali
+00000b30: 641b 5b30 6d20 2020 2020 2020 2020 2020  d.[0m           
+00000b40: 2020 2020 7c20 7a6a 207c 0a20 2020 207c      | zj |.    |
+00000b50: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000b60: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000b70: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000b80: 2d2d 2d2d 2d2d 7c0a 2020 2020 7c20 1b5b  ------|.    | .[
+00000b90: 313b 3439 3b39 376d 436f 756e 7472 7920  1;49;97mCountry 
+00000ba0: 436f 6465 1b5b 306d 2020 2020 2020 2020  Code.[0m        
+00000bb0: 7c20 7a2d 207c 0a20 2020 207c 201b 5b31  | z- |.    | .[1
+00000bc0: 3b34 393b 3937 6d43 6f75 6e74 7279 1b5b  ;49;97mCountry.[
+00000bd0: 306d 2020 2020 2020 2020 2020 2020 207c  0m             |
+00000be0: 20fa 2d20 7c0a 2020 2020 7c20 1b5b 313b   .- |.    | .[1;
+00000bf0: 3439 3b39 376d 5265 6769 6f6e 2043 6f64  49;97mRegion Cod
+00000c00: 651b 5b30 6d20 2020 2020 2020 2020 7c20  e.[0m         | 
+00000c10: 7a2d 207c 0a20 2020 207c 201b 5b31 3b34  z- |.    | .[1;4
+00000c20: 393b 3937 6d53 6572 7669 6365 2050 726f  9;97mService Pro
+00000c30: 7669 6465 721b 5b30 6d20 2020 207c 20fa  vider.[0m    | .
+00000c40: 2d20 7c0a 2020 2020 7c20 1b5b 313b 3439  - |.    | .[1;49
+00000c50: 3b39 376d 5469 6d65 7a6f 6e65 1b5b 306d  ;97mTimezone.[0m
+00000c60: 2020 2020 2020 2020 2020 2020 7c20 7a6a              | zj
+00000c70: 207c 0a20 2020 207c 2d2d 2d2d 2d2d 2d2d   |.    |--------
+00000c80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000c90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000ca0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 7c0a  --------------|.
+00000cb0: 2020 2020 7c20 1b5b 313b 3439 3b39 376d      | .[1;49;97m
+00000cc0: 496e 7465 726e 6174 696f 6e61 6c20 466f  International Fo
+00000cd0: 726d 6174 1b5b 306d 7c20 7a2d 207c 0a20  rmat.[0m| z- |. 
+00000ce0: 2020 207c 201b 5b31 3b34 393b 3937 6d4e     | .[1;49;97mN
+00000cf0: 6174 696f 6e61 6c20 466f 726d 6174 1b5b  ational Format.[
+00000d00: 306d 2020 2020 207c 207a 2d20 7c0a 2020  0m     | z- |.  
+00000d10: 2020 7c20 1b5b 313b 3439 3b39 376d 5246    | .[1;49;97mRF
+00000d20: 4333 3936 3620 466f 726d 6174 1b5b 306d  C3966 Format.[0m
+00000d30: 2020 2020 2020 7c20 75b8 0000 0020 7c0a        | u.... |.
+00000d40: 2020 2020 e294 94e2 9480 e294 80e2 9480      ............
+00000d50: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00000d60: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00000d70: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00000d80: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00000d90: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00000da0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00000db0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00000dc0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00000dd0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00000de0: e294 80e2 9480 e294 80e2 9498 0a20 2020  .............   
+00000df0: 2020 2020 20da 010a 7a2b 0a20 2020 201b       ...z+.    .
+00000e00: 5b31 3b34 393b 3933 6d5b 2b5d 2053 6561  [1;49;93m[+] Sea
+00000e10: 7263 6869 6e67 2066 6f72 201b 5b31 3b34  rching for .[1;4
+00000e20: 393b 3936 6d7a 741b 5b31 3b34 393b 3933  9;96mzt.[1;49;93
+00000e30: 6d20 6f6e 2076 6172 696f 7573 2070 6c61  m on various pla
+00000e40: 7466 6f72 6d73 3a0a 0a20 2020 201b 5b31  tforms:..    .[1
+00000e50: 3b34 393b 3932 6d3e 2068 7474 7073 3a2f  ;49;92m> https:/
+00000e60: 2f77 7777 2e69 7071 7561 6c69 7479 7363  /www.ipqualitysc
+00000e70: 6f72 652e 636f 6d2f 7265 7665 7273 652d  ore.com/reverse-
+00000e80: 7068 6f6e 652d 6e75 6d62 6572 2d6c 6f6f  phone-number-loo
+00000e90: 6b75 702f 6c6f 6f6b 7570 2ffa 012f 7a29  kup/lookup/../z)
+00000ea0: 0a20 2020 203e 2068 7474 7073 3a2f 2f77  .    > https://w
+00000eb0: 7777 2e74 7275 6563 616c 6c65 722e 636f  ww.truecaller.co
+00000ec0: 6d2f 7365 6172 6368 2f7a 090a 2020 2020  m/search/z..    
+00000ed0: 1b5b 306d 7a59 0a20 2020 201b 5b31 3b34  .[0mzY.    .[1;4
+00000ee0: 393b 3933 6d5b 2b5d 2047 6f6f 676c 6520  9;93m[+] Google 
+00000ef0: 446f 726b 2051 7565 7269 6573 3a0a 0a20  Dork Queries:.. 
+00000f00: 2020 201b 5b31 3b34 393b 3932 6d3e 2068     .[1;49;92m> h
+00000f10: 7474 7073 3a2f 2f77 7777 2e67 6f6f 676c  ttps://www.googl
+00000f20: 652e 636f 6d2f 7365 6172 6368 3f71 3d7a  e.com/search?q=z
+00000f30: 2820 2020 205b 2b5d 2053 6361 6e6e 696e  (    [+] Scannin
+00000f40: 6720 736f 6369 616c 206d 6564 6961 2070  g social media p
+00000f50: 6c61 7466 6f72 6d73 3a29 1cda 0c70 686f  latforms:)...pho
+00000f60: 6e65 6e75 6d62 6572 7372 1e00 0000 721f  nenumbersr....r.
+00000f70: 0000 0072 2000 0000 da06 7072 765f 6f70  ...r .....prv_op
+00000f80: da07 7072 696e 7469 74da 0272 65da 056d  ..printit..re..m
+00000f90: 6174 6368 da05 7061 7273 655a 0f70 686f  atch..parseZ.pho
+00000fa0: 6e65 6e75 6d62 6572 7574 696c 5a14 4e75  nenumberutilZ.Nu
+00000fb0: 6d62 6572 5061 7273 6545 7863 6570 7469  mberParseExcepti
+00000fc0: 6f6e da03 7374 72da 0573 706c 6974 da05  on..str..split..
+00000fd0: 7374 7269 705a 0f69 735f 7661 6c69 645f  stripZ.is_valid_
+00000fe0: 6e75 6d62 6572 5a12 6973 5f70 6f73 7369  numberZ.is_possi
+00000ff0: 626c 655f 6e75 6d62 6572 5a16 7265 6769  ble_numberZ.regi
+00001000: 6f6e 5f63 6f64 655f 666f 725f 6e75 6d62  on_code_for_numb
+00001010: 6572 5a16 6465 7363 7269 7074 696f 6e5f  erZ.description_
+00001020: 666f 725f 6e75 6d62 6572 5a0f 6e61 6d65  for_numberZ.name
+00001030: 5f66 6f72 5f6e 756d 6265 725a 1574 696d  _for_numberZ.tim
+00001040: 655f 7a6f 6e65 735f 666f 725f 6e75 6d62  e_zones_for_numb
+00001050: 6572 da07 7265 706c 6163 655a 0d66 6f72  er..replaceZ.for
+00001060: 6d61 745f 6e75 6d62 6572 5a11 5068 6f6e  mat_numberZ.Phon
+00001070: 654e 756d 6265 7246 6f72 6d61 745a 0752  eNumberFormatZ.R
+00001080: 4643 3339 3636 da03 696e 74da 036c 656e  FC3966..int..len
+00001090: da05 7072 696e 74da 056c 6f77 6572 2914  ..print..lower).
+000010a0: 5a0c 7068 6f6e 655f 6e75 6d62 6572 721e  Z.phone_numberr.
+000010b0: 0000 0072 1f00 0000 7220 0000 005a 1470  ...r....r ...Z.p
+000010c0: 686f 6e65 5f6e 756d 6265 725f 6465 7461  hone_number_deta
+000010d0: 696c 73da 0c63 6f75 6e74 7279 5f63 6f64  ils..country_cod
+000010e0: 655a 0b6f 6e6c 795f 6e75 6d62 6572 5a05  eZ.only_numberZ.
+000010f0: 7661 6c69 64da 0870 6f73 7369 626c 655a  valid..possibleZ
+00001100: 0e63 6f75 6e72 7479 5f6e 756d 6265 72da  .counrty_number.
+00001110: 0b72 6567 696f 6e5f 636f 6465 da07 636f  .region_code..co
+00001120: 756e 7472 795a 0e73 6572 7669 6365 5f6e  untryZ.service_n
+00001130: 756d 6265 725a 1073 6572 7669 6365 5f70  umberZ.service_p
+00001140: 726f 7669 6465 725a 1b74 696d 657a 6f6e  roviderZ.timezon
+00001150: 655f 6465 7461 696c 735f 756e 6669 6c74  e_details_unfilt
+00001160: 6572 6564 5a10 7469 6d65 7a6f 6e65 5f64  eredZ.timezone_d
+00001170: 6574 6169 6c73 5a08 725f 666f 726d 6174  etailsZ.r_format
+00001180: da0c 6669 6e61 6c5f 6f75 7470 7574 5a12  ..final_outputZ.
+00001190: 6f6e 6c69 6e65 5f66 7265 655f 6c6f 6f6b  online_free_look
+000011a0: 7570 5a13 676f 6f67 6c65 5f64 6f72 6b5f  upZ.google_dork_
+000011b0: 7175 6572 6965 7372 1b00 0000 721b 0000  queriesr....r...
+000011c0: 0072 1c00 0000 da0d 6e75 6d62 6572 5f6c  .r......number_l
+000011d0: 6f6f 6b75 7044 0000 0073 be00 0000 0002  ookupD...s......
+000011e0: 0c01 0c01 0c04 0403 1a01 1403 0c01 1001  ................
+000011f0: 0403 0202 0e01 1001 1001 0803 2401 2403  ............$.$.
+00001200: 0a03 0a02 0c02 0c03 0a03 0c03 0c03 0c03  ................
+00001210: 0e01 3c03 1803 2001 2001 2001 2001 2001  ..<... . . . . .
+00001220: 2001 2001 2001 2001 2003 0202 02fe 0406   . . . . .......
+00001230: 02fa 0407 02f9 0409 02f7 040a 02f6 040b  ................
+00001240: 02f5 040c 02f4 040d 02f3 0402 02fe 0410  ................
+00001250: 02f0 0411 02ef 0814 0801 0c03 0201 06ff  ................
+00001260: 0403 06fd 0403 06fd 0404 0afc 0403 06fd  ................
+00001270: 0806 0801 0c03 0203 06fd 0805 0801 0c03  ................
+00001280: 1202 0404 2001 2001 2002 0202 02fe 0406  .... . . .......
+00001290: 02fa 0407 02f9 080a 0801 0c01 724f 0000  ............rO..
+000012a0: 0063 0100 0000 0000 0000 0000 0000 3600  .c............6.
+000012b0: 0000 3700 0000 4300 0000 7316 0f00 0064  ..7...C...s....d
+000012c0: 0161 0074 0164 0267 0064 03a2 0164 0464  .a.t.d.g.d...d.d
+000012d0: 058d 0301 0074 0283 0073 3274 0164 0667  .....t...s2t.d.g
+000012e0: 0064 07a2 0164 0464 058d 0301 0064 0853  .d...d.d.....d.S
+000012f0: 0074 0164 097c 009b 0064 0a9d 0367 0064  .t.d.|...d...g.d
+00001300: 03a2 0164 0464 058d 0301 0074 0064 0b7c  ...d.d.....t.d.|
+00001310: 009b 0064 0c9d 0364 0d17 0037 0061 0074  ...d...d...7.a.t
+00001320: 03a0 0464 0e7c 00a1 0273 8074 0164 0f67  ...d.|...s.t.d.g
+00001330: 0064 07a2 0164 108d 0201 0064 0853 0064  .d...d.....d.S.d
+00001340: 117c 009b 009d 0264 127c 009b 0064 139d  .|.....d.|...d..
+00001350: 0364 147c 009b 009d 0267 037d 0174 057c  .d.|.....g.}.t.|
+00001360: 0083 0164 1574 0664 1674 0774 057c 0083  ...d.t.d.t.t.|..
+00001370: 0183 0118 0083 0114 0017 007d 0064 1764  ...........}.d.d
+00001380: 1869 017d 0274 08a0 0967 0064 19a2 01a1  .i.}.t...g.d....
+00001390: 017d 037c 0364 1a6b 0290 0372 ba90 027a  .}.|.d.k...r...z
+000013a0: 8674 0a6a 0b7c 0164 1a19 0064 1b7c 0264  .t.j.|.d...d.|.d
+000013b0: 1c8d 037d 047c 04a0 0ca1 007d 057c 046a  ...}.|.....}.|.j
+000013c0: 0d64 1d6b 0290 0172 7a7c 0564 1e19 0064  .d.k...rz|.d...d
+000013d0: 1f6b 0290 0172 7a7c 0564 2019 007d 067c  .k...rz|.d ..}.|
+000013e0: 0564 2119 007d 077c 0564 2219 007d 087c  .d!..}.|.d"..}.|
+000013f0: 0564 2319 007d 097c 0564 2419 007d 0a7c  .d#..}.|.d$..}.|
+00001400: 0564 2519 007d 0b7c 0564 2619 007d 0c7c  .d%..}.|.d&..}.|
+00001410: 0564 2719 007d 0d7c 0564 2819 007d 0e7c  .d'..}.|.d(..}.|
+00001420: 0564 2919 007d 0f7c 0564 2a19 007d 107c  .d)..}.|.d*..}.|
+00001430: 0564 2b19 007d 116e 0874 0e64 2c83 0182  .d+..}.n.t.d,...
+00001440: 0174 057c 0683 0164 1574 0664 1674 0774  .t.|...d.t.d.t.t
+00001450: 057c 0683 0183 0118 0083 0114 0017 007d  .|.............}
+00001460: 0674 057c 0783 0164 1574 0664 1674 0774  .t.|...d.t.d.t.t
+00001470: 057c 0783 0183 0118 0083 0114 0017 007d  .|.............}
+00001480: 0774 057c 0883 0164 1574 0664 1674 0774  .t.|...d.t.d.t.t
+00001490: 057c 0883 0183 0118 0083 0114 0017 007d  .|.............}
+000014a0: 0874 057c 0983 0164 1574 0664 1674 0774  .t.|...d.t.d.t.t
+000014b0: 057c 0983 0183 0118 0083 0114 0017 007d  .|.............}
+000014c0: 0974 057c 0a83 0164 1574 0664 1674 0774  .t.|...d.t.d.t.t
+000014d0: 057c 0a83 0183 0118 0083 0114 0017 007d  .|.............}
+000014e0: 0a74 057c 0b83 0164 1574 0664 1674 0774  .t.|...d.t.d.t.t
+000014f0: 057c 0b83 0183 0118 0083 0114 0017 007d  .|.............}
+00001500: 0b74 057c 0c83 0164 1574 0664 1674 0774  .t.|...d.t.d.t.t
+00001510: 057c 0c83 0183 0118 0083 0114 0017 007d  .|.............}
+00001520: 0c74 057c 0d83 0164 1574 0664 1674 0774  .t.|...d.t.d.t.t
+00001530: 057c 0d83 0183 0118 0083 0114 0017 007d  .|.............}
+00001540: 0d74 057c 0e83 0164 1574 0664 1674 0774  .t.|...d.t.d.t.t
+00001550: 057c 0e83 0183 0118 0083 0114 0017 007d  .|.............}
+00001560: 0e74 057c 0f83 0164 1574 0664 1674 0774  .t.|...d.t.d.t.t
+00001570: 057c 0f83 0183 0118 0083 0114 0017 007d  .|.............}
+00001580: 0f74 057c 1083 0164 1574 0664 1674 0774  .t.|...d.t.d.t.t
+00001590: 057c 1083 0183 0118 0083 0114 0017 007d  .|.............}
+000015a0: 1074 057c 1183 0164 1574 0664 1674 0774  .t.|...d.t.d.t.t
+000015b0: 057c 1183 0183 0118 0083 0114 0017 007d  .|.............}
+000015c0: 1164 2d7c 009b 0064 2e7c 069b 0064 2f7c  .d-|...d.|...d/|
+000015d0: 079b 0064 307c 089b 0064 317c 099b 0064  ...d0|...d1|...d
+000015e0: 327c 0a9b 0064 337c 0e9b 0064 347c 0d9b  2|...d3|...d4|..
+000015f0: 0064 357c 0f9b 0064 367c 109b 0064 377c  .d5|...d6|...d7|
+00001600: 0b9b 0064 387c 0c9b 0064 399d 197d 1274  ...d8|...d9..}.t
+00001610: 0f7c 1283 0101 0074 007c 1264 3a17 0037  .|.....t.|.d:..7
+00001620: 0061 0057 006e 4e04 0074 0e90 0379 b401  .a.W.nN..t...y..
+00001630: 007d 1301 007a 3474 0f7c 1383 0101 0064  .}...z4t.|.....d
+00001640: 2d7c 009b 0064 3b9d 037d 1274 0f7c 1283  -|...d;..}.t.|..
+00001650: 0101 0074 007c 1264 3a17 0037 0061 0057  ...t.|.d:..7.a.W
+00001660: 0059 0064 007d 137e 136e 0a64 007d 137e  .Y.d.}.~.n.d.}.~
+00001670: 1330 0030 0090 0b6e 587c 0364 3c6b 0290  .0.0...nX|.d<k..
+00001680: 0972 2290 057a 2a74 0a6a 0b7c 0164 3c19  .r"..z*t.j.|.d<.
+00001690: 0064 1b7c 0264 1c8d 037d 047c 04a0 0ca1  .d.|.d...}.|....
+000016a0: 007d 057c 046a 0d64 1d6b 0290 0472 ca7c  .}.|.j.d.k...r.|
+000016b0: 0564 3d19 007d 117c 0564 3e19 007d 147c  .d=..}.|.d>..}.|
+000016c0: 0564 3f19 007d 157c 0564 2419 007d 0a7c  .d?..}.|.d$..}.|
+000016d0: 0564 2319 007d 087c 0564 4019 007d 167c  .d#..}.|.d@..}.|
+000016e0: 0564 4119 007d 067c 0564 4119 007d 177c  .dA..}.|.dA..}.|
+000016f0: 0564 4219 007d 187c 0564 4319 007d 197c  .dB..}.|.dC..}.|
+00001700: 0564 4419 007d 1a7c 0564 4519 007d 1b7c  .dD..}.|.dE..}.|
+00001710: 0564 4619 007d 1c7c 0564 4719 007d 1d7c  .dF..}.|.dG..}.|
+00001720: 0564 4819 007d 0e7c 0564 4919 007d 0f7c  .dH..}.|.dI..}.|
+00001730: 0564 4a19 007d 107c 0564 2719 007d 0d7c  .dJ..}.|.d'..}.|
+00001740: 0564 4b19 007d 1e7c 0564 4c19 007d 1f7c  .dK..}.|.dL..}.|
+00001750: 0564 4d19 007d 207c 0564 4e19 007d 217c  .dM..} |.dN..}!|
+00001760: 0564 4f19 007d 227c 0564 5019 007d 237c  .dO..}"|.dP..}#|
+00001770: 0564 5119 007d 247c 0564 5219 007d 257c  .dQ..}$|.dR..}%|
+00001780: 0564 2619 007d 0c6e 0874 0e64 5383 0182  .d&..}.n.t.dS...
+00001790: 0174 057c 1183 0164 1574 0664 1674 0774  .t.|...d.t.d.t.t
+000017a0: 057c 1183 0183 0118 0083 0114 0017 007d  .|.............}
+000017b0: 1174 057c 1483 0164 1574 0664 1674 0774  .t.|...d.t.d.t.t
+000017c0: 057c 1483 0183 0118 0083 0114 0017 007d  .|.............}
+000017d0: 1474 057c 1583 0164 1574 0664 1674 0774  .t.|...d.t.d.t.t
+000017e0: 057c 1583 0183 0118 0083 0114 0017 007d  .|.............}
+000017f0: 1574 057c 0a83 0164 1574 0664 1674 0774  .t.|...d.t.d.t.t
+00001800: 057c 0a83 0183 0118 0083 0114 0017 007d  .|.............}
+00001810: 0a74 057c 0883 0164 1574 0664 1674 0774  .t.|...d.t.d.t.t
+00001820: 057c 0883 0183 0118 0083 0114 0017 007d  .|.............}
+00001830: 0874 057c 1683 0164 1574 0664 1674 0774  .t.|...d.t.d.t.t
+00001840: 057c 1683 0183 0118 0083 0114 0017 007d  .|.............}
+00001850: 1674 057c 0683 0164 1574 0664 1674 0774  .t.|...d.t.d.t.t
+00001860: 057c 0683 0183 0118 0083 0114 0017 007d  .|.............}
+00001870: 0674 057c 1783 0164 1574 0664 1674 0774  .t.|...d.t.d.t.t
+00001880: 057c 1783 0183 0118 0083 0114 0017 007d  .|.............}
+00001890: 1774 057c 1883 0164 1574 0664 1674 0774  .t.|...d.t.d.t.t
+000018a0: 057c 1883 0183 0118 0083 0114 0017 007d  .|.............}
+000018b0: 1874 057c 1983 0164 1574 0664 1674 0774  .t.|...d.t.d.t.t
+000018c0: 057c 1983 0183 0118 0083 0114 0017 007d  .|.............}
+000018d0: 1974 057c 1a83 0164 1574 0664 1674 0774  .t.|...d.t.d.t.t
+000018e0: 057c 1a83 0183 0118 0083 0114 0017 007d  .|.............}
+000018f0: 1a74 057c 1b83 0164 1574 0664 1674 0774  .t.|...d.t.d.t.t
+00001900: 057c 1b83 0183 0118 0083 0114 0017 007d  .|.............}
+00001910: 1b74 057c 1c83 0164 1574 0664 1674 0774  .t.|...d.t.d.t.t
+00001920: 057c 1c83 0183 0118 0083 0114 0017 007d  .|.............}
+00001930: 1c74 057c 1d83 0164 1574 0664 1674 0774  .t.|...d.t.d.t.t
+00001940: 057c 1d83 0183 0118 0083 0114 0017 007d  .|.............}
+00001950: 1d74 057c 0e83 0164 1574 0664 1674 0774  .t.|...d.t.d.t.t
+00001960: 057c 0e83 0183 0118 0083 0114 0017 007d  .|.............}
+00001970: 0e74 057c 0f83 0164 1574 0664 1674 0774  .t.|...d.t.d.t.t
+00001980: 057c 0f83 0183 0118 0083 0114 0017 007d  .|.............}
+00001990: 0f74 057c 1083 0164 1574 0664 1674 0774  .t.|...d.t.d.t.t
+000019a0: 057c 1083 0183 0118 0083 0114 0017 007d  .|.............}
+000019b0: 1074 057c 0d83 0164 1574 0664 1674 0774  .t.|...d.t.d.t.t
+000019c0: 057c 0d83 0183 0118 0083 0114 0017 007d  .|.............}
+000019d0: 0d74 057c 1e83 0164 1574 0664 1674 0774  .t.|...d.t.d.t.t
+000019e0: 057c 1e83 0183 0118 0083 0114 0017 007d  .|.............}
+000019f0: 1e74 057c 1f83 0164 1574 0664 1674 0774  .t.|...d.t.d.t.t
+00001a00: 057c 1f83 0183 0118 0083 0114 0017 007d  .|.............}
+00001a10: 1f74 057c 2083 0164 1574 0664 1674 0774  .t.| ..d.t.d.t.t
+00001a20: 057c 2083 0183 0118 0083 0114 0017 007d  .| ............}
+00001a30: 2074 057c 2183 0164 1574 0664 1674 0774   t.|!..d.t.d.t.t
+00001a40: 057c 2183 0183 0118 0083 0114 0017 007d  .|!............}
+00001a50: 2174 057c 2283 0164 1574 0664 1674 0774  !t.|"..d.t.d.t.t
+00001a60: 057c 2283 0183 0118 0083 0114 0017 007d  .|"............}
+00001a70: 2274 057c 2383 0164 1574 0664 1674 0774  "t.|#..d.t.d.t.t
+00001a80: 057c 2383 0183 0118 0083 0114 0017 007d  .|#............}
+00001a90: 2374 057c 2483 0164 1574 0664 1674 0774  #t.|$..d.t.d.t.t
+00001aa0: 057c 2483 0183 0118 0083 0114 0017 007d  .|$............}
+00001ab0: 2474 057c 2583 0164 1574 0664 1674 0774  $t.|%..d.t.d.t.t
+00001ac0: 057c 2583 0183 0118 0083 0114 0017 007d  .|%............}
+00001ad0: 2574 057c 0c83 0164 1574 0664 1674 0774  %t.|...d.t.d.t.t
+00001ae0: 057c 0c83 0183 0118 0083 0114 0017 007d  .|.............}
+00001af0: 0c64 2d7c 009b 0064 547c 159b 0064 557c  .d-|...dT|...dU|
+00001b00: 149b 0064 567c 069b 0064 577c 179b 0064  ...dV|...dW|...d
+00001b10: 2f7c 189b 0064 587c 199b 0064 597c 1a9b  /|...dX|...dY|..
+00001b20: 0064 307c 089b 0064 317c 169b 0064 327c  .d0|...d1|...d2|
+00001b30: 0a9b 0064 5a7c 1b9b 0064 5b7c 1f9b 0064  ...dZ|...d[|...d
+00001b40: 5c7c 1c9b 0064 5d7c 1d9b 0064 5e7c 239b  \|...d]|...d^|#.
+00001b50: 0064 5f7c 249b 0064 607c 229b 0064 617c  .d_|$..d`|"..da|
+00001b60: 209b 0064 627c 219b 0064 337c 0e9b 0064   ..db|!..d3|...d
+00001b70: 357c 0f9b 0064 367c 109b 0064 347c 0d9b  5|...d6|...d4|..
+00001b80: 0064 637c 1e9b 0064 647c 259b 0064 657c  .dc|...dd|%..de|
+00001b90: 0c9b 0064 399d 377d 1274 0f7c 1283 0101  ...d9.7}.t.|....
+00001ba0: 0074 007c 1264 3a17 0037 0061 0057 006e  .t.|.d:..7.a.W.n
+00001bb0: 2c01 0001 0001 0064 2d7c 009b 0064 3b9d  ,......d-|...d;.
+00001bc0: 037d 1274 0f7c 1283 0101 0074 007c 1264  .}.t.|.....t.|.d
+00001bd0: 3a17 0037 0061 0059 006e 0230 0090 056e  :..7.a.Y.n.0...n
+00001be0: f07c 0364 666b 0290 0f72 1290 057a b674  .|.dfk...r...z.t
+00001bf0: 0a6a 0b7c 0164 6619 0064 1b7c 0264 1c8d  .j.|.df..d.|.d..
+00001c00: 037d 047c 04a0 0ca1 007d 057c 046a 0d64  .}.|.....}.|.j.d
+00001c10: 1d6b 0290 0a72 847c 0564 1f19 0064 046b  .k...r.|.d...d.k
+00001c20: 0290 0a72 847c 0564 3d19 007d 117c 0564  ...r.|.d=..}.|.d
+00001c30: 6719 007d 267c 0564 6819 007d 277c 0564  g..}&|.dh..}'|.d
+00001c40: 4619 007d 1c7c 0564 2019 007d 067c 0564  F..}.|.d ..}.|.d
+00001c50: 4219 007d 187c 0564 2319 007d 087c 0564  B..}.|.d#..}.|.d
+00001c60: 4019 007d 167c 0564 2419 007d 0a7c 0564  @..}.|.d$..}.|.d
+00001c70: 4919 007d 0f7c 0564 4a19 007d 107c 0564  I..}.|.dJ..}.|.d
+00001c80: 6919 007d 287c 0564 4819 007d 0e7c 0564  i..}(|.dH..}.|.d
+00001c90: 6a19 007d 297c 0564 6b19 007d 2a7c 0564  j..})|.dk..}*|.d
+00001ca0: 6c19 007d 2b7c 0564 6d19 0064 6e19 007d  l..}+|.dm..dn..}
+00001cb0: 2c7c 0564 6d19 0064 6f19 007d 2d7c 0564  ,|.dm..do..}-|.d
+00001cc0: 6d19 0064 7019 007d 2e7c 0564 7119 0064  m..dp..}.|.dq..d
+00001cd0: 5219 007d 257c 0564 7119 0064 2619 007d  R..}%|.dq..d&..}
+00001ce0: 0c7c 0564 7119 0064 2519 007d 0b7c 0564  .|.dq..d%..}.|.d
+00001cf0: 7119 0064 7219 007d 2f7c 0564 2719 0064  q..dr..}/|.d'..d
+00001d00: 7319 007d 307c 0564 2719 0064 7419 007d  s..}0|.d'..dt..}
+00001d10: 317c 0564 2719 0064 7519 007d 327c 0564  1|.d'..du..}2|.d
+00001d20: 2719 0064 7619 007d 337c 0564 2719 0064  '..dv..}3|.d'..d
+00001d30: 7719 007d 347c 0564 2719 0064 7819 007d  w..}4|.d'..dx..}
+00001d40: 356e 0874 0e64 7983 0182 0174 057c 1183  5n.t.dy....t.|..
+00001d50: 0164 1574 0664 1674 0774 057c 1183 0183  .d.t.d.t.t.|....
+00001d60: 0118 0083 0114 0017 007d 1174 057c 2683  .........}.t.|&.
+00001d70: 0164 1574 0664 1674 0774 057c 2683 0183  .d.t.d.t.t.|&...
+00001d80: 0118 0083 0114 0017 007d 2674 057c 2783  .........}&t.|'.
+00001d90: 0164 1574 0664 1674 0774 057c 2783 0183  .d.t.d.t.t.|'...
+00001da0: 0118 0083 0114 0017 007d 2774 057c 1c83  .........}'t.|..
+00001db0: 0164 1574 0664 1674 0774 057c 1c83 0183  .d.t.d.t.t.|....
+00001dc0: 0118 0083 0114 0017 007d 1c74 057c 0683  .........}.t.|..
+00001dd0: 0164 1574 0664 1674 0774 057c 0683 0183  .d.t.d.t.t.|....
+00001de0: 0118 0083 0114 0017 007d 0674 057c 1883  .........}.t.|..
+00001df0: 0164 1574 0664 1674 0774 057c 1883 0183  .d.t.d.t.t.|....
+00001e00: 0118 0083 0114 0017 007d 1874 057c 0883  .........}.t.|..
+00001e10: 0164 1574 0664 1674 0774 057c 0883 0183  .d.t.d.t.t.|....
+00001e20: 0118 0083 0114 0017 007d 0874 057c 1683  .........}.t.|..
+00001e30: 0164 1574 0664 1674 0774 057c 1683 0183  .d.t.d.t.t.|....
+00001e40: 0118 0083 0114 0017 007d 1674 057c 0a83  .........}.t.|..
+00001e50: 0164 1574 0664 1674 0774 057c 0a83 0183  .d.t.d.t.t.|....
+00001e60: 0118 0083 0114 0017 007d 0a74 057c 0f83  .........}.t.|..
+00001e70: 0164 1574 0664 1674 0774 057c 0f83 0183  .d.t.d.t.t.|....
+00001e80: 0118 0083 0114 0017 007d 0f74 057c 1083  .........}.t.|..
+00001e90: 0164 1574 0664 1674 0774 057c 1083 0183  .d.t.d.t.t.|....
+00001ea0: 0118 0083 0114 0017 007d 1074 057c 2883  .........}.t.|(.
+00001eb0: 0164 1574 0664 1674 0774 057c 2883 0183  .d.t.d.t.t.|(...
+00001ec0: 0118 0083 0114 0017 007d 2874 057c 0e83  .........}(t.|..
+00001ed0: 0164 1574 0664 1674 0774 057c 0e83 0183  .d.t.d.t.t.|....
+00001ee0: 0118 0083 0114 0017 007d 0e74 057c 2983  .........}.t.|).
+00001ef0: 0164 1574 0664 1674 0774 057c 2983 0183  .d.t.d.t.t.|)...
+00001f00: 0118 0083 0114 0017 007d 2974 057c 2a83  .........})t.|*.
+00001f10: 0164 1574 0664 1674 0774 057c 2a83 0183  .d.t.d.t.t.|*...
+00001f20: 0118 0083 0114 0017 007d 2a74 057c 2b83  .........}*t.|+.
+00001f30: 0164 1574 0664 1674 0774 057c 2b83 0183  .d.t.d.t.t.|+...
+00001f40: 0118 0083 0114 0017 007d 2b74 057c 2c83  .........}+t.|,.
+00001f50: 0164 1574 0664 1674 0774 057c 2c83 0183  .d.t.d.t.t.|,...
+00001f60: 0118 0083 0114 0017 007d 2c74 057c 2d83  .........},t.|-.
+00001f70: 0164 1574 0664 1674 0774 057c 2d83 0183  .d.t.d.t.t.|-...
+00001f80: 0118 0083 0114 0017 007d 2d74 057c 2e83  .........}-t.|..
+00001f90: 0164 1574 0664 1674 0774 057c 2e83 0183  .d.t.d.t.t.|....
+00001fa0: 0118 0083 0114 0017 007d 2e74 057c 2583  .........}.t.|%.
+00001fb0: 0164 1574 0664 1674 0774 057c 2583 0183  .d.t.d.t.t.|%...
+00001fc0: 0118 0083 0114 0017 007d 2574 057c 0c83  .........}%t.|..
+00001fd0: 0164 1574 0664 1674 0774 057c 0c83 0183  .d.t.d.t.t.|....
+00001fe0: 0118 0083 0114 0017 007d 0c74 057c 0b83  .........}.t.|..
+00001ff0: 0164 1574 0664 1674 0774 057c 0b83 0183  .d.t.d.t.t.|....
+00002000: 0118 0083 0114 0017 007d 0b74 057c 2f83  .........}.t.|/.
+00002010: 0164 1574 0664 1674 0774 057c 2f83 0183  .d.t.d.t.t.|/...
+00002020: 0118 0083 0114 0017 007d 2f74 057c 3083  .........}/t.|0.
+00002030: 0164 1574 0664 1674 0774 057c 3083 0183  .d.t.d.t.t.|0...
+00002040: 0118 0083 0114 0017 007d 3074 057c 3183  .........}0t.|1.
+00002050: 0164 1574 0664 1674 0774 057c 3183 0183  .d.t.d.t.t.|1...
+00002060: 0118 0083 0114 0017 007d 3174 057c 3283  .........}1t.|2.
+00002070: 0164 1574 0664 1674 0774 057c 3283 0183  .d.t.d.t.t.|2...
+00002080: 0118 0083 0114 0017 007d 3274 057c 3383  .........}2t.|3.
+00002090: 0164 1574 0664 1674 0774 057c 3383 0183  .d.t.d.t.t.|3...
+000020a0: 0118 0083 0114 0017 007d 3374 057c 3483  .........}3t.|4.
+000020b0: 0164 1574 0664 1674 0774 057c 3483 0183  .d.t.d.t.t.|4...
+000020c0: 0118 0083 0114 0017 007d 3474 057c 3583  .........}4t.|5.
+000020d0: 0164 1574 0664 1674 0774 057c 3583 0183  .d.t.d.t.t.|5...
+000020e0: 0118 0083 0114 0017 007d 3564 2d7c 009b  .........}5d-|..
+000020f0: 0064 547c 269b 0064 567c 069b 0064 2f7c  .dT|&..dV|...d/|
+00002100: 189b 0064 307c 089b 0064 317c 169b 0064  ...d0|...d1|...d
+00002110: 327c 0a9b 0064 7a7c 2a9b 0064 7b7c 279b  2|...dz|*..d{|'.
+00002120: 0064 5c7c 1c9b 0064 5d7c 289b 0064 7c7c  .d\|...d]|(..d||
+00002130: 2b9b 0064 7d7c 2e9b 0064 337c 0e9b 0064  +..d}|...d3|...d
+00002140: 5b7c 299b 0064 357c 0f9b 0064 367c 109b  [|)..d5|...d6|..
+00002150: 0064 7e7c 309b 0064 7f7c 319b 0064 807c  .d~|0..d.|1..d.|
+00002160: 329b 0064 817c 339b 0064 827c 349b 0064  2..d.|3..d.|4..d
+00002170: 837c 359b 0064 647c 259b 0064 657c 0b9b  .|5..dd|%..de|..
+00002180: 0064 847c 2f9b 0064 399d 357d 1274 0f7c  .d.|/..d9.5}.t.|
+00002190: 1283 0101 0074 007c 1264 3a17 0037 0061  .....t.|.d:..7.a
+000021a0: 0057 006e 2c01 0001 0001 0064 2d7c 009b  .W.n,......d-|..
+000021b0: 0064 3b9d 037d 1274 0f7c 1283 0101 0074  .d;..}.t.|.....t
+000021c0: 007c 1264 3a17 0037 0061 0059 006e 0230  .|.d:..7.a.Y.n.0
+000021d0: 0064 0453 0029 854e 7213 0000 00fa 2820  .d.S.).Nr.....( 
+000021e0: 2020 205b 2b5d 2056 6572 6966 7969 6e67     [+] Verifying
+000021f0: 2069 6e74 6572 6e65 7420 636f 6e6e 6563   internet connec
+00002200: 7469 6f6e 2e2e 2e72 2300 0000 5472 2700  tion...r#...Tr'.
+00002210: 0000 fa28 2020 2020 3e20 496e 7465 726e  ...(    > Intern
+00002220: 6574 2063 6f6e 6e65 6374 696f 6e20 6e6f  et connection no
+00002230: 7420 6176 6169 6c61 626c 6521 722c 0000  t available!r,..
+00002240: 0046 7221 0000 0072 2200 0000 7a3a 2020  .Fr!...r"...z:  
+00002250: 2020 1b5b 313b 3439 3b39 336d 5b23 5d20    .[1;49;93m[#] 
+00002260: 5265 7665 7273 6520 6970 2061 6464 7265  Reverse ip addre
+00002270: 7373 206c 6f6f 6b75 7020 666f 7220 1b5b  ss lookup for .[
+00002280: 313b 3439 3b39 366d 722a 0000 0072 2b00  1;49;96mr*...r+.
+00002290: 0000 7a24 5e5c 647b 312c 337d 5c2e 5c64  ..z$^\d{1,3}\.\d
+000022a0: 7b31 2c33 7d5c 2e5c 647b 312c 337d 5c2e  {1,3}\.\d{1,3}\.
+000022b0: 5c64 7b31 2c33 7d24 7a33 2020 2020 3e20  \d{1,3}$z3    > 
+000022c0: 496e 7661 6c69 6420 6970 2061 6464 7265  Invalid ip addre
+000022d0: 7373 2066 6f72 6d61 7421 2028 4578 616d  ss format! (Exam
+000022e0: 706c 653a 2038 2e38 2e38 2e38 2972 2e00  ple: 8.8.8.8)r..
+000022f0: 0000 7a17 6874 7470 3a2f 2f69 702d 6170  ..z.http://ip-ap
+00002300: 692e 636f 6d2f 6a73 6f6e 2f7a 1168 7474  i.com/json/z.htt
+00002310: 7073 3a2f 2f69 7061 7069 2e63 6f2f 7a06  ps://ipapi.co/z.
+00002320: 2f6a 736f 6e2f 7a10 6874 7470 3a2f 2f69  /json/z.http://i
+00002330: 7077 686f 2e69 732f 7236 0000 0072 3700  pwho.is/r6...r7.
+00002340: 0000 fa0a 5573 6572 2d41 6765 6e74 7a44  ....User-AgentzD
+00002350: 4d6f 7a69 6c6c 612f 352e 3020 2858 3131  Mozilla/5.0 (X11
+00002360: 3b20 4c69 6e75 7820 7838 365f 3634 3b20  ; Linux x86_64; 
+00002370: 7276 3a38 392e 3029 2047 6563 6b6f 2f32  rv:89.0) Gecko/2
+00002380: 3031 3030 3130 3120 4669 7265 666f 782f  0100101 Firefox/
+00002390: 3839 2e30 2903 7201 0000 0072 2400 0000  89.0).r....r$...
+000023a0: e902 0000 0072 0100 0000 7214 0000 0029  .....r....r....)
+000023b0: 0272 1500 0000 da07 6865 6164 6572 73e9  .r......headers.
+000023c0: c800 0000 da06 7374 6174 7573 da07 7375  ......status..su
+000023d0: 6363 6573 7372 4d00 0000 da0b 636f 756e  ccessrM.....coun
+000023e0: 7472 7943 6f64 655a 0a72 6567 696f 6e4e  tryCodeZ.regionN
+000023f0: 616d 65da 0672 6567 696f 6eda 0463 6974  ame..region..cit
+00002400: 79da 0369 7370 da03 6f72 6772 1e00 0000  y..isp..orgr....
+00002410: da03 7a69 705a 036c 6174 5a03 6c6f 6eda  ..zipZ.latZ.lon.
+00002420: 0571 7565 7279 7a20 7265 7665 7273 652d  .queryz reverse-
+00002430: 6970 2d6c 6f6f 6b75 702d 7365 7276 6572  ip-lookup-server
+00002440: 2d31 2d65 7272 6f72 75d2 0000 000a 2020  -1-erroru.....  
+00002450: 2020 e294 8ce2 9480 e294 80e2 9480 e294    ..............
+00002460: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00002470: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00002480: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00002490: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+000024a0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+000024b0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+000024c0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+000024d0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+000024e0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+000024f0: 80e2 9480 e294 80e2 9490 0a20 2020 207c  ...........    |
+00002500: 2053 6361 6e6e 6564 2049 5020 4164 6472   Scanned IP Addr
+00002510: 6573 733a 201b 5b31 3b34 393b 3936 6d7a  ess: .[1;49;96mz
+00002520: ea1b 5b30 6d20 2020 7c0a 2020 2020 7c2d  ..[0m   |.    |-
 00002530: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00002540: 2d2d 2d2d 2d2d 2d2d 2d7c 0a20 2020 207c  ---------|.    |
-00002550: 2049 4e46 4f52 4d41 5449 4f4e 2020 2020   INFORMATION    
-00002560: 2020 2020 207c 2044 4553 4352 4950 5449       | DESCRIPTI
-00002570: 4f4e 2020 2020 2020 2020 2020 2020 2020  ON              
-00002580: 2020 2020 2020 7c0a 2020 2020 7c2d 2d2d        |.    |---
-00002590: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000025a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00002540: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00002550: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00002560: 2d2d 2d2d 2d7c 0a20 2020 207c 2049 4e46  -----|.    | INF
+00002570: 4f52 4d41 5449 4f4e 2020 2020 2020 2020  ORMATION        
+00002580: 207c 2044 4553 4352 4950 5449 4f4e 2020   | DESCRIPTION  
+00002590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000025a0: 2020 7c0a 2020 2020 7c2d 2d2d 2d2d 2d2d    |.    |-------
 000025b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000025c0: 2d2d 2d7c 0a20 2020 207c 201b 5b31 3b34  ---|.    | .[1;4
-000025d0: 393b 3937 6d43 6f75 6e74 7279 1b5b 306d  9;97mCountry.[0m
-000025e0: 2020 2020 2020 2020 2020 2020 207c 207a               | z
-000025f0: 2d20 7c0a 2020 2020 7c20 1b5b 313b 3439  - |.    | .[1;49
-00002600: 3b39 376d 436f 756e 7472 7920 436f 6465  ;97mCountry Code
-00002610: 1b5b 306d 2020 2020 2020 2020 7c20 7a2d  .[0m        | z-
-00002620: 207c 0a20 2020 207c 201b 5b31 3b34 393b   |.    | .[1;49;
-00002630: 3937 6d52 6567 696f 6e1b 5b30 6d20 2020  97mRegion.[0m   
-00002640: 2020 2020 2020 2020 2020 207c 2072 3200             | r2.
-00002650: 0000 7a2d 207c 0a20 2020 207c 201b 5b31  ..z- |.    | .[1
-00002660: 3b34 393b 3937 6d43 6974 791b 5b30 6d20  ;49;97mCity.[0m 
-00002670: 2020 2020 2020 2020 2020 2020 2020 207c                 |
-00002680: 207a 6a20 7c0a 2020 2020 7c2d 2d2d 2d2d   zj |.    |-----
-00002690: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000026a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000025c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000025d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d7c  ---------------|
+000025e0: 0a20 2020 207c 201b 5b31 3b34 393b 3937  .    | .[1;49;97
+000025f0: 6d43 6f75 6e74 7279 1b5b 306d 2020 2020  mCountry.[0m    
+00002600: 2020 2020 2020 2020 207c 207a 2d20 7c0a           | z- |.
+00002610: 2020 2020 7c20 1b5b 313b 3439 3b39 376d      | .[1;49;97m
+00002620: 436f 756e 7472 7920 436f 6465 1b5b 306d  Country Code.[0m
+00002630: 2020 2020 2020 2020 7c20 7a2d 207c 0a20          | z- |. 
+00002640: 2020 207c 201b 5b31 3b34 393b 3937 6d52     | .[1;49;97mR
+00002650: 6567 696f 6e1b 5b30 6d20 2020 2020 2020  egion.[0m       
+00002660: 2020 2020 2020 207c 2072 3800 0000 7a2d         | r8...z-
+00002670: 207c 0a20 2020 207c 201b 5b31 3b34 393b   |.    | .[1;49;
+00002680: 3937 6d43 6974 791b 5b30 6d20 2020 2020  97mCity.[0m     
+00002690: 2020 2020 2020 2020 2020 207c 207a 6a20             | zj 
+000026a0: 7c0a 2020 2020 7c2d 2d2d 2d2d 2d2d 2d2d  |.    |---------
 000026b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000026c0: 2d7c 0a20 2020 207c 201b 5b31 3b34 393b  -|.    | .[1;49;
-000026d0: 3937 6d50 6f73 7461 6c20 436f 6465 1b5b  97mPostal Code.[
-000026e0: 306d 2020 2020 2020 2020 207c 2072 3300  0m         | r3.
-000026f0: 0000 7a2d 207c 0a20 2020 207c 201b 5b31  ..z- |.    | .[1
-00002700: 3b34 393b 3937 6d4c 6174 6974 7564 651b  ;49;97mLatitude.
-00002710: 5b30 6d20 2020 2020 2020 2020 2020 207c  [0m            |
-00002720: 207a 2d20 7c0a 2020 2020 7c20 1b5b 313b   z- |.    | .[1;
-00002730: 3439 3b39 376d 4c6f 6e67 6974 7564 651b  49;97mLongitude.
-00002740: 5b30 6d20 2020 2020 2020 2020 2020 7c20  [0m           | 
-00002750: 7a6a 207c 0a20 2020 207c 2d2d 2d2d 2d2d  zj |.    |------
-00002760: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00002770: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000026c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000026d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d7c 0a20  -------------|. 
+000026e0: 2020 207c 201b 5b31 3b34 393b 3937 6d50     | .[1;49;97mP
+000026f0: 6f73 7461 6c20 436f 6465 1b5b 306d 2020  ostal Code.[0m  
+00002700: 2020 2020 2020 207c 2072 3900 0000 7a2d         | r9...z-
+00002710: 207c 0a20 2020 207c 201b 5b31 3b34 393b   |.    | .[1;49;
+00002720: 3937 6d4c 6174 6974 7564 651b 5b30 6d20  97mLatitude.[0m 
+00002730: 2020 2020 2020 2020 2020 207c 207a 2d20             | z- 
+00002740: 7c0a 2020 2020 7c20 1b5b 313b 3439 3b39  |.    | .[1;49;9
+00002750: 376d 4c6f 6e67 6974 7564 651b 5b30 6d20  7mLongitude.[0m 
+00002760: 2020 2020 2020 2020 2020 7c20 7a6a 207c            | zj |
+00002770: 0a20 2020 207c 2d2d 2d2d 2d2d 2d2d 2d2d  .    |----------
 00002780: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00002790: 7c0a 2020 2020 7c20 1b5b 313b 3439 3b39  |.    | .[1;49;9
-000027a0: 376d 4953 501b 5b30 6d20 2020 2020 2020  7mISP.[0m       
-000027b0: 2020 2020 2020 2020 2020 7c20 7a2d 207c            | z- |
-000027c0: 0a20 2020 207c 201b 5b31 3b34 393b 3937  .    | .[1;49;97
-000027d0: 6d4f 7267 1b5b 306d 2020 2020 2020 2020  mOrg.[0m        
-000027e0: 2020 2020 2020 2020 207c 2075 b400 0000           | u....
-000027f0: 207c 0a20 2020 20e2 9494 e294 80e2 9480   |.    .........
-00002800: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00002810: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00002820: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00002830: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00002840: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00002850: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00002860: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00002870: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00002880: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00002890: e294 80e2 9480 e294 80e2 9480 e294 980a  ................
-000028a0: 2020 2020 758d 0100 001b 5b30 6d20 2020      u.....[0m   
-000028b0: 7c0a 2020 2020 7c20 5365 7276 6572 2063  |.    | Server c
-000028c0: 6f64 6520 6e61 6d65 2020 3a20 1b5b 313b  ode name  : .[1;
-000028d0: 3439 3b39 366d 7265 7665 7273 652d 6970  49;96mreverse-ip
-000028e0: 2d6c 6f6f 6b75 702d 7365 7276 6572 2d31  -lookup-server-1
-000028f0: 1b5b 306d 2020 2020 2020 207c 0a20 2020  .[0m       |.   
-00002900: 207c 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   |--------------
-00002910: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00002920: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00002930: 2d2d 2d2d 2d2d 2d2d 7c0a 2020 2020 7c20  --------|.    | 
-00002940: 1b5b 313b 3439 3b39 316d 4661 696c 6564  .[1;49;91mFailed
-00002950: 2074 6f20 4665 7463 6820 696e 666f 726d   to Fetch inform
-00002960: 6174 696f 6e20 6672 6f6d 2074 6869 7320  ation from this 
-00002970: 7365 7276 6572 211b 5b30 6d20 2020 2020  server!.[0m     
-00002980: 2020 207c 0a20 2020 20e2 9494 e294 80e2     |.    .......
+00002790: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000027a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 7c0a 2020  ------------|.  
+000027b0: 2020 7c20 1b5b 313b 3439 3b39 376d 4953    | .[1;49;97mIS
+000027c0: 501b 5b30 6d20 2020 2020 2020 2020 2020  P.[0m           
+000027d0: 2020 2020 2020 7c20 7a2d 207c 0a20 2020        | z- |.   
+000027e0: 207c 201b 5b31 3b34 393b 3937 6d4f 7267   | .[1;49;97mOrg
+000027f0: 1b5b 306d 2020 2020 2020 2020 2020 2020  .[0m            
+00002800: 2020 2020 207c 20f5 b400 0000 207c 0a20       | ..... |. 
+00002810: 2020 20e2 9494 e294 80e2 9480 e294 80e2     .............
+00002820: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00002830: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00002840: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00002850: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00002860: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00002870: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00002880: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00002890: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+000028a0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+000028b0: 9480 e294 80e2 9480 e294 980a 2020 2020  ............    
+000028c0: 723a 0000 0075 4201 0000 1b5b 306d 2020  r:...uB....[0m  
+000028d0: 207c 0a20 2020 207c 2d2d 2d2d 2d2d 2d2d   |.    |--------
+000028e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000028f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00002900: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 7c0a  --------------|.
+00002910: 2020 2020 7c20 1b5b 313b 3439 3b39 316d      | .[1;49;91m
+00002920: 4661 696c 6564 2074 6f20 4665 7463 6820  Failed to Fetch 
+00002930: 696e 666f 726d 6174 696f 6e20 6672 6f6d  information from
+00002940: 2074 6869 7320 7365 7276 6572 211b 5b30   this server!.[0
+00002950: 6d20 2020 2020 2020 207c 0a20 2020 20e2  m        |.    .
+00002960: 9494 e294 80e2 9480 e294 80e2 9480 e294  ................
+00002970: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00002980: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
 00002990: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
 000029a0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
 000029b0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
 000029c0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
 000029d0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
 000029e0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
 000029f0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00002a00: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00002a10: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00002a20: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00002a30: 980a 2020 2020 721e 0000 0072 0e00 0000  ..    r....r....
-00002a40: da07 6e65 7477 6f72 6bda 0776 6572 7369  ..network..versi
-00002a50: 6f6e 7245 0000 00da 0c63 6f75 6e74 7279  onrE.....country
-00002a60: 5f6e 616d 6572 4300 0000 da11 636f 756e  _namerC.....coun
-00002a70: 7472 795f 636f 6465 5f69 736f 33da 0f63  try_code_iso3..c
-00002a80: 6f75 6e74 7279 5f63 6170 6974 616c da0b  ountry_capital..
-00002a90: 636f 756e 7472 795f 746c 64da 0e63 6f6e  country_tld..con
-00002aa0: 7469 6e65 6e74 5f63 6f64 65da 0569 6e5f  tinent_code..in_
-00002ab0: 6575 da06 706f 7374 616c da08 6c61 7469  eu..postal..lati
-00002ac0: 7475 6465 da09 6c6f 6e67 6974 7564 65da  tude..longitude.
-00002ad0: 0a75 7463 5f6f 6666 7365 74da 1463 6f75  .utc_offset..cou
-00002ae0: 6e74 7279 5f63 616c 6c69 6e67 5f63 6f64  ntry_calling_cod
-00002af0: 65da 0863 7572 7265 6e63 79da 0d63 7572  e..currency..cur
-00002b00: 7265 6e63 795f 6e61 6d65 da09 6c61 6e67  rency_name..lang
-00002b10: 7561 6765 73da 0c63 6f75 6e74 7279 5f61  uages..country_a
-00002b20: 7265 61da 1263 6f75 6e74 7279 5f70 6f70  rea..country_pop
-00002b30: 756c 6174 696f 6eda 0361 736e 7a20 7265  ulation..asnz re
-00002b40: 7665 7273 652d 6970 2d6c 6f6f 6b75 702d  verse-ip-lookup-
-00002b50: 7365 7276 6572 2d32 2d65 7272 6f72 6135  server-2-errora5
-00002b60: 0100 001b 5b30 6d20 2020 7c0a 2020 2020  ....[0m   |.    
-00002b70: 7c20 5365 7276 6572 2063 6f64 6520 6e61  | Server code na
-00002b80: 6d65 2020 3a20 1b5b 313b 3439 3b39 366d  me  : .[1;49;96m
-00002b90: 7265 7665 7273 652d 6970 2d6c 6f6f 6b75  reverse-ip-looku
-00002ba0: 702d 7365 7276 6572 2d32 1b5b 306d 2020  p-server-2.[0m  
-00002bb0: 2020 2020 207c 0a20 2020 207c 2d2d 2d2d       |.    |----
+00002a00: 80e2 9480 e294 980a 2020 2020 7224 0000  ........    r$..
+00002a10: 0072 0c00 0000 da07 6e65 7477 6f72 6bda  .r......network.
+00002a20: 0776 6572 7369 6f6e 724c 0000 00da 0c63  .versionrL.....c
+00002a30: 6f75 6e74 7279 5f6e 616d 6572 4a00 0000  ountry_namerJ...
+00002a40: da11 636f 756e 7472 795f 636f 6465 5f69  ..country_code_i
+00002a50: 736f 33da 0f63 6f75 6e74 7279 5f63 6170  so3..country_cap
+00002a60: 6974 616c da0b 636f 756e 7472 795f 746c  ital..country_tl
+00002a70: 64da 0e63 6f6e 7469 6e65 6e74 5f63 6f64  d..continent_cod
+00002a80: 65da 0569 6e5f 6575 da06 706f 7374 616c  e..in_eu..postal
+00002a90: da08 6c61 7469 7475 6465 da09 6c6f 6e67  ..latitude..long
+00002aa0: 6974 7564 65da 0a75 7463 5f6f 6666 7365  itude..utc_offse
+00002ab0: 74da 1463 6f75 6e74 7279 5f63 616c 6c69  t..country_calli
+00002ac0: 6e67 5f63 6f64 65da 0863 7572 7265 6e63  ng_code..currenc
+00002ad0: 79da 0d63 7572 7265 6e63 795f 6e61 6d65  y..currency_name
+00002ae0: da09 6c61 6e67 7561 6765 73da 0c63 6f75  ..languages..cou
+00002af0: 6e74 7279 5f61 7265 61da 1263 6f75 6e74  ntry_area..count
+00002b00: 7279 5f70 6f70 756c 6174 696f 6eda 0361  ry_population..a
+00002b10: 736e 7a20 7265 7665 7273 652d 6970 2d6c  snz reverse-ip-l
+00002b20: 6f6f 6b75 702d 7365 7276 6572 2d32 2d65  ookup-server-2-e
+00002b30: 7272 6f72 7aea 1b5b 306d 2020 207c 0a20  rrorz..[0m   |. 
+00002b40: 2020 207c 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d     |------------
+00002b50: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00002b60: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00002b70: 2d2d 2d2d 2d2d 2d2d 2d2d 7c0a 2020 2020  ----------|.    
+00002b80: 7c20 494e 464f 524d 4154 494f 4e20 2020  | INFORMATION   
+00002b90: 2020 2020 2020 7c20 4445 5343 5249 5054        | DESCRIPT
+00002ba0: 494f 4e20 2020 2020 2020 2020 2020 2020  ION             
+00002bb0: 2020 2020 2020 207c 0a20 2020 207c 2d2d         |.    |--
 00002bc0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00002bd0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00002be0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00002bf0: 2d2d 7c0a 2020 2020 7c20 494e 464f 524d  --|.    | INFORM
-00002c00: 4154 494f 4e20 2020 2020 2020 2020 7c20  ATION         | 
-00002c10: 4445 5343 5249 5054 494f 4e20 2020 2020  DESCRIPTION     
-00002c20: 2020 2020 2020 2020 2020 2020 2020 207c                 |
-00002c30: 0a20 2020 207c 2d2d 2d2d 2d2d 2d2d 2d2d  .    |----------
-00002c40: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00002c50: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00002c60: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 7c0a 2020  ------------|.  
-00002c70: 2020 7c20 1b5b 313b 3439 3b39 376d 4950    | .[1;49;97mIP
-00002c80: 2054 7970 651b 5b30 6d20 2020 2020 2020   Type.[0m       
-00002c90: 2020 2020 2020 7c20 7a2d 207c 0a20 2020        | z- |.   
-00002ca0: 207c 201b 5b31 3b34 393b 3937 6d4e 6574   | .[1;49;97mNet
-00002cb0: 776f 726b 1b5b 306d 2020 2020 2020 2020  work.[0m        
-00002cc0: 2020 2020 207c 207a 6a20 7c0a 2020 2020       | zj |.    
-00002cd0: 7c2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  |---------------
-00002ce0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00002cf0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00002d00: 2d2d 2d2d 2d2d 2d7c 0a20 2020 207c 201b  -------|.    | .
-00002d10: 5b31 3b34 393b 3937 6d43 6f75 6e74 7279  [1;49;97mCountry
-00002d20: 1b5b 306d 2020 2020 2020 2020 2020 2020  .[0m            
-00002d30: 207c 207a 2d20 7c0a 2020 2020 7c20 1b5b   | z- |.    | .[
-00002d40: 313b 3439 3b39 376d 436f 756e 7472 7920  1;49;97mCountry 
-00002d50: 4e61 6d65 1b5b 306d 2020 2020 2020 2020  Name.[0m        
-00002d60: 7c20 7a2d 207c 0a20 2020 207c 201b 5b31  | z- |.    | .[1
-00002d70: 3b34 393b 3937 6d43 6f75 6e74 7279 2043  ;49;97mCountry C
-00002d80: 6f64 6520 4953 4f33 1b5b 306d 2020 207c  ode ISO3.[0m   |
-00002d90: 207a 2d20 7c0a 2020 2020 7c20 1b5b 313b   z- |.    | .[1;
-00002da0: 3439 3b39 376d 436f 756e 7472 7920 4361  49;97mCountry Ca
-00002db0: 7069 7461 6c1b 5b30 6d20 2020 2020 7c20  pital.[0m     | 
-00002dc0: 7a6a 207c 0a20 2020 207c 2d2d 2d2d 2d2d  zj |.    |------
-00002dd0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00002de0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00002df0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00002e00: 7c0a 2020 2020 7c20 1b5b 313b 3439 3b39  |.    | .[1;49;9
-00002e10: 376d 436f 756e 7472 7920 544c 441b 5b30  7mCountry TLD.[0
-00002e20: 6d20 2020 2020 2020 2020 7c20 7a2d 207c  m         | z- |
-00002e30: 0a20 2020 207c 201b 5b31 3b34 393b 3937  .    | .[1;49;97
-00002e40: 6d43 616c 6c69 6e67 2050 7265 6669 781b  mCalling Prefix.
-00002e50: 5b30 6d20 2020 2020 207c 207a 2d20 7c0a  [0m      | z- |.
-00002e60: 2020 2020 7c20 1b5b 313b 3439 3b39 376d      | .[1;49;97m
-00002e70: 436f 6e74 696e 656e 7420 436f 6465 1b5b  Continent Code.[
-00002e80: 306d 2020 2020 2020 7c20 7a2d 207c 0a20  0m      | z- |. 
-00002e90: 2020 207c 201b 5b31 3b34 393b 3937 6d49     | .[1;49;97mI
-00002ea0: 6e20 4555 1b5b 306d 2020 2020 2020 2020  n EU.[0m        
-00002eb0: 2020 2020 2020 207c 207a 2d20 7c0a 2020         | z- |.  
-00002ec0: 2020 7c20 1b5b 313b 3439 3b39 376d 4170    | .[1;49;97mAp
-00002ed0: 7072 6f78 2e20 4172 6561 1b5b 306d 2020  prox. Area.[0m  
-00002ee0: 2020 2020 2020 7c20 7a2d 207c 0a20 2020        | z- |.   
-00002ef0: 207c 201b 5b31 3b34 393b 3937 6d41 7070   | .[1;49;97mApp
-00002f00: 726f 782e 2050 6f70 756c 6174 696f 6e1b  rox. Population.
-00002f10: 5b30 6d20 207c 207a 2d20 7c0a 2020 2020  [0m  | z- |.    
-00002f20: 7c20 1b5b 313b 3439 3b39 376d 4c61 6e67  | .[1;49;97mLang
-00002f30: 7561 6765 7320 5370 6f6b 656e 1b5b 306d  uages Spoken.[0m
-00002f40: 2020 2020 7c20 7a2d 207c 0a20 2020 207c      | z- |.    |
-00002f50: 201b 5b31 3b34 393b 3937 6d43 7572 7265   .[1;49;97mCurre
-00002f60: 6e63 791b 5b30 6d20 2020 2020 2020 2020  ncy.[0m         
-00002f70: 2020 207c 207a 2d20 7c0a 2020 2020 7c20     | z- |.    | 
-00002f80: 1b5b 313b 3439 3b39 376d 4375 7272 656e  .[1;49;97mCurren
-00002f90: 6379 204e 616d 651b 5b30 6d20 2020 2020  cy Name.[0m     
-00002fa0: 2020 7c20 7a2d 207c 0a20 2020 207c 201b    | z- |.    | .
-00002fb0: 5b31 3b34 393b 3937 6d55 5443 204f 6666  [1;49;97mUTC Off
-00002fc0: 7365 741b 5b30 6d20 2020 2020 2020 2020  set.[0m         
-00002fd0: 207c 207a 6a20 7c0a 2020 2020 7c2d 2d2d   | zj |.    |---
-00002fe0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00002ff0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00003000: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00003010: 2d2d 2d7c 0a20 2020 207c 201b 5b31 3b34  ---|.    | .[1;4
-00003020: 393b 3937 6d41 534e 1b5b 306d 2020 2020  9;97mASN.[0m    
-00003030: 2020 2020 2020 2020 2020 2020 207c 207a               | z
-00003040: 2d20 7c0a 2020 2020 7c20 1b5b 313b 3439  - |.    | .[1;49
-00003050: 3b39 376d 4953 501b 5b30 6d20 2020 2020  ;97mISP.[0m     
-00003060: 2020 2020 2020 2020 2020 2020 7c20 758d              | u.
-00003070: 0100 001b 5b30 6d20 2020 7c0a 2020 2020  ....[0m   |.    
-00003080: 7c20 5365 7276 6572 2063 6f64 6520 6e61  | Server code na
-00003090: 6d65 2020 3a20 1b5b 313b 3439 3b39 366d  me  : .[1;49;96m
-000030a0: 7265 7665 7273 652d 6970 2d6c 6f6f 6b75  reverse-ip-looku
-000030b0: 702d 7365 7276 6572 2d32 1b5b 306d 2020  p-server-2.[0m  
-000030c0: 2020 2020 207c 0a20 2020 207c 2d2d 2d2d       |.    |----
+00002bf0: 2d2d 2d2d 7c0a 2020 2020 7c20 1b5b 313b  ----|.    | .[1;
+00002c00: 3439 3b39 376d 4950 2054 7970 651b 5b30  49;97mIP Type.[0
+00002c10: 6d20 2020 2020 2020 2020 2020 2020 7c20  m             | 
+00002c20: 7a2d 207c 0a20 2020 207c 201b 5b31 3b34  z- |.    | .[1;4
+00002c30: 393b 3937 6d4e 6574 776f 726b 1b5b 306d  9;97mNetwork.[0m
+00002c40: 2020 2020 2020 2020 2020 2020 207c 207a               | z
+00002c50: 6a20 7c0a 2020 2020 7c2d 2d2d 2d2d 2d2d  j |.    |-------
+00002c60: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00002c70: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00002c80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d7c  ---------------|
+00002c90: 0a20 2020 207c 201b 5b31 3b34 393b 3937  .    | .[1;49;97
+00002ca0: 6d43 6f75 6e74 7279 1b5b 306d 2020 2020  mCountry.[0m    
+00002cb0: 2020 2020 2020 2020 207c 207a 2d20 7c0a           | z- |.
+00002cc0: 2020 2020 7c20 1b5b 313b 3439 3b39 376d      | .[1;49;97m
+00002cd0: 436f 756e 7472 7920 4e61 6d65 1b5b 306d  Country Name.[0m
+00002ce0: 2020 2020 2020 2020 7c20 7a2d 207c 0a20          | z- |. 
+00002cf0: 2020 207c 201b 5b31 3b34 393b 3937 6d43     | .[1;49;97mC
+00002d00: 6f75 6e74 7279 2043 6f64 6520 4953 4f33  ountry Code ISO3
+00002d10: 1b5b 306d 2020 207c 207a 2d20 7c0a 2020  .[0m   | z- |.  
+00002d20: 2020 7c20 1b5b 313b 3439 3b39 376d 436f    | .[1;49;97mCo
+00002d30: 756e 7472 7920 4361 7069 7461 6c1b 5b30  untry Capital.[0
+00002d40: 6d20 2020 2020 7c20 7a6a 207c 0a20 2020  m     | zj |.   
+00002d50: 207c 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   |--------------
+00002d60: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00002d70: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00002d80: 2d2d 2d2d 2d2d 2d2d 7c0a 2020 2020 7c20  --------|.    | 
+00002d90: 1b5b 313b 3439 3b39 376d 436f 756e 7472  .[1;49;97mCountr
+00002da0: 7920 544c 441b 5b30 6d20 2020 2020 2020  y TLD.[0m       
+00002db0: 2020 7c20 7a2d 207c 0a20 2020 207c 201b    | z- |.    | .
+00002dc0: 5b31 3b34 393b 3937 6d43 616c 6c69 6e67  [1;49;97mCalling
+00002dd0: 2050 7265 6669 781b 5b30 6d20 2020 2020   Prefix.[0m     
+00002de0: 207c 207a 2d20 7c0a 2020 2020 7c20 1b5b   | z- |.    | .[
+00002df0: 313b 3439 3b39 376d 436f 6e74 696e 656e  1;49;97mContinen
+00002e00: 7420 436f 6465 1b5b 306d 2020 2020 2020  t Code.[0m      
+00002e10: 7c20 7a2d 207c 0a20 2020 207c 201b 5b31  | z- |.    | .[1
+00002e20: 3b34 393b 3937 6d49 6e20 4555 1b5b 306d  ;49;97mIn EU.[0m
+00002e30: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+00002e40: 207a 2d20 7c0a 2020 2020 7c20 1b5b 313b   z- |.    | .[1;
+00002e50: 3439 3b39 376d 4170 7072 6f78 2e20 4172  49;97mApprox. Ar
+00002e60: 6561 1b5b 306d 2020 2020 2020 2020 7c20  ea.[0m        | 
+00002e70: 7a2d 207c 0a20 2020 207c 201b 5b31 3b34  z- |.    | .[1;4
+00002e80: 393b 3937 6d41 7070 726f 782e 2050 6f70  9;97mApprox. Pop
+00002e90: 756c 6174 696f 6e1b 5b30 6d20 207c 207a  ulation.[0m  | z
+00002ea0: 2d20 7c0a 2020 2020 7c20 1b5b 313b 3439  - |.    | .[1;49
+00002eb0: 3b39 376d 4c61 6e67 7561 6765 7320 5370  ;97mLanguages Sp
+00002ec0: 6f6b 656e 1b5b 306d 2020 2020 7c20 7a2d  oken.[0m    | z-
+00002ed0: 207c 0a20 2020 207c 201b 5b31 3b34 393b   |.    | .[1;49;
+00002ee0: 3937 6d43 7572 7265 6e63 791b 5b30 6d20  97mCurrency.[0m 
+00002ef0: 2020 2020 2020 2020 2020 207c 207a 2d20             | z- 
+00002f00: 7c0a 2020 2020 7c20 1b5b 313b 3439 3b39  |.    | .[1;49;9
+00002f10: 376d 4375 7272 656e 6379 204e 616d 651b  7mCurrency Name.
+00002f20: 5b30 6d20 2020 2020 2020 7c20 7a2d 207c  [0m       | z- |
+00002f30: 0a20 2020 207c 201b 5b31 3b34 393b 3937  .    | .[1;49;97
+00002f40: 6d55 5443 204f 6666 7365 741b 5b30 6d20  mUTC Offset.[0m 
+00002f50: 2020 2020 2020 2020 207c 207a 6a20 7c0a           | zj |.
+00002f60: 2020 2020 7c2d 2d2d 2d2d 2d2d 2d2d 2d2d      |-----------
+00002f70: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00002f80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00002f90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d7c 0a20 2020  -----------|.   
+00002fa0: 207c 201b 5b31 3b34 393b 3937 6d41 534e   | .[1;49;97mASN
+00002fb0: 1b5b 306d 2020 2020 2020 2020 2020 2020  .[0m            
+00002fc0: 2020 2020 207c 207a 2d20 7c0a 2020 2020       | z- |.    
+00002fd0: 7c20 1b5b 313b 3439 3b39 376d 4953 501b  | .[1;49;97mISP.
+00002fe0: 5b30 6d20 2020 2020 2020 2020 2020 2020  [0m             
+00002ff0: 2020 2020 7c20 7253 0000 00da 0474 7970      | rS.....typ
+00003000: 65da 0963 6f6e 7469 6e65 6e74 da05 6973  e..continent..is
+00003010: 5f65 75da 0c63 616c 6c69 6e67 5f63 6f64  _eu..calling_cod
+00003020: 65da 0763 6170 6974 616c da07 626f 7264  e..capital..bord
+00003030: 6572 73da 0466 6c61 675a 0369 6d67 5a05  ers..flagZ.imgZ.
+00003040: 656d 6f6a 695a 0d65 6d6f 6a69 5f75 6e69  emojiZ.emoji_uni
+00003050: 636f 6465 da0a 636f 6e6e 6563 7469 6f6e  code..connection
+00003060: da06 646f 6d61 696e da02 6964 5a04 6162  ..domain..idZ.ab
+00003070: 6272 5a06 6973 5f64 7374 da06 6f66 6673  brZ.is_dst..offs
+00003080: 6574 da03 7574 635a 0c63 7572 7265 6e74  et..utcZ.current
+00003090: 5f74 696d 657a 2072 6576 6572 7365 2d69  _timez reverse-i
+000030a0: 702d 6c6f 6f6b 7570 2d73 6572 7665 722d  p-lookup-server-
+000030b0: 332d 6572 726f 727a 6a20 7c0a 2020 2020  3-errorzj |.    
+000030c0: 7c2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  |---------------
 000030d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 000030e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000030f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00003100: 2d2d 7c0a 2020 2020 7c20 1b5b 313b 3439  --|.    | .[1;49
-00003110: 3b39 316d 4661 696c 6564 2074 6f20 4665  ;91mFailed to Fe
-00003120: 7463 6820 696e 666f 726d 6174 696f 6e20  tch information 
-00003130: 6672 6f6d 2074 6869 7320 7365 7276 6572  from this server
-00003140: 211b 5b30 6d20 2020 2020 2020 207c 0a20  !.[0m        |. 
-00003150: 2020 20e2 9494 e294 80e2 9480 e294 80e2     .............
-00003160: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00003170: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00003180: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00003190: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-000031a0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-000031b0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-000031c0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-000031d0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-000031e0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-000031f0: 9480 e294 80e2 9480 e294 980a 2020 2020  ............    
-00003200: 724a 0000 00da 0474 7970 65da 0963 6f6e  rJ.....type..con
-00003210: 7469 6e65 6e74 da05 6973 5f65 75da 0c63  tinent..is_eu..c
-00003220: 616c 6c69 6e67 5f63 6f64 65da 0763 6170  alling_code..cap
-00003230: 6974 616c da07 626f 7264 6572 73da 0466  ital..borders..f
-00003240: 6c61 675a 0369 6d67 5a05 656d 6f6a 695a  lagZ.imgZ.emojiZ
-00003250: 0d65 6d6f 6a69 5f75 6e69 636f 6465 da0a  .emoji_unicode..
-00003260: 636f 6e6e 6563 7469 6f6e da06 646f 6d61  connection..doma
-00003270: 696e da02 6964 5a04 6162 6272 5a06 6973  in..idZ.abbrZ.is
-00003280: 5f64 7374 da06 6f66 6673 6574 da03 7574  _dst..offset..ut
-00003290: 635a 0c63 7572 7265 6e74 5f74 696d 657a  cZ.current_timez
-000032a0: 2072 6576 6572 7365 2d69 702d 6c6f 6f6b   reverse-ip-look
-000032b0: 7570 2d73 6572 7665 722d 332d 6572 726f  up-server-3-erro
-000032c0: 7261 3501 0000 1b5b 306d 2020 207c 0a20  ra5....[0m   |. 
-000032d0: 2020 207c 2053 6572 7665 7220 636f 6465     | Server code
-000032e0: 206e 616d 6520 203a 201b 5b31 3b34 393b   name  : .[1;49;
-000032f0: 3936 6d72 6576 6572 7365 2d69 702d 6c6f  96mreverse-ip-lo
-00003300: 6f6b 7570 2d73 6572 7665 722d 331b 5b30  okup-server-3.[0
-00003310: 6d20 2020 2020 2020 7c0a 2020 2020 7c2d  m       |.    |-
-00003320: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00003330: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00003340: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00003350: 2d2d 2d2d 2d7c 0a20 2020 207c 2049 4e46  -----|.    | INF
-00003360: 4f52 4d41 5449 4f4e 2020 2020 2020 2020  ORMATION        
-00003370: 207c 2044 4553 4352 4950 5449 4f4e 2020   | DESCRIPTION  
-00003380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003390: 2020 7c0a 2020 2020 7c2d 2d2d 2d2d 2d2d    |.    |-------
-000033a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000033b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000033c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d7c  ---------------|
-000033d0: 0a20 2020 207c 201b 5b31 3b34 393b 3937  .    | .[1;49;97
-000033e0: 6d49 5020 5479 7065 1b5b 306d 2020 2020  mIP Type.[0m    
-000033f0: 2020 2020 2020 2020 207c 207a 6a20 7c0a           | zj |.
-00003400: 2020 2020 7c2d 2d2d 2d2d 2d2d 2d2d 2d2d      |-----------
-00003410: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00003420: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00003430: 2d2d 2d2d 2d2d 2d2d 2d2d 2d7c 0a20 2020  -----------|.   
-00003440: 207c 201b 5b31 3b34 393b 3937 6d43 6f75   | .[1;49;97mCou
-00003450: 6e74 7279 2043 6170 6974 616c 1b5b 306d  ntry Capital.[0m
-00003460: 2020 2020 207c 207a 2d20 7c0a 2020 2020       | z- |.    
-00003470: 7c20 1b5b 313b 3439 3b39 376d 436f 6e74  | .[1;49;97mCont
-00003480: 696e 656e 741b 5b30 6d20 2020 2020 2020  inent.[0m       
-00003490: 2020 2020 7c20 7a2d 207c 0a20 2020 207c      | z- |.    |
-000034a0: 201b 5b31 3b34 393b 3937 6d53 6861 7269   .[1;49;97mShari
-000034b0: 6e67 2042 6f72 6465 7220 7769 7468 1b5b  ng Border with.[
-000034c0: 306d 207c 207a 2d20 7c0a 2020 2020 7c20  0m | z- |.    | 
-000034d0: 1b5b 313b 3439 3b39 376d 466c 6167 2045  .[1;49;97mFlag E
-000034e0: 6d6f 6a69 1b5b 306d 2020 2020 2020 2020  moji.[0m        
-000034f0: 2020 7c20 7a6a 207c 0a20 2020 207c 2d2d    | zj |.    |--
-00003500: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00003510: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00003520: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00003530: 2d2d 2d2d 7c0a 2020 2020 7c20 1b5b 313b  ----|.    | .[1;
-00003540: 3439 3b39 376d 5469 6d65 7a6f 6e65 1b5b  49;97mTimezone.[
-00003550: 306d 2020 2020 2020 2020 2020 2020 7c20  0m            | 
-00003560: 7a2d 207c 0a20 2020 207c 201b 5b31 3b34  z- |.    | .[1;4
-00003570: 393b 3937 6d54 696d 657a 6f6e 6520 4162  9;97mTimezone Ab
-00003580: 6272 1b5b 306d 2020 2020 2020 207c 207a  br.[0m       | z
-00003590: 2d20 7c0a 2020 2020 7c20 1b5b 313b 3439  - |.    | .[1;49
-000035a0: 3b39 376d 5469 6d65 7a6f 6e65 2069 7320  ;97mTimezone is 
-000035b0: 4453 541b 5b30 6d20 2020 2020 7c20 7a2d  DST.[0m     | z-
-000035c0: 207c 0a20 2020 207c 201b 5b31 3b34 393b   |.    | .[1;49;
-000035d0: 3937 6d54 696d 657a 6f6e 6520 4f66 6673  97mTimezone Offs
-000035e0: 6574 1b5b 306d 2020 2020 207c 207a 2d20  et.[0m     | z- 
-000035f0: 7c0a 2020 2020 7c20 1b5b 313b 3439 3b39  |.    | .[1;49;9
-00003600: 376d 5469 6d65 7a6f 6e65 2055 5443 1b5b  7mTimezone UTC.[
-00003610: 306d 2020 2020 2020 2020 7c20 7a2d 207c  0m        | z- |
-00003620: 0a20 2020 207c 201b 5b31 3b34 393b 3937  .    | .[1;49;97
-00003630: 6d43 7572 7265 6e74 2054 696d 651b 5b30  mCurrent Time.[0
-00003640: 6d20 2020 2020 2020 207c 207a 2d20 7c0a  m        | z- |.
-00003650: 2020 2020 7c20 1b5b 313b 3439 3b39 376d      | .[1;49;97m
-00003660: 446f 6d61 696e 1b5b 306d 2020 2020 2020  Domain.[0m      
-00003670: 2020 2020 2020 2020 7c20 758d 0100 001b          | u.....
-00003680: 5b30 6d20 2020 7c0a 2020 2020 7c20 5365  [0m   |.    | Se
-00003690: 7276 6572 2063 6f64 6520 6e61 6d65 2020  rver code name  
-000036a0: 3a20 1b5b 313b 3439 3b39 366d 7265 7665  : .[1;49;96mreve
-000036b0: 7273 652d 6970 2d6c 6f6f 6b75 702d 7365  rse-ip-lookup-se
-000036c0: 7276 6572 2d33 1b5b 306d 2020 2020 2020  rver-3.[0m      
-000036d0: 207c 0a20 2020 207c 2d2d 2d2d 2d2d 2d2d   |.    |--------
-000036e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000036f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00003700: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 7c0a  --------------|.
-00003710: 2020 2020 7c20 1b5b 313b 3439 3b39 316d      | .[1;49;91m
-00003720: 4661 696c 6564 2074 6f20 4665 7463 6820  Failed to Fetch 
-00003730: 696e 666f 726d 6174 696f 6e20 6672 6f6d  information from
-00003740: 2074 6869 7320 7365 7276 6572 211b 5b30   this server!.[0
-00003750: 6d20 2020 2020 2020 207c 0a20 2020 20e2  m        |.    .
-00003760: 9494 e294 80e2 9480 e294 80e2 9480 e294  ................
-00003770: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00003780: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00003790: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-000037a0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-000037b0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-000037c0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-000037d0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-000037e0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-000037f0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00003800: 80e2 9480 e294 980a 2020 2020 2910 7236  ........    ).r6
-00003810: 0000 0072 3700 0000 7217 0000 0072 3800  ...r7...r....r8.
-00003820: 0000 7239 0000 0072 3b00 0000 723f 0000  ..r9...r;...r?..
-00003830: 0072 4000 0000 da06 7261 6e64 6f6d da06  .r@.....random..
-00003840: 6368 6f69 6365 7212 0000 0072 1300 0000  choicer....r....
-00003850: da04 6a73 6f6e da0b 7374 6174 7573 5f63  ..json..status_c
-00003860: 6f64 65da 0945 7863 6570 7469 6f6e 7241  ode..ExceptionrA
-00003870: 0000 0029 365a 0a69 705f 6164 6472 6573  ...)6Z.ip_addres
-00003880: 735a 0c69 705f 6164 6472 6573 7365 7372  sZ.ip_addressesr
-00003890: 4b00 0000 5a0a 7261 6e64 6f6d 5f61 7069  K...Z.random_api
-000038a0: da08 7265 7370 6f6e 7365 5a0d 7265 7370  ..responseZ.resp
-000038b0: 6f6e 7365 5f6a 736f 6e72 4600 0000 724f  onse_jsonrF...rO
-000038c0: 0000 0072 5000 0000 5a0a 7265 6769 6f6e  ...rP...Z.region
-000038d0: 436f 6465 7251 0000 0072 5200 0000 7253  CoderQ...rR...rS
-000038e0: 0000 0072 1800 0000 725e 0000 0072 5f00  ...r....r^...r_.
-000038f0: 0000 7260 0000 0072 0e00 0000 7247 0000  ..r`...r....rG..
-00003900: 00da 0165 7256 0000 0072 5700 0000 7245  ...erV...rW...rE
-00003910: 0000 0072 5800 0000 7243 0000 0072 5900  ...rX...rC...rY.
-00003920: 0000 725a 0000 0072 5b00 0000 725c 0000  ..rZ...r[...r\..
-00003930: 0072 5d00 0000 7261 0000 0072 6200 0000  .r]...ra...rb...
-00003940: 7263 0000 0072 6400 0000 7265 0000 0072  rc...rd...re...r
-00003950: 6600 0000 7267 0000 0072 6800 0000 5a07  f...rg...rh...Z.
-00003960: 6970 5f74 7970 6572 6a00 0000 726b 0000  ip_typerj...rk..
-00003970: 0072 6c00 0000 726d 0000 0072 6e00 0000  .rl...rm...rn...
-00003980: 5a08 666c 6167 5f69 6d67 5a0a 666c 6167  Z.flag_imgZ.flag
-00003990: 5f65 6d6f 6a69 5a12 666c 6167 5f65 6d6f  _emojiZ.flag_emo
-000039a0: 6a69 5f75 6e69 636f 6465 7271 0000 005a  ji_unicoderq...Z
-000039b0: 0b74 696d 657a 6f6e 655f 6964 5a0d 7469  .timezone_idZ.ti
-000039c0: 6d65 7a6f 6e65 5f61 6262 725a 0f74 696d  mezone_abbrZ.tim
-000039d0: 657a 6f6e 655f 6973 5f64 7374 5a0f 7469  ezone_is_dstZ.ti
-000039e0: 6d65 7a6f 6e65 5f6f 6666 7365 745a 0c74  mezone_offsetZ.t
-000039f0: 696d 657a 6f6e 655f 7574 635a 1574 696d  imezone_utcZ.tim
-00003a00: 657a 6f6e 655f 6375 7272 656e 745f 7469  ezone_current_ti
-00003a10: 6d65 7215 0000 0072 1500 0000 7216 0000  mer....r....r...
-00003a20: 00da 0969 705f 6c6f 6f6b 7570 c300 0000  ...ip_lookup....
-00003a30: 7394 0200 0000 0304 0312 0108 0112 0108  s...............
-00003a40: 0104 031a 0114 030c 0110 0108 0104 031e  ................
-00003a50: 0120 0404 ff04 050e 030a 0104 0214 0108  . ..............
-00003a60: 031a 0108 0108 0108 0108 0108 0108 0108  ................
-00003a70: 0108 0108 0108 0108 010a 0208 0320 0120  ............. . 
-00003a80: 0120 0120 0120 0120 0120 0120 0120 0120  . . . . . . . . 
-00003a90: 0120 0120 0302 0202 fe04 0702 f904 0802  . . ............
-00003aa0: f804 0902 f704 0a02 f604 0b02 f504 0d02  ................
-00003ab0: f304 0e02 f204 0f02 f104 1002 f004 1202  ................
-00003ac0: ee04 1302 ed08 1608 0110 0210 0108 0102  ................
-00003ad0: 0202 fe08 0808 0126 030a 0104 0214 0108  .......&........
-00003ae0: 030c 0108 0108 0108 0108 0108 0108 0108  ................
-00003af0: 0108 0108 0108 0108 0108 0108 0108 0108  ................
-00003b00: 0108 0108 0108 0108 0108 0108 0108 0108  ................
-00003b10: 0108 0108 0108 010a 0208 0320 0120 0120  ........... . . 
-00003b20: 0120 0120 0120 0120 0120 0120 0120 0120  . . . . . . . . 
-00003b30: 0120 0120 0120 0120 0120 0120 0120 0120  . . . . . . . . 
-00003b40: 0120 0120 0120 0120 0120 0120 0120 0120  . . . . . . . . 
-00003b50: 0302 0202 fe04 0702 f904 0802 f804 0a02  ................
-00003b60: f604 0b02 f504 0c02 f404 0d02 f304 0e02  ................
-00003b70: f204 0f02 f104 1002 f004 1102 ef04 1302  ................
-00003b80: ed04 1402 ec04 1502 eb04 1602 ea04 1702  ................
-00003b90: e904 1802 e804 1902 e704 1a02 e604 1b02  ................
-00003ba0: e504 1d02 e304 1e02 e204 1f02 e104 2002  .............. .
-00003bb0: e004 2102 df04 2302 dd04 2402 dc08 2708  ..!...#...$...'.
-00003bc0: 0110 0206 0102 0202 fe08 0808 0116 030a  ................
-00003bd0: 0104 0214 0108 031a 0108 0108 0108 0108  ................
-00003be0: 0108 0108 0108 0108 0108 0108 0108 0108  ................
-00003bf0: 0108 0108 0108 0108 010c 010c 010c 010c  ................
-00003c00: 010c 010c 010c 010c 010c 010c 010c 010c  ................
-00003c10: 010e 0208 0320 0120 0120 0120 0120 0120  ..... . . . . . 
-00003c20: 0120 0120 0120 0120 0120 0120 0120 0120  . . . . . . . . 
-00003c30: 0120 0120 0120 0120 0120 0120 0120 0120  . . . . . . . . 
-00003c40: 0120 0120 0120 0120 0120 0120 0120 0302  . . . . . . . ..
-00003c50: 0202 fe04 0702 f904 0902 f704 0a02 f604  ................
-00003c60: 0b02 f504 0c02 f404 0d02 f304 0f02 f104  ................
-00003c70: 1002 f004 1102 ef04 1202 ee04 1302 ed04  ................
-00003c80: 1402 ec04 1602 ea04 1702 e904 1802 e804  ................
-00003c90: 1902 e704 1b02 e504 1c02 e404 1d02 e304  ................
-00003ca0: 1e02 e204 1f02 e104 2002 e004 2202 de04  ........ ..."...
-00003cb0: 2302 dd04 2402 dc08 2708 0110 0206 0102  #...$...'.......
-00003cc0: 0202 fe08 0808 0112 0272 7c00 0000 2903  .........r|...).
-00003cd0: 7201 0000 0072 0100 0000 7201 0000 0063  r....r....r....c
-00003ce0: 0c00 0000 0000 0000 0000 0000 0f00 0000  ................
-00003cf0: 0800 0000 4300 0000 73fc 0000 007c 0972  ....C...s....|.r
-00003d00: 087c 0a72 f874 00a0 01a1 006a 027d 0c7c  .|.r.t.....j.}.|
-00003d10: 0472 1c74 0383 0001 007c 0272 2c74 0364  .r.t.....|.r,t.d
-00003d20: 017c 0c14 0083 0101 0074 037c 0764 0264  .|.......t.|.d.d
-00003d30: 038d 0201 0074 047c 0083 017c 0c6b 0072  .....t.|...|.k.r
-00003d40: ca74 057c 0c74 047c 0083 0118 0064 041b  .t.|.t.|.....d..
-00003d50: 0083 017d 0d74 037c 017c 0d14 0064 0264  ...}.t.|.|...d.d
-00003d60: 038d 0201 0074 0364 057c 0664 0619 009b  .....t.d.|.d....
-00003d70: 0064 077c 0664 0819 009b 0064 077c 0664  .d.|.d.....d.|.d
-00003d80: 0419 009b 0064 099d 0764 0264 038d 0201  .....d...d.d....
-00003d90: 007c 0b72 a274 067c 0083 017d 0e6e 1074  .|.r.t.|...}.n.t
-00003da0: 0374 077c 0083 0164 0264 038d 0201 0074  .t.|...d.d.....t
-00003db0: 0364 0a64 0264 038d 0201 0074 037c 017c  .d.d.d.....t.|.|
-00003dc0: 0d14 0083 0101 0074 037c 0864 0264 038d  .......t.|.d.d..
-00003dd0: 0201 007c 0372 e674 0364 017c 0c14 0083  ...|.r.t.d.|....
-00003de0: 0101 007c 0572 f074 0383 0001 007c 0b72  ...|.r.t.....|.r
-00003df0: f87c 0e53 0064 0053 0029 0b4e 7503 0000  .|.S.d.S.).Nu...
-00003e00: 00e2 b8ba 720f 0000 0029 01da 0365 6e64  ....r....)...end
-00003e10: 724a 0000 007a 021b 5b72 0100 0000 fa01  rJ...z..[r......
-00003e20: 3b72 1e00 0000 da01 6dfa 041b 5b30 6d29  ;r......m...[0m)
-00003e30: 08da 026f 73da 1167 6574 5f74 6572 6d69  ...os..get_termi
-00003e40: 6e61 6c5f 7369 7a65 da07 636f 6c75 6d6e  nal_size..column
-00003e50: 7372 4100 0000 7240 0000 0072 3f00 0000  srA...r@...r?...
-00003e60: da05 696e 7075 7472 3b00 0000 290f da04  ..inputr;...)...
-00003e70: 7465 7874 da06 6365 6e74 6572 da07 6c69  text..center..li
-00003e80: 6e65 5f75 70da 096c 696e 655f 646f 776e  ne_up..line_down
-00003e90: da08 7370 6163 655f 7570 7223 0000 0072  ..space_upr#...r
-00003ea0: 2200 0000 da0f 6e6f 726d 616c 7478 745f  ".....normaltxt_
-00003eb0: 7374 6172 745a 0d6e 6f72 6d61 6c74 7874  startZ.normaltxt
-00003ec0: 5f65 6e64 5a04 6869 6465 5a0c 7665 7262  _endZ.hideZ.verb
-00003ed0: 6f73 655f 6d6f 6465 da0a 696e 7075 745f  ose_mode..input_
-00003ee0: 6d6f 6465 da05 7769 6474 685a 096e 6577  mode..widthZ.new
-00003ef0: 5f77 6964 7468 5a09 696e 7075 745f 7661  _widthZ.input_va
-00003f00: 7272 1500 0000 7215 0000 0072 1600 0000  rr....r....r....
-00003f10: 7237 0000 0031 0200 0073 2200 0000 0001  r7...1...s".....
-00003f20: 0802 0a03 0a01 1002 0c02 0c01 1401 1001  ................
-00003f30: 2c01 0e01 1001 0c01 0c02 0c02 1001 0a02  ,...............
-00003f40: 7237 0000 0063 0100 0000 0000 0000 0000  r7...c..........
-00003f50: 0000 0800 0000 0800 0000 4300 0000 73fa  ..........C...s.
-00003f60: 0000 007a d47c 0064 0117 0074 0074 01a0  ...z.|.d...t.t..
-00003f70: 0264 02a1 0183 0117 0064 0317 007d 0174  .d.......d...}.t
-00003f80: 03a0 04a1 007d 0274 03a0 05a1 007d 037c  .....}.t.....}.|
-00003f90: 0264 0417 007c 0117 007d 0464 057c 019b  .d...|...}.d.|..
-00003fa0: 0064 067c 049b 0064 079d 057d 0574 067c  .d.|...d...}.t.|
-00003fb0: 0583 0101 0074 077c 0464 0883 028f 1a7d  .....t.|.d.....}
-00003fc0: 067c 06a0 0874 09a1 0101 0057 0064 0004  .|...t.....W.d..
-00003fd0: 0004 0083 0301 006e 1031 0073 7c30 0001  .......n.1.s|0..
-00003fe0: 0001 0001 0059 0001 0074 0a64 0967 0064  .....Y...t.d.g.d
-00003ff0: 0aa2 0164 0b64 0b64 0c8d 0401 007c 0364  ...d.d.d.....|.d
-00004000: 0d6b 0272 b664 0e7c 049b 0064 0f7c 049b  .k.r.d.|...d.|..
-00004010: 0064 109d 057d 076e 1264 117c 049b 0064  .d...}.n.d.|...d
-00004020: 127c 049b 0064 109d 057d 0774 067c 0783  .|...d...}.t.|..
-00004030: 0101 0057 0064 0b53 0001 0001 0001 0074  ...W.d.S.......t
-00004040: 0a64 1367 0064 14a2 0164 0b64 158d 0301  .d.g.d...d.d....
-00004050: 0059 0064 1653 0030 0064 0053 0029 174e  .Y.d.S.0.d.S.).N
-00004060: da01 5f7a 1125 642d 256d 2d25 595f 2548  .._z.%d-%m-%Y_%H
-00004070: 2d25 4d2d 2553 7a04 2e74 7874 7234 0000  -%M-%Sz..txtr4..
-00004080: 007a 2f0a 2020 2020 1b5b 313b 3439 3b39  .z/.    .[1;49;9
-00004090: 336d 5b23 5d20 4f75 7470 7574 2046 696c  3m[#] Output Fil
-000040a0: 6520 4e61 6d65 3a20 1b5b 313b 3439 3b39  e Name: .[1;49;9
-000040b0: 376d 7a33 1b5b 306d 0a20 2020 201b 5b31  7mz3.[0m.    .[1
-000040c0: 3b34 393b 3933 6d5b 235d 204f 7574 7075  ;49;93m[#] Outpu
-000040d0: 7420 4669 6c65 2050 6174 683a 201b 5b31  t File Path: .[1
-000040e0: 3b34 393b 3937 6d7a 0d1b 5b30 6d0a 2020  ;49;97mz..[0m.  
-000040f0: 2020 2020 2020 da01 777a 3120 2020 205b        ..wz1    [
-00004100: 2b5d 2045 7863 7574 6520 666f 6c6c 6f77  +] Excute follow
-00004110: 696e 6720 636f 6d6d 616e 6473 2074 6f20  ing commands to 
-00004120: 7669 6577 206f 7574 7075 743a 721d 0000  view output:r...
-00004130: 0054 2903 7222 0000 0072 2300 0000 7289  .T).r"...r#...r.
-00004140: 0000 00da 026e 747a 1b20 2020 201b 5b31  .....ntz.    .[1
-00004150: 3b34 393b 3932 6d3e 2073 6865 6c6c 206d  ;49;92m> shell m
-00004160: 6f72 6520 7a20 1b5b 306d 0a20 2020 201b  ore z .[0m.    .
-00004170: 5b31 3b34 393b 3932 6d3e 2073 6865 6c6c  [1;49;92m> shell
-00004180: 2074 7970 6520 7280 0000 007a 1a20 2020   type r....z.   
-00004190: 201b 5b31 3b34 393b 3932 6d3e 2073 6865   .[1;49;92m> she
-000041a0: 6c6c 2063 6174 207a 201b 5b30 6d0a 2020  ll cat z .[0m.  
-000041b0: 2020 1b5b 313b 3439 3b39 326d 3e20 7368    .[1;49;92m> sh
-000041c0: 656c 6c20 6c65 7373 207a 2220 2020 205b  ell less z"    [
-000041d0: 215d 204f 7574 7075 7420 636f 756c 6420  !] Output could 
-000041e0: 6e6f 7420 6265 2073 6176 6564 2172 2600  not be saved!r&.
-000041f0: 0000 7221 0000 0046 290b 723b 0000 00da  ..r!...F).r;....
-00004200: 0474 696d 65da 0873 7472 6674 696d 6572  .time..strftimer
-00004210: 8100 0000 da06 6765 7463 7764 da05 756e  ......getcwd..un
-00004220: 616d 6572 4100 0000 da04 6f70 656e da05  amerA.....open..
-00004230: 7772 6974 6572 3600 0000 7237 0000 0029  writer6...r7...)
-00004240: 08da 0770 7276 5f63 6d64 da08 6669 6c65  ...prv_cmd..file
-00004250: 6e61 6d65 da03 7077 64da 076f 735f 6e61  name..pwd..os_na
-00004260: 6d65 da04 7061 7468 5a0e 6669 6c65 5f73  me..pathZ.file_s
-00004270: 6176 655f 696e 666f da01 665a 0765 7865  ave_info..fZ.exe
-00004280: 5f63 6d64 7215 0000 0072 1500 0000 7216  _cmdr....r....r.
-00004290: 0000 00da 0b73 6176 655f 6f75 7470 7574  .....save_output
-000042a0: 4c02 0000 732c 0000 0000 0102 011a 0108  L...s,..........
-000042b0: 0108 010c 0202 0102 ff04 0202 fe08 0408  ................
-000042c0: 020c 0128 0214 0208 0114 0312 0208 0206  ...(............
-000042d0: 0106 0112 0172 9c00 0000 6300 0000 0000  .....r....c.....
-000042e0: 0000 0000 0000 0005 0000 0007 0000 0043  ...............C
-000042f0: 0000 0073 8000 0000 7a60 6401 6402 6901  ...s....z`d.d.i.
-00004300: 7d00 7400 6a01 6403 7402 7403 a004 6404  }.t.j.d.t.t...d.
-00004310: 6405 a102 8301 1700 7c00 6406 8d02 7d01  d.......|.d...}.
-00004320: 7c01 6a05 6407 6b02 725e 7406 a007 7c01  |.j.d.k.r^t...|.
-00004330: 6a08 6408 a102 7d02 7c02 6a09 6409 640a  j.d...}.|.j.d.d.
-00004340: 640b 6901 640c 8d02 6a08 a00a a100 7d03  d.i.d...j.....}.
-00004350: 7c03 5700 5300 5700 6e0c 0100 0100 0100  |.W.S.W.n.......
-00004360: 5900 6e02 3000 6700 640d a201 7d04 7403  Y.n.0.g.d...}.t.
-00004370: a00b 7c04 a101 5300 290e 4e72 4900 0000  ..|...S.).NrI...
-00004380: 7a44 4d6f 7a69 6c6c 612f 352e 3020 2858  zDMozilla/5.0 (X
-00004390: 3131 3b20 4c69 6e75 7820 7838 365f 3634  11; Linux x86_64
-000043a0: 3b20 7276 3a39 302e 3029 2047 6563 6b6f  ; rv:90.0) Gecko
-000043b0: 2f32 3031 3030 3130 3120 4669 7265 666f  /20100101 Firefo
-000043c0: 782f 3930 2e30 7a20 6874 7470 733a 2f2f  x/90.0z https://
-000043d0: 7777 772e 6578 706c 6f69 742d 6462 2e63  www.exploit-db.c
-000043e0: 6f6d 2f67 6864 622f 69e8 0300 0069 401f  om/ghdb/i....i@.
-000043f0: 0000 2901 724b 0000 0072 4c00 0000 7a0b  ..).rK...rL...z.
-00004400: 6874 6d6c 2e70 6172 7365 725a 0268 31da  html.parserZ.h1.
-00004410: 0563 6c61 7373 7a0a 6361 7264 2d74 6974  .classz.card-tit
-00004420: 6c65 2901 da05 6174 7472 7329 167a 1d73  le)...attrs).z.s
-00004430: 6974 653a 646f 6d61 696e 2e63 6f6d 2066  ite:domain.com f
-00004440: 696c 6574 7970 653a 2070 6466 7a0f 696e  iletype: pdfz.in
-00004450: 7572 6c3a 2070 6173 7377 6f72 6475 1500  url: passwordu..
-00004460: 0000 696e 7465 7874 3ae2 809d 7573 6572  ..intext:...user
-00004470: 6e61 6d65 e280 9d7a 0c66 696c 6574 7970  name...z.filetyp
-00004480: 653a 786c 7375 1b00 0000 6669 6c65 7479  e:xlsu....filety
-00004490: 7065 3a74 7874 20e2 809c 7573 6572 6e61  pe:txt ...userna
-000044a0: 6d65 e280 9d75 4800 0000 6669 6c65 7479  me...uH...filety
-000044b0: 7065 3a6c 6f67 20e2 809c 5048 5020 5061  pe:log ...PHP Pa
-000044c0: 7273 6520 6572 726f 72e2 809d 207c 20e2  rse error... | .
-000044d0: 809c 5048 5020 5761 726e 696e 67e2 809d  ..PHP Warning...
-000044e0: 207c 20e2 809c 5048 5020 4572 726f 72e2   | ...PHP Error.
-000044f0: 809d 7517 0000 0069 6e74 6974 6c65 3a20  ..u....intitle: 
-00004500: e280 9c69 6e64 6578 206f 66e2 809d 7522  ...index of...u"
-00004510: 0000 0069 6e74 6974 6c65 3a20 e280 9c69  ...intitle: ...i
-00004520: 6e64 6578 206f 66e2 809d 20e2 809c 2e67  ndex of... ....g
-00004530: 6974 e280 9d75 2200 0000 696e 7469 746c  it...u"...intitl
-00004540: 653a 20e2 809c 696e 6465 7820 6f66 e280  e: ...index of..
-00004550: 9d20 e280 9c2e 7376 6ee2 809d 7519 0000  . ....svn...u...
-00004560: 0069 6e75 726c 3ae2 809d 7669 6577 6572  .inurl:...viewer
-00004570: 6672 616d 653f 6d6f 6465 7528 0000 0069  frame?modeu(...i
-00004580: 6e75 726c 3ae2 809d 4d75 6c74 6943 616d  nurl:...MultiCam
-00004590: 6572 6146 7261 6d65 3f4d 6f64 653d 4d6f  eraFrame?Mode=Mo
-000045a0: 7469 6f6e e280 9d75 2b00 0000 696e 7469  tion...u+...inti
-000045b0: 746c 653a 20e2 809c 696e 6465 7820 6f66  tle: ...index of
-000045c0: e280 9d20 e280 9c2e 6261 7368 5f68 6973  ... ....bash_his
-000045d0: 746f 7279 e280 9d75 1b00 0000 696e 7465  tory...u....inte
-000045e0: 7874 3a20 e280 9c4c 6173 7420 6d6f 6469  xt: ...Last modi
-000045f0: 6669 6564 e280 9d75 1800 0000 696e 7465  fied...u....inte
-00004600: 7874 3a20 e280 9c49 6e64 6578 206f 6620  xt: ...Index of 
-00004610: 2fe2 809d 751e 0000 0069 6e74 6578 743a  /...u....intext:
-00004620: 20e2 809c 5061 7265 6e74 2044 6972 6563   ...Parent Direc
-00004630: 746f 7279 e280 9d75 1200 0000 696e 7572  tory...u....inur
-00004640: 6c3a 20e2 809c 6164 6d69 6ee2 809d 7512  l: ...admin...u.
-00004650: 0000 0069 6e75 726c 3a20 e280 9c6c 6f67  ...inurl: ...log
-00004660: 696e e280 9d75 1e00 0000 696e 7572 6c3a  in...u....inurl:
-00004670: 20e2 809c 6c6f 6769 6ee2 809d 20e2 809c   ...login... ...
-00004680: 6164 6d69 6ee2 809d 7529 0000 0069 6e75  admin...u)...inu
-00004690: 726c 3a20 e280 9c6c 6f67 696e e280 9d20  rl: ...login... 
-000046a0: e280 9c61 646d 696e e280 9d20 e280 9c75  ...admin... ...u
-000046b0: 7365 72e2 809d 751b 0000 0069 6e74 6578  ser...u....intex
-000046c0: 743a e280 9d70 7269 7661 6379 2070 6f6c  t:...privacy pol
-000046d0: 6963 79e2 809d 7a22 2270 6173 7377 6f72  icy...z""passwor
-000046e0: 6473 2e74 7874 2220 696e 7469 746c 653a  ds.txt" intitle:
-000046f0: 2249 6e64 6578 206f 6622 7517 0000 0069  "Index of"u....i
-00004700: 6e74 6578 743a e280 9d40 676d 6169 6c2e  ntext:...@gmail.
-00004710: 636f 6de2 809d 290c 7212 0000 0072 1300  com...).r....r..
-00004720: 0000 723b 0000 0072 7500 0000 da07 7261  ..r;...ru.....ra
-00004730: 6e64 696e 7472 7800 0000 da03 6273 345a  ndintrx.....bs4Z
-00004740: 0d42 6561 7574 6966 756c 536f 7570 7285  .BeautifulSoupr.
-00004750: 0000 00da 0466 696e 6472 3d00 0000 7276  .....findr=...rv
-00004760: 0000 0029 0572 4b00 0000 da0a 646f 726b  ...).rK.....dork
-00004770: 5f71 7565 7279 5a0b 7061 7273 6564 5f68  _queryZ.parsed_h
-00004780: 746d 6c72 5500 0000 5a10 6c6f 6361 6c5f  tmlrU...Z.local_
-00004790: 646f 726b 5f71 7565 7279 7215 0000 0072  dork_queryr....r
-000047a0: 1500 0000 7216 0000 0072 a200 0000 6b02  ....r....r....k.
-000047b0: 0000 7316 0000 0000 0202 0108 011e 030a  ..s.............
-000047c0: 020e 0318 020a 0106 0106 0308 0772 a200  .............r..
-000047d0: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
-000047e0: 0000 0009 0000 0043 0000 0073 9a00 0000  .......C...s....
-000047f0: 7400 a001 7400 6a02 6401 6b02 7212 6402  t...t.j.d.k.r.d.
-00004800: 6e02 6403 a101 0100 7403 6404 6405 6406  n.d.....t.d.d.d.
-00004810: 6407 7404 a005 6700 6408 a201 a101 6703  d.t...g.d.....g.
-00004820: 6409 640a 8d04 0100 7403 640b 6405 6406  d.d.....t.d.d.d.
-00004830: 6407 7404 a005 6700 6408 a201 a101 6703  d.t...g.d.....g.
-00004840: 640c 8d03 0100 7403 640d 6405 6406 6407  d.....t.d.d.d.d.
-00004850: 7404 a005 6700 6408 a201 a101 6703 6409  t...g.d.....g.d.
-00004860: 640e 8d04 0100 7403 640f 6405 6406 6407  d.....t.d.d.d.d.
-00004870: 7404 a005 6700 6408 a201 a101 6703 6409  t...g.d.....g.d.
-00004880: 640e 8d04 0100 6400 5300 2910 4e72 8f00  d.....d.S.).Nr..
-00004890: 0000 da03 636c 7372 0800 0000 7577 0000  ....clsr....uw..
-000048a0: 00e2 9480 20e2 9692 e296 88e2 9680 e296  .... ...........
-000048b0: 80e2 9688 20e2 9692 e296 88e2 9691 e296  .... ...........
-000048c0: 92e2 9688 20e2 9688 e296 80e2 9680 e296  .... ...........
-000048d0: 8820 e296 92e2 9688 e296 80e2 9684 e296  . ..............
-000048e0: 80e2 9688 20e2 9692 e296 88e2 9680 e296  .... ...........
-000048f0: 80e2 9688 20e2 9692 e296 88e2 9680 e296  .... ...........
-00004900: 80e2 9680 20e2 9692 e296 88e2 9680 e296  .... ...........
-00004910: 80e2 9688 20e2 9480 7230 0000 0072 1e00  .... ...r0...r..
-00004920: 0000 721f 0000 0029 0772 2700 0000 e95c  ..r....).r'....\
-00004930: 0000 0072 2000 0000 e95e 0000 00e9 5f00  ...r ....^...._.
-00004940: 0000 e960 0000 00e9 6100 0000 5429 0372  ...`....a...T).r
-00004950: 8600 0000 7222 0000 0072 8900 0000 7577  ....r"...r....uw
-00004960: 0000 00e2 9480 20e2 9692 e296 88e2 9684  ...... .........
-00004970: e296 84e2 9688 20e2 9692 e296 88e2 9680  ...... .........
-00004980: e296 80e2 9688 20e2 9688 e296 84e2 9680  ...... .........
-00004990: e296 8820 e296 92e2 9688 e296 92e2 9688  ... ............
-000049a0: e296 92e2 9688 20e2 9692 e296 88e2 9680  ...... .........
-000049b0: e296 80e2 9684 20e2 9692 e296 88e2 9680  ...... .........
-000049c0: e296 80e2 9680 20e2 9692 e296 88e2 9684  ...... .........
-000049d0: e296 84e2 9680 20e2 9480 2902 7286 0000  ...... ...).r...
-000049e0: 0072 2200 0000 7577 0000 00e2 9480 20e2  .r"...uw...... .
-000049f0: 9692 e296 88e2 9691 e296 91e2 9691 20e2  .............. .
-00004a00: 9692 e296 88e2 9691 e296 92e2 9688 20e2  .............. .
-00004a10: 9688 e296 84e2 9684 e296 8820 e296 92e2  ........... ....
-00004a20: 9688 e296 91e2 9691 e296 92e2 9688 20e2  .............. .
-00004a30: 9692 e296 88e2 9684 e296 84e2 9688 20e2  .............. .
-00004a40: 9692 e296 88e2 9684 e296 84e2 9684 20e2  .............. .
-00004a50: 9692 e296 88e2 9691 e296 92e2 9688 20e2  .............. .
-00004a60: 9480 2903 7286 0000 0072 2200 0000 7223  ..).r....r"...r#
-00004a70: 0000 007a 294f 5349 4e54 2d46 5241 4d45  ...z)OSINT-FRAME
-00004a80: 574f 524b 2020 2020 2020 2020 2020 2020  WORK            
-00004a90: 2020 2020 2020 2040 7334 3172 346a 2906         @s41r4j).
-00004aa0: 7281 0000 00da 0673 7973 7465 6dda 046e  r......system..n
-00004ab0: 616d 6572 3700 0000 7275 0000 0072 7600  amer7...ru...rv.
-00004ac0: 0000 7215 0000 0072 1500 0000 7215 0000  ..r....r....r...
-00004ad0: 0072 1600 0000 da04 6c6f 676f 8702 0000  .r......logo....
-00004ae0: 730a 0000 0000 0218 0320 011e 0120 0172  s........ ... .r
-00004af0: ab00 0000 6302 0000 0000 0000 0000 0000  ....c...........
-00004b00: 0004 0000 0003 0000 0003 0000 0073 3200  .............s2.
-00004b10: 0000 7400 7d02 8700 6601 6401 6402 8408  ..t.}...f.d.d...
-00004b20: 7c02 4400 8301 7d03 7c01 7401 7c03 8301  |.D...}.|.t.|...
-00004b30: 6b00 722a 7c03 7c01 1900 5300 6400 5300  k.r*|.|...S.d.S.
-00004b40: 6400 5300 2903 4e63 0100 0000 0000 0000  d.S.).Nc........
-00004b50: 0000 0000 0200 0000 0500 0000 1300 0000  ................
-00004b60: 731a 0000 0067 007c 005d 127d 017c 01a0  s....g.|.].}.|..
-00004b70: 0088 00a1 0172 047c 0191 0271 0453 0072  .....r.|...q.S.r
-00004b80: 1500 0000 2901 da0a 7374 6172 7473 7769  ....)...startswi
-00004b90: 7468 2902 da02 2e30 da01 69a9 0172 8500  th)....0..i..r..
-00004ba0: 0000 7215 0000 0072 1600 0000 da0a 3c6c  ..r....r......<l
-00004bb0: 6973 7463 6f6d 703e 9302 0000 f300 0000  istcomp>........
-00004bc0: 007a 1d63 6f6d 706c 6574 6572 2e3c 6c6f  .z.completer.<lo
-00004bd0: 6361 6c73 3e2e 3c6c 6973 7463 6f6d 703e  cals>.<listcomp>
-00004be0: 2902 da12 6176 616c 6961 626c 655f 636f  )...avaliable_co
-00004bf0: 6d6d 616e 6473 7240 0000 0029 0472 8500  mmandsr@...).r..
-00004c00: 0000 da05 7374 6174 65da 0863 6f6d 6d61  ....state..comma
-00004c10: 6e64 73da 076f 7074 696f 6e73 7215 0000  nds..optionsr...
-00004c20: 0072 af00 0000 7216 0000 00da 0963 6f6d  .r....r......com
-00004c30: 706c 6574 6572 9102 0000 730a 0000 0000  pleter....s.....
-00004c40: 0104 0112 010c 0108 0272 b600 0000 6300  .........r....c.
-00004c50: 0000 0000 0000 0000 0000 0020 0000 000f  ........... ....
-00004c60: 0000 0043 0000 0073 f009 0000 7400 7326  ...C...s....t.s&
-00004c70: 7401 6401 6402 6403 7402 a003 6700 6404  t.d.d.d.t...g.d.
-00004c80: a201 a101 6703 6405 6405 6405 6406 8d05  ....g.d.d.d.d...
-00004c90: 0100 6700 6407 a201 7d00 7c00 6408 1900  ..g.d...}.|.d...
-00004ca0: 7d01 6409 7d02 640a 7404 7405 a006 a100  }.d.}.d.t.t.....
-00004cb0: 8301 1700 640b 1700 640c 7407 640d 7408  ....d...d.t.d.t.
-00004cc0: 7404 7405 a006 a100 8301 8301 1800 8301  t.t.............
-00004cd0: 1400 1700 7d03 640a 7404 7405 a009 a100  ....}.d.t.t.....
-00004ce0: 6a0a 8301 1700 640b 1700 640c 7407 640d  j.....d...d.t.d.
-00004cf0: 7408 7404 7405 a009 a100 6a0a 8301 8301  t.t.t.....j.....
-00004d00: 1800 8301 1400 1700 7d04 640a 7404 7405  ........}.d.t.t.
-00004d10: a009 a100 6a0b 8301 1700 640b 1700 640c  ....j.....d...d.
-00004d20: 7407 640d 7408 7404 7405 a009 a100 6a0b  t.d.t.t.t.....j.
-00004d30: 8301 8301 1800 8301 1400 1700 7d05 640a  ............}.d.
-00004d40: 7404 740c a00d a100 6a0e 8301 1700 640e  t.t.....j.....d.
-00004d50: 1700 640b 1700 640c 7407 640f 7408 7404  ..d...d.t.d.t.t.
-00004d60: 740c a00d a100 6a0e 8301 8301 1800 8301  t.....j.........
-00004d70: 1400 1700 7d06 640a 7404 740c a00f a100  ....}.d.t.t.....
-00004d80: 8301 1700 640e 1700 640b 1700 640c 7407  ....d...d...d.t.
-00004d90: 6410 7408 7404 740c a00f a100 8301 8301  d.t.t.t.........
-00004da0: 1800 8301 1400 1700 7d07 640a 7404 740c  ........}.d.t.t.
-00004db0: a010 6411 a101 6a0e 8301 1700 640e 1700  ..d...j.....d...
-00004dc0: 640b 1700 640c 7407 640f 7408 7404 740c  d...d.t.d.t.t.t.
-00004dd0: a010 6411 a101 6a0e 8301 8301 1800 8301  ..d...j.........
-00004de0: 1400 1700 7d08 6412 640c 7407 640d 7408  ....}.d.d.t.d.t.
-00004df0: 7404 6413 8301 8301 1800 8301 1400 1700  t.d.............
-00004e00: 7d09 6414 7c03 9b00 6415 7c04 9b00 6416  }.d.|...d.|...d.
-00004e10: 7c05 9b00 6417 7c06 9b00 6418 7c07 9b00  |...d.|...d.|...
-00004e20: 6419 7c08 9b00 641a 7c09 9b00 641b 9d0f  d.|...d.|...d...
-00004e30: 7d0a 641c 7d0b 641d 7d0c 7411 a012 641e  }.d.}.d.}.t...d.
-00004e40: a101 0100 7411 a013 7414 a101 0100 641f  ....t...t.....d.
-00004e50: 6420 6702 7d0d 7c0d 6402 1900 7d0e 7401  d g.}.|.d...}.t.
-00004e60: 6421 7c03 a015 a100 9b00 6422 7c01 9b00  d!|.......d"|...
-00004e70: 6423 7c0e 9b00 9d06 6405 6405 6424 8d03  d#|.....d.d.d$..
-00004e80: a015 a100 7d0f 7c0f 6425 6b02 9002 723c  ....}.|.d%k...r<
-00004e90: 7c00 6402 1900 7d01 641d 6116 7417 7c0b  |.d...}.d.a.t.|.
-00004ea0: 8301 0100 9007 6ea8 7c0f 6400 6426 8502  ......n.|.d.d&..
-00004eb0: 1900 6425 6b02 9004 7270 7c0f 6427 1700  ..d%k...rp|.d'..
-00004ec0: 6426 1900 640c 6b02 9004 7250 7c0f 6428  d&..d.k...rP|.d(
-00004ed0: 6400 8502 1900 7d0f 7c0f 6425 6b02 9002  d.....}.|.d%k...
-00004ee0: 728e 7c00 6402 1900 7d01 6429 7d10 7417  r.|.d...}.d)}.t.
-00004ef0: 7c10 8301 0100 9004 7168 7c0f 642a 6b02  |.......qh|.d*k.
-00004f00: 9002 73a2 7c0f 642b 6b02 9002 72ba 7c00  ..s.|.d+k...r.|.
-00004f10: 6402 1900 7d01 642c 7d11 7417 7c11 8301  d...}.d,}.t.|...
-00004f20: 0100 9004 7168 7c0f 642d 6b02 9002 72dc  ....qh|.d-k...r.
-00004f30: 7c00 6402 1900 7d01 642e 7d12 7417 7c12  |.d...}.d.}.t.|.
-00004f40: 8301 0100 9004 7168 7c0f 642f 6b02 9002  ......qh|.d/k...
-00004f50: 72fe 7c00 6402 1900 7d01 6430 7d13 7417  r.|.d...}.d0}.t.
-00004f60: 7c13 8301 0100 9004 7168 7c0f 6431 6b02  |.......qh|.d1k.
-00004f70: 9003 7220 7c00 6402 1900 7d01 6432 7d14  ..r |.d...}.d2}.
-00004f80: 7417 7c14 8301 0100 9004 7168 7c0f 6433  t.|.......qh|.d3
-00004f90: 6b02 9003 7242 7c00 6402 1900 7d01 6434  k...rB|.d...}.d4
-00004fa0: 7d15 7417 7c15 8301 0100 9004 7168 7c0f  }.t.|.......qh|.
-00004fb0: 6435 6b02 9003 7262 7c00 6402 1900 7d01  d5k...rb|.d...}.
-00004fc0: 6436 7d16 7417 7c16 8301 0100 6eec 7c0f  d6}.t.|.....n.|.
-00004fd0: 6400 6428 8502 1900 6437 6b02 9003 728a  d.d(....d7k...r.
-00004fe0: 7c00 6402 1900 7d01 6438 7d17 7417 7c17  |.d...}.d8}.t.|.
-00004ff0: 8301 0100 6ec4 7c0f 6439 6b02 9003 72aa  ....n.|.d9k...r.
-00005000: 7c00 6402 1900 7d01 643a 7d18 7417 7c18  |.d...}.d:}.t.|.
-00005010: 8301 0100 6ea4 7c0f 643b 6b02 9003 72ca  ....n.|.d;k...r.
-00005020: 7c00 6402 1900 7d01 643c 7d19 7417 7c19  |.d...}.d<}.t.|.
-00005030: 8301 0100 6e84 7c0f 643d 6b02 9003 72ea  ....n.|.d=k...r.
-00005040: 7c00 6402 1900 7d01 643e 7d1a 7417 7c1a  |.d...}.d>}.t.|.
-00005050: 8301 0100 6e64 7c0f 643f 6b02 9004 7216  ....nd|.d?k...r.
-00005060: 7c00 6402 1900 7d01 6440 7c03 a015 a100  |.d...}.d@|.....
-00005070: 9b00 6441 9d03 7d1b 7417 7c1b 8301 0100  ..dA..}.t.|.....
-00005080: 6e38 7c0f 6442 6b02 9004 7236 7c00 6402  n8|.dBk...r6|.d.
-00005090: 1900 7d01 6443 7d1c 7417 7c1c 8301 0100  ..}.dC}.t.|.....
-000050a0: 6e18 7c00 6444 1900 7d01 7401 6445 6700  n.|.dD..}.t.dEg.
-000050b0: 6446 a201 6447 8d02 0100 6e18 7c00 6444  dF..dG....n.|.dD
-000050c0: 1900 7d01 7401 6448 6700 6446 a201 6447  ..}.t.dHg.dF..dG
-000050d0: 8d02 0100 641d 6116 9005 6e74 7c0f 642a  ....d.a...nt|.d*
-000050e0: 6b02 9004 7384 7c0f 642b 6b02 9004 72a8  k...s.|.d+k...r.
-000050f0: 7401 6449 6402 6403 7402 a003 6700 6404  t.dId.d.t...g.d.
-00005100: a201 a101 6703 6447 8d02 0100 7418 8201  ....g.dG....t...
-00005110: 9005 6e3c 7c0f 642d 6b02 9004 72ea 7c00  ..n<|.d-k...r.|.
-00005120: 6402 1900 7d01 641d 6116 7401 644a 6700  d...}.d.a.t.dJg.
-00005130: 644b a201 6405 644c 8d03 0100 7401 644d  dK..d.dL....t.dM
-00005140: 7419 8300 1700 6700 644e a201 6447 8d02  t.....g.dN..dG..
-00005150: 0100 9004 6efa 7c0f 642f 6b02 9005 720c  ....n.|.d/k...r.
-00005160: 7c00 6402 1900 7d01 641d 6116 7417 7c02  |.d...}.d.a.t.|.
-00005170: 8301 0100 9004 6ed8 7c0f 6431 6b02 9006  ......n.|.d1k...
-00005180: 720c 7401 644f 6700 644b a201 6405 644c  r.t.dOg.dK..d.dL
-00005190: 8d03 0100 7aa6 741a a01b 6450 a101 0100  ....z.t...dP....
-000051a0: 7401 6451 6700 644e a201 6447 8d02 0100  t.dQg.dN..dG....
-000051b0: 7a16 741a a01b 6452 a101 a01c a100 6453  z.t...dR......dS
-000051c0: 1900 7d1d 5700 6e4c 0100 0100 0100 7a10  ..}.W.nL......z.
-000051d0: 741a a01b 6454 a101 6a1d 7d1d 5700 6e2e  t...dT..j.}.W.n.
-000051e0: 0100 0100 0100 7a10 741a a01b 6455 a101  ......z.t...dU..
-000051f0: 6a1d 7d1d 5700 6e10 0100 0100 0100 6456  j.}.W.n.......dV
-00005200: 7d1d 5900 6e02 3000 5900 6e02 3000 5900  }.Y.n.0.Y.n.0.Y.
-00005210: 6e02 3000 7c1d 9005 72c4 7401 6457 7c1d  n.0.|...r.t.dW|.
-00005220: 9b00 9d02 6700 644e a201 6447 8d02 0100  ....g.dN..dG....
-00005230: 7c00 6408 1900 7d01 5700 6e34 0100 0100  |.d...}.W.n4....
-00005240: 0100 7401 6458 6700 6446 a201 6447 8d02  ..t.dXg.dF..dG..
-00005250: 0100 7401 6459 6700 644e a201 6447 8d02  ..t.dYg.dN..dG..
-00005260: 0100 7c00 6444 1900 7d01 5900 6e02 3000  ..|.dD..}.Y.n.0.
-00005270: 641d 6116 9003 6ed8 7c0f 6433 6b02 9006  d.a...n.|.d3k...
-00005280: 7240 7c00 6408 1900 7d01 641d 6116 7405  r@|.d...}.d.a.t.
-00005290: a01e 7405 6a1f 645a 6b02 9006 7236 645b  ..t.j.dZk...r6d[
-000052a0: 6e02 6433 a101 0100 9003 6ea4 7c0f 6435  n.d3......n.|.d5
-000052b0: 6b02 9006 72a4 7401 645c 6700 644b a201  k...r.t.d\g.dK..
-000052c0: 6405 644c 8d03 0100 7416 641d 6b02 9006  d.dL....t.d.k...
-000052d0: 7280 7401 645d 6700 6446 a201 6447 8d02  r.t.d]g.dF..dG..
-000052e0: 0100 7c00 645e 1900 7d01 6e1c 7420 7c0c  ..|.d^..}.n.t |.
-000052f0: 8301 9006 7294 7c00 6408 1900 7d01 6e08  ....r.|.d...}.n.
-00005300: 7c00 6444 1900 7d01 641d 6116 9003 6e40  |.dD..}.d.a...n@
-00005310: 7c0f 6437 6b02 9006 72ce 7c00 645e 1900  |.d7k...r.|.d^..
-00005320: 7d01 641d 6116 7401 645f 6700 6446 a201  }.d.a.t.d_g.dF..
-00005330: 6447 8d02 0100 9003 6e16 7c0f 6400 6428  dG......n.|.d.d(
-00005340: 8502 1900 6437 6b02 9007 7280 7c0f 6427  ....d7k...r.|.d'
-00005350: 1700 6428 1900 640c 6b02 9007 7260 7c0f  ..d(..d.k...r`|.
-00005360: 6460 6400 8502 1900 7d0f 6461 7404 7c0f  d`d.....}.dat.|.
-00005370: 8301 9b00 6462 9d03 7d1e 7417 7c1e 8301  ....db..}.t.|...
-00005380: 0100 7405 a01e 7c0f a101 7d1f 7c1f 6408  ..t...|...}.|.d.
-00005390: 6b02 9007 7246 7401 6463 6700 6464 a201  k...rFt.dcg.dd..
-000053a0: 6465 6466 8d03 0100 7c00 6408 1900 7d01  dedf....|.d...}.
-000053b0: 6e18 7401 6467 6700 6446 a201 6447 8d02  n.t.dgg.dF..dG..
-000053c0: 0100 7c00 6444 1900 7d01 6e18 7c00 6444  ..|.dD..}.n.|.dD
-000053d0: 1900 7d01 7401 6448 6700 6446 a201 6447  ..}.t.dHg.dF..dG
-000053e0: 8d02 0100 641d 6116 9002 6e64 7c0f 6439  ....d.a...nd|.d9
-000053f0: 6b02 9007 72a2 7c00 6402 1900 7d01 641d  k...r.|.d...}.d.
-00005400: 6116 7417 7c0a 8301 0100 9002 6e42 7c0f  a.t.|.......nB|.
-00005410: 643b 6b02 9007 72cc 7c00 645e 1900 7d01  d;k...r.|.d^..}.
-00005420: 641d 6116 7401 6468 6700 6446 a201 6447  d.a.t.dhg.dF..dG
-00005430: 8d02 0100 9002 6e18 7c0f 6400 6460 8502  ......n.|.d.d`..
-00005440: 1900 643b 6b02 9008 728e 7c0f 6427 1700  ..d;k...r.|.d'..
-00005450: 6460 1900 640c 6b02 9008 726e 7c0f 6469  d`..d.k...rn|.di
-00005460: 6400 8502 1900 7d0f 7c0f 646a 6b02 9008  d.....}.|.djk...
-00005470: 7228 7c0d 6408 1900 7d0e 7c00 6408 1900  r(|.d...}.|.d...
-00005480: 7d01 7401 646b 6700 644e a201 6447 8d02  }.t.dkg.dN..dG..
-00005490: 0100 6e44 7c0f 646c 6b02 9008 7254 7c0d  ..nD|.dlk...rT|.
-000054a0: 6402 1900 7d0e 7c00 6408 1900 7d01 7401  d...}.|.d...}.t.
-000054b0: 646d 6700 644e a201 6447 8d02 0100 6e18  dmg.dN..dG....n.
-000054c0: 7c00 6444 1900 7d01 7401 646e 6700 6446  |.dD..}.t.dng.dF
-000054d0: a201 6447 8d02 0100 6e18 7c00 6444 1900  ..dG....n.|.dD..
-000054e0: 7d01 7401 6448 6700 6446 a201 6447 8d02  }.t.dHg.dF..dG..
-000054f0: 0100 641d 6116 9001 6e56 7c0f 643d 6b02  ..d.a...nV|.d=k.
-00005500: 9008 72b4 7c00 645e 1900 7d01 7401 646f  ..r.|.d^..}.t.do
-00005510: 6700 6446 a201 6447 8d02 0100 9001 6e30  g.dF..dG......n0
-00005520: 7c0f 6400 6460 8502 1900 643d 6b02 9009  |.d.d`....d=k...
-00005530: 722e 7c0f 6427 1700 6460 1900 640c 6b02  r.|.d'..d`..d.k.
-00005540: 9009 7214 7c0f 6469 6400 8502 1900 7d0f  ..r.|.did.....}.
-00005550: 7401 6470 6700 644b a201 6405 644c 8d03  t.dpg.dK..d.dL..
-00005560: 0100 7421 7c0f 8301 9009 720a 7c00 6426  ..t!|.....r.|.d&
-00005570: 1900 7d01 6e08 7c00 6444 1900 7d01 6e18  ..}.n.|.dD..}.n.
-00005580: 7c00 6444 1900 7d01 7401 6448 6700 6446  |.dD..}.t.dHg.dF
-00005590: a201 6447 8d02 0100 6eb6 7c0f 6442 6b02  ..dG....n.|.dBk.
-000055a0: 9009 7252 7c00 645e 1900 7d01 7401 6471  ..rR|.d^..}.t.dq
-000055b0: 6700 6446 a201 6447 8d02 0100 6e92 7c0f  g.dF..dG....n.|.
-000055c0: 6400 645e 8502 1900 6442 6b02 9009 72cc  d.d^....dBk...r.
-000055d0: 7c0f 6427 1700 645e 1900 640c 6b02 9009  |.d'..d^..d.k...
-000055e0: 72b2 7c0f 6444 6400 8502 1900 7d0f 7401  r.|.dDd.....}.t.
-000055f0: 6472 6700 644b a201 6405 644c 8d03 0100  drg.dK..d.dL....
-00005600: 7422 7c0f 8301 9009 72a8 7c00 6426 1900  t"|.....r.|.d&..
-00005610: 7d01 6e08 7c00 6444 1900 7d01 6e18 7c00  }.n.|.dD..}.n.|.
-00005620: 6444 1900 7d01 7401 6448 6700 6446 a201  dD..}.t.dHg.dF..
-00005630: 6447 8d02 0100 6e18 7c00 6444 1900 7d01  dG....n.|.dD..}.
-00005640: 7401 6448 6700 6446 a201 6447 8d02 0100  t.dHg.dF..dG....
-00005650: 7c0f 7d0c 9001 71f2 6400 5300 2973 4e7a  |.}...q.d.S.)sNz
-00005660: 275b 235d 2049 6e69 7469 616c 697a 696e  '[#] Initializin
-00005670: 6720 6050 4830 4d42 4552 6020 6672 616d  g `PH0MBER` fram
-00005680: 6577 6f72 6b2e 2e2e 721e 0000 0072 1f00  ework...r....r..
-00005690: 0000 2903 72a4 0000 0072 a700 0000 72a8  ..).r....r....r.
-000056a0: 0000 0054 2904 7222 0000 0072 8800 0000  ...T).r"...r....
-000056b0: 7287 0000 0072 8900 0000 2905 7a10 1b5b  r....r....).z..[
-000056c0: 313b 3439 3b39 326d 3a44 1b5b 306d 7a10  1;49;92m:D.[0mz.
-000056d0: 1b5b 313b 3439 3b39 366d 3a29 1b5b 306d  .[1;49;96m:).[0m
-000056e0: 7a10 1b5b 313b 3439 3b39 336d 3a7c 1b5b  z..[1;49;93m:|.[
-000056f0: 306d 7a10 1b5b 313b 3439 3b39 316d 3a28  0mz..[1;49;91m:(
-00005700: 1b5b 306d 7a10 1b5b 313b 3439 3b39 376d  .[0mz..[1;49;97m
-00005710: 3a6f 1b5b 306d 7201 0000 0075 f303 0000  :o.[0mr....u....
-00005720: 2020 2020 1b5b 313b 3439 3b39 336d 3e20      .[1;49;93m> 
-00005730: 4578 7072 6573 7369 6f6e 7320 6172 6520  Expressions are 
-00005740: 7573 6564 2074 6f20 7368 6f77 2074 6865  used to show the
-00005750: 2073 7461 7475 7320 6f66 2074 6865 2070   status of the p
-00005760: 7265 7669 6f75 7320 636f 6d6d 616e 641b  revious command.
-00005770: 5b30 6d0a 0a20 2020 201b 5b31 3b34 393b  [0m..    .[1;49;
-00005780: 3933 6d3e 2053 796e 7461 783a 1b5b 306d  93m> Syntax:.[0m
-00005790: 201b 5b31 3b34 393b 3937 6d5b 3c75 7365   .[1;49;97m[<use
-000057a0: 723e 4070 6830 6d62 6572 5de2 b8ba 201b  r>@ph0mber]... .
-000057b0: 5b31 3b34 393b 3936 6d5b 3c65 7870 7265  [1;49;96m[<expre
-000057c0: 7373 696f 6e3e 5d1b 5b31 3b34 393b 3937  ssion>].[1;49;97
-000057d0: 6d20 2420 3c63 6f6d 6d61 6e64 3e1b 5b30  m $ <command>.[0
-000057e0: 6d0a 0a20 2020 20e2 948c e294 80e2 9480  m..    .........
-000057f0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00005800: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00005810: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00005820: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00005830: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00005840: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00005850: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00005860: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00005870: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00005880: e294 80e2 9480 e294 900a 2020 2020 7c20  ..........    | 
-00005890: 4558 5052 4553 5349 4f4e 5320 2020 7c20  EXPRESSIONS   | 
-000058a0: 4445 5343 5249 5054 494f 4e20 2020 2020  DESCRIPTION     
-000058b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000058c0: 2020 207c 0a20 2020 207c 2d2d 2d2d 2d2d     |.    |------
-000058d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000058e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000058f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 7c0a  --------------|.
-00005900: 2020 2020 7c20 1b5b 313b 3439 3b39 326d      | .[1;49;92m
-00005910: 3a44 1b5b 306d 2020 2020 2020 2020 2020  :D.[0m          
-00005920: 2020 7c20 4576 6572 7974 6869 6e67 2069    | Everything i
-00005930: 7320 6669 6e65 2020 2020 2020 2020 2020  s fine          
-00005940: 2020 2020 2020 207c 0a20 2020 207c 201b         |.    | .
-00005950: 5b31 3b34 393b 3936 6d3a 291b 5b30 6d20  [1;49;96m:).[0m 
-00005960: 2020 2020 2020 2020 2020 207c 2049 6e66             | Inf
-00005970: 6f72 6d61 7469 6f6e 2061 7661 696c 6162  ormation availab
-00005980: 6c65 2020 2020 2020 2020 2020 2020 2020  le              
-00005990: 7c0a 2020 2020 7c20 1b5b 313b 3439 3b39  |.    | .[1;49;9
-000059a0: 336d 3a7c 1b5b 306d 2020 2020 2020 2020  3m:|.[0m        
-000059b0: 2020 2020 7c20 4974 2773 2061 2077 6172      | It's a war
-000059c0: 6e69 6e67 2028 7265 6d65 6d62 6572 2920  ning (remember) 
-000059d0: 2020 2020 2020 2020 207c 0a20 2020 207c           |.    |
-000059e0: 201b 5b31 3b34 393b 3931 6d3a 281b 5b30   .[1;49;91m:(.[0
-000059f0: 6d20 2020 2020 2020 2020 2020 207c 2053  m            | S
-00005a00: 6f6d 6574 6869 6e67 2077 656e 7420 7772  omething went wr
-00005a10: 6f6e 6720 2020 2020 2020 2020 2020 2020  ong             
-00005a20: 2020 7c0a 2020 2020 7c20 1b5b 313b 3439    |.    | .[1;49
-00005a30: 3b39 376d 3a6f 1b5b 306d 2020 2020 2020  ;97m:o.[0m      
-00005a40: 2020 2020 2020 7c20 5363 616e 2072 6573        | Scan res
-00005a50: 756c 7473 2061 7661 696c 6162 6c65 2020  ults available  
-00005a60: 2020 2020 2020 2020 2020 207c 0a20 2020             |.   
-00005a70: 20e2 9494 e294 80e2 9480 e294 80e2 9480   ...............
-00005a80: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00005a90: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00005aa0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00005ab0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00005ac0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00005ad0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00005ae0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00005af0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00005b00: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00005b10: e294 987a 0a1b 5b31 3b34 393b 3936 6d72  ...z..[1;49;96mr
-00005b20: 8000 0000 7230 0000 00e9 2200 0000 fa01  ....r0....".....
-00005b30: 25e9 2100 0000 e920 0000 0072 3400 0000  %.!.... ...r4...
-00005b40: 7a16 1b5b 313b 3439 3b39 366d 332e 3020  z..[1;49;96m3.0 
-00005b50: 6265 7461 1b5b 306d 6700 0000 0000 0008  beta.[0mg.......
-00005b60: 4075 4201 0000 0a20 2020 20e2 948c e294  @uB....    .....
-00005b70: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00005b80: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00005b90: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00005ba0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00005bb0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00005bc0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00005bd0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00005be0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00005bf0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00005c00: 80e2 9480 e294 80e2 9480 e294 900a 2020  ..............  
-00005c10: 2020 7c20 5359 5354 454d 2049 4e46 4f20    | SYSTEM INFO 
-00005c20: 2020 7c20 4445 5343 5249 5054 494f 4e20    | DESCRIPTION 
-00005c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005c40: 2020 2020 2020 207c 0a20 2020 207c 2d2d         |.    |--
-00005c50: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00005c60: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00005c70: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00005c80: 2d2d 7c0a 2020 2020 7c20 1b5b 313b 3439  --|.    | .[1;49
-00005c90: 3b39 376d 5573 6572 1b5b 306d 2020 2020  ;97mUser.[0m    
-00005ca0: 2020 2020 2020 7c20 7a27 207c 0a20 2020        | z' |.   
-00005cb0: 207c 201b 5b31 3b34 393b 3937 6d48 6f73   | .[1;49;97mHos
-00005cc0: 746e 616d 651b 5b30 6d20 2020 2020 207c  tname.[0m      |
-00005cd0: 207a 2720 7c0a 2020 2020 7c20 1b5b 313b   z' |.    | .[1;
-00005ce0: 3439 3b39 376d 4f53 1b5b 306d 2020 2020  49;97mOS.[0m    
-00005cf0: 2020 2020 2020 2020 7c20 7a27 207c 0a20          | z' |. 
-00005d00: 2020 207c 201b 5b31 3b34 393b 3937 6d52     | .[1;49;97mR
-00005d10: 414d 2055 7361 6765 1b5b 306d 2020 2020  AM Usage.[0m    
-00005d20: 207c 207a 2720 7c0a 2020 2020 7c20 1b5b   | z' |.    | .[
-00005d30: 313b 3439 3b39 376d 4350 5520 5573 6167  1;49;97mCPU Usag
-00005d40: 651b 5b30 6d20 2020 2020 7c20 7a27 207c  e.[0m     | z' |
-00005d50: 0a20 2020 207c 201b 5b31 3b34 393b 3937  .    | .[1;49;97
-00005d60: 6d44 6973 6b20 5573 6167 651b 5b30 6d20  mDisk Usage.[0m 
-00005d70: 2020 207c 2075 4302 0000 207c 0a20 2020     | uC... |.   
-00005d80: 20e2 9494 e294 80e2 9480 e294 80e2 9480   ...............
-00005d90: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00005da0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00005db0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00005dc0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00005dd0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00005de0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00005df0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00005e00: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00005e10: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00005e20: e294 980a 0a20 2020 20e2 948c e294 80e2  .....    .......
-00005e30: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00005e40: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00005e50: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00005e60: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00005e70: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00005e80: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00005e90: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00005ea0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00005eb0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00005ec0: 9480 e294 80e2 9480 e294 900a 2020 2020  ............    
-00005ed0: 7c20 4652 414d 4557 4f52 4b20 494e 464f  | FRAMEWORK INFO
-00005ee0: 7c20 4445 5343 5249 5054 494f 4e20 2020  | DESCRIPTION   
-00005ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005f00: 2020 2020 207c 0a20 2020 207c 2d2d 2d2d       |.    |----
-00005f10: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00005f20: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00005f30: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00005f40: 7c0a 2020 2020 7c20 1b5b 313b 3439 3b39  |.    | .[1;49;9
-00005f50: 376d 4e61 6d65 1b5b 306d 2020 2020 2020  7mName.[0m      
-00005f60: 2020 2020 7c20 1b5b 313b 3439 3b39 366d      | .[1;49;96m
-00005f70: 5048 304d 4245 521b 5b30 6d20 2020 2020  PH0MBER.[0m     
-00005f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005f90: 2020 2020 2020 207c 0a20 2020 207c 201b         |.    | .
-00005fa0: 5b31 3b34 393b 3937 6d56 6572 7369 6f6e  [1;49;97mVersion
-00005fb0: 1b5b 306d 2020 2020 2020 207c 2075 b301  .[0m       | u..
-00005fc0: 0000 207c 0a20 2020 207c 201b 5b31 3b34  .. |.    | .[1;4
-00005fd0: 393b 3937 6d54 7970 651b 5b30 6d20 2020  9;97mType.[0m   
-00005fe0: 2020 2020 2020 207c 201b 5b31 3b34 393b         | .[1;49;
-00005ff0: 3936 6d4f 5349 4e54 1b5b 306d 2020 2020  96mOSINT.[0m    
-00006000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006010: 2020 2020 2020 2020 2020 7c0a 2020 2020            |.    
-00006020: 7c20 1b5b 313b 3439 3b39 376d 4175 7468  | .[1;49;97mAuth
-00006030: 6f72 1b5b 306d 2020 2020 2020 2020 7c20  or.[0m        | 
-00006040: 1b5b 313b 3439 3b39 366d 7334 3172 346a  .[1;49;96ms41r4j
-00006050: 1b5b 306d 2020 2020 2020 2020 2020 2020  .[0m            
-00006060: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006070: 207c 0a20 2020 207c 201b 5b31 3b34 393b   |.    | .[1;49;
-00006080: 3937 6d47 6974 6875 621b 5b30 6d20 2020  97mGithub.[0m   
-00006090: 2020 2020 207c 201b 5b31 3b34 393b 3936       | .[1;49;96
-000060a0: 6d68 7474 7073 3a2f 2f67 6974 6875 622e  mhttps://github.
-000060b0: 636f 6d2f 7334 3172 346a 2f70 686f 6d62  com/s41r4j/phomb
-000060c0: 6572 1b5b 306d 2020 7c0a 2020 2020 e294  er.[0m  |.    ..
-000060d0: 94e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-000060e0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-000060f0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00006100: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00006110: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00006120: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00006130: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00006140: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00006150: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00006160: 80e2 9480 e294 80e2 9480 e294 80e2 9498  ................
-00006170: 0a20 2020 2075 ea07 0000 0a20 2020 20e2  .    u.....    .
-00006180: 948c e294 80e2 9480 e294 80e2 9480 e294  ................
-00006190: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-000061a0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-000061b0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-000061c0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-000061d0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-000061e0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-000061f0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00006200: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00006210: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00006220: 900a 2020 2020 7c20 434f 4d4d 414e 4453  ..    | COMMANDS
-00006230: 2020 2020 2020 7c20 4445 5343 5249 5054        | DESCRIPT
-00006240: 494f 4e20 2020 2020 2020 2020 2020 2020  ION             
-00006250: 2020 2020 2020 2020 2020 207c 0a20 2020             |.   
-00006260: 207c 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   |--------------
-00006270: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00006280: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00006290: 2d2d 2d2d 2d2d 7c0a 2020 2020 7c20 2020  ------|.    |   
-000062a0: 2020 2020 2020 2020 2020 2020 203c 4261               <Ba
-000062b0: 7369 6320 436f 6d6d 616e 6473 3e20 2020  sic Commands>   
-000062c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000062d0: 207c 0a20 2020 207c 2d2d 2d2d 2d2d 2d2d   |.    |--------
-000062e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000062f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00006300: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 7c0a 2020  ------------|.  
-00006310: 2020 7c20 1b5b 313b 3439 3b39 376d 6865    | .[1;49;97mhe
-00006320: 6c70 1b5b 306d 2020 2020 2020 2020 2020  lp.[0m          
-00006330: 7c20 4469 7370 6c61 7920 7468 6973 2068  | Display this h
-00006340: 656c 7020 6d65 6e75 2020 2020 2020 2020  elp menu        
-00006350: 2020 2020 207c 200a 2020 2020 7c20 1b5b       | .    | .[
-00006360: 313b 3439 3b39 376d 6578 6974 2f71 7569  1;49;97mexit/qui
-00006370: 741b 5b30 6d20 2020 2020 7c20 4578 6974  t.[0m     | Exit
-00006380: 2074 6865 2066 7261 6d65 776f 726b 2020   the framework  
-00006390: 2020 2020 2020 2020 2020 2020 2020 207c                 |
-000063a0: 0a20 2020 207c 201b 5b31 3b34 393b 3937  .    | .[1;49;97
-000063b0: 6d64 6f72 6b1b 5b30 6d20 2020 2020 2020  mdork.[0m       
-000063c0: 2020 207c 2053 686f 7720 6120 7261 6e64     | Show a rand
-000063d0: 6f6d 2067 6f6f 676c 6520 646f 726b 2071  om google dork q
-000063e0: 7565 7279 2020 2020 7c20 200a 2020 2020  uery    |  .    
-000063f0: 7c20 1b5b 313b 3439 3b39 376d 6578 701b  | .[1;49;97mexp.
-00006400: 5b30 6d20 2020 2020 2020 2020 2020 7c20  [0m           | 
-00006410: 5368 6f77 2069 6e66 6f20 6162 6f75 7420  Show info about 
-00006420: 616c 6c20 6176 6169 6c61 626c 6520 2020  all available   
-00006430: 2020 207c 2020 2020 2020 200a 2020 2020     |       .    
-00006440: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
-00006450: 7c20 6578 7072 6573 7369 6f6e 7320 2020  | expressions   
-00006460: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006470: 2020 2020 207c 0a20 2020 207c 201b 5b31       |.    | .[1
-00006480: 3b34 393b 3937 6d63 6865 636b 1b5b 306d  ;49;97mcheck.[0m
-00006490: 2020 2020 2020 2020 207c 2043 6865 636b           | Check
-000064a0: 2069 6e74 6572 6e65 7420 636f 6e6e 6563   internet connec
-000064b0: 7469 6f6e 2020 2020 2020 2020 2020 7c0a  tion          |.
-000064c0: 2020 2020 7c20 1b5b 313b 3439 3b39 376d      | .[1;49;97m
-000064d0: 636c 6561 721b 5b30 6d20 2020 2020 2020  clear.[0m       
-000064e0: 2020 7c20 436c 6561 7220 7363 7265 656e    | Clear screen
-000064f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006500: 2020 2020 2020 207c 0a20 2020 207c 201b         |.    | .
-00006510: 5b31 3b34 393b 3937 6d73 6176 651b 5b30  [1;49;97msave.[0
-00006520: 6d20 2020 2020 2020 2020 207c 2053 6176  m          | Sav
-00006530: 6520 6f75 7470 7574 206f 6620 7072 6576  e output of prev
-00006540: 696f 7573 2073 6361 6e6e 6572 2020 2020  ious scanner    
-00006550: 7c0a 2020 2020 7c20 2020 2020 2020 2020  |.    |         
-00006560: 2020 2020 2020 7c20 636f 6d6d 616e 6420        | command 
-00006570: 696e 2061 2066 696c 6520 2020 2020 2020  in a file       
-00006580: 2020 2020 2020 2020 2020 207c 0a20 2020             |.   
-00006590: 207c 201b 5b31 3b34 393b 3937 6d73 6865   | .[1;49;97mshe
-000065a0: 6c6c 203c 636d 643e 1b5b 306d 2020 207c  ll <cmd>.[0m   |
-000065b0: 2045 7865 6375 7465 206e 6174 6976 6520   Execute native 
-000065c0: 7368 656c 6c2f 636d 6420 636f 6d6d 616e  shell/cmd comman
-000065d0: 6473 2020 7c0a 2020 2020 7c20 1b5b 313b  ds  |.    | .[1;
-000065e0: 3439 3b39 376d 696e 666f 1b5b 306d 2020  49;97minfo.[0m  
-000065f0: 2020 2020 2020 2020 7c20 5368 6f77 2069          | Show i
-00006600: 6e66 6f20 6162 6f75 7420 6672 616d 6577  nfo about framew
-00006610: 6f72 6b20 2620 7379 7374 656d 207c 0a20  ork & system |. 
-00006620: 2020 207c 201b 5b31 3b34 393b 3937 6d63     | .[1;49;97mc
-00006630: 6861 6e67 651b 5b30 6d20 2020 2020 2020  hange.[0m       
-00006640: 207c 2043 6861 6e67 6520 7573 6572 2063   | Change user c
-00006650: 6f6d 6d61 6e64 2069 6e70 7574 2063 6f6c  ommand input col
-00006660: 6f72 2020 2020 7c0a 2020 2020 7c2d 2d2d  or    |.    |---
-00006670: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00006680: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00006690: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000066a0: 2d7c 0a20 2020 207c 2020 2020 2020 2020  -|.    |        
-000066b0: 2020 2020 2020 2020 203c 5363 616e 6e65           <Scanne
-000066c0: 7220 436f 6d6d 616e 6473 3e20 2020 2020  r Commands>     
-000066d0: 2020 2020 2020 2020 2020 2020 7c0a 2020              |.  
-000066e0: 2020 7c2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d    |-------------
-000066f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00006700: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00006710: 2d2d 2d2d 2d2d 2d7c 0a20 2020 207c 201b  -------|.    | .
-00006720: 5b31 3b34 393b 3937 6d6e 756d 6265 721b  [1;49;97mnumber.
-00006730: 5b30 6d20 2020 2020 2020 207c 2052 6576  [0m        | Rev
-00006740: 6572 7365 2070 686f 6e65 206e 756d 6265  erse phone numbe
-00006750: 7220 6c6f 6f6b 7570 2020 2020 2020 2020  r lookup        
-00006760: 7c0a 2020 2020 7c20 1b5b 313b 3439 3b39  |.    | .[1;49;9
-00006770: 376d 6970 1b5b 306d 2020 2020 2020 2020  7mip.[0m        
-00006780: 2020 2020 7c20 5265 7665 7273 6520 6970      | Reverse ip
-00006790: 2061 6464 7265 7373 206c 6f6f 6b75 7020   address lookup 
-000067a0: 2020 2020 2020 2020 207c 0a20 2020 207c           |.    |
-000067b0: 201b 5b31 3b34 393b 3931 6d4d 4f52 4520   .[1;49;91mMORE 
-000067c0: 5343 414e 4e45 5253 2043 4f4d 494e 4720  SCANNERS COMING 
-000067d0: 534f 4f4e 2c20 5448 4953 2049 5320 4120  SOON, THIS IS A 
-000067e0: 4245 5441 2056 4552 1b5b 306d 2020 2020  BETA VER.[0m    
-000067f0: 2020 7c0a 2020 2020 e294 94e2 9480 e294    |.    ........
-00006800: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00006810: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00006820: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00006830: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00006840: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00006850: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00006860: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00006870: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00006880: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00006890: 80e2 9480 e294 80e2 9498 0a0a 2020 2020  ............    
-000068a0: 1b5b 313b 3439 3b39 336d 3e20 5479 7065  .[1;49;93m> Type
-000068b0: 2060 6865 6c70 203c 636f 6d6d 616e 643e   `help <command>
-000068c0: 6020 746f 2073 6565 206d 6f72 6520 696e  ` to see more in
-000068d0: 666f 2061 626f 7574 2061 2063 6f6d 6d61  fo about a comma
-000068e0: 6e64 1b5b 306d 0a20 2020 201b 5b31 3b34  nd.[0m.    .[1;4
-000068f0: 393b 3933 6d3e 2055 7365 2060 5461 6260  9;93m> Use `Tab`
-00006900: 206b 6579 2074 6f20 6175 746f 2d63 6f6d   key to auto-com
-00006910: 706c 6574 6520 636f 6d6d 616e 6473 1b5b  plete commands.[
-00006920: 306d 0a20 2020 201b 5b31 3b34 393b 3933  0m.    .[1;49;93
-00006930: 6d3e 2054 7279 2073 696c 656e 7420 6d6f  m> Try silent mo
-00006940: 6465 2062 7920 7573 696e 6720 602d 7360  de by using `-s`
-00006950: 2f60 2d2d 7369 6c65 6e74 6020 666c 6167  /`--silent` flag
-00006960: 1b5b 306d 720f 0000 007a 0d74 6162 3a20  .[0mr....z.tab: 
-00006970: 636f 6d70 6c65 7465 7a0a 1b5b 313b 3439  completez..[1;49
-00006980: 3b39 306d 7a0a 1b5b 313b 3439 3b39 376d  ;90mz..[1;49;97m
-00006990: 7a02 0a5b 750e 0000 0040 7068 306d 6265  z..[u....@ph0mbe
-000069a0: 725d e2b8 ba20 5b7a 045d 2024 2029 0272  r]... [z.] $ ).r
-000069b0: 8b00 0000 7289 0000 0072 0200 0000 e904  ....r....r......
-000069c0: 0000 00fa 0123 e905 0000 0061 2b01 0000  .....#.....a+...
-000069d0: 2020 1b5b 313b 3439 3b39 336d 5b2b 5d20    .[1;49;93m[+] 
-000069e0: 436f 6d6d 616e 6420 496e 666f 3a20 1b5b  Command Info: .[
-000069f0: 313b 3439 3b39 336d 6865 6c70 0a0a 2020  1;49;93mhelp..  
-00006a00: 2020 1b5b 313b 3439 3b39 326d 3e20 4445    .[1;49;92m> DE
-00006a10: 5343 5249 5054 494f 4e3a 201b 5b31 3b34  SCRIPTION: .[1;4
-00006a20: 393b 3937 6d57 6865 6e20 796f 7520 7479  9;97mWhen you ty
-00006a30: 7065 2060 6865 6c70 602c 2074 6865 2068  pe `help`, the h
-00006a40: 656c 7020 6d65 6e75 2077 696c 6c20 6265  elp menu will be
-00006a50: 2064 6973 706c 6179 6564 0a20 2020 201b   displayed.    .
-00006a60: 5b31 3b34 393b 3932 6d3e 2053 594e 5441  [1;49;92m> SYNTA
-00006a70: 583a 201b 5b31 3b34 393b 3937 6d68 656c  X: .[1;49;97mhel
-00006a80: 7020 1b5b 313b 3439 3b39 326d 4f52 201b  p .[1;49;92mOR .
-00006a90: 5b31 3b34 393b 3937 6d68 656c 7020 3c63  [1;49;97mhelp <c
-00006aa0: 6f6d 6d61 6e64 3e0a 2020 2020 1b5b 313b  ommand>.    .[1;
-00006ab0: 3439 3b39 326d 3e20 4558 414d 504c 453a  49;92m> EXAMPLE:
-00006ac0: 201b 5b31 3b34 393b 3937 6d68 656c 7020   .[1;49;97mhelp 
-00006ad0: 1b5b 313b 3439 3b39 326d 4f52 201b 5b31  .[1;49;92mOR .[1
-00006ae0: 3b34 393b 3937 6d68 656c 7020 6e75 6d62  ;49;97mhelp numb
-00006af0: 6572 0a20 2020 201b 5b30 6d72 0300 0000  er.    .[0mr....
-00006b00: 7204 0000 007a ee20 201b 5b31 3b34 393b  r....z.  .[1;49;
-00006b10: 3933 6d5b 2b5d 2043 6f6d 6d61 6e64 2049  93m[+] Command I
-00006b20: 6e66 6f3a 201b 5b31 3b34 393b 3933 6d65  nfo: .[1;49;93me
-00006b30: 7869 742f 1b5b 313b 3439 3b39 336d 7175  xit/.[1;49;93mqu
-00006b40: 6974 0a0a 2020 2020 1b5b 313b 3439 3b39  it..    .[1;49;9
-00006b50: 326d 3e20 4445 5343 5249 5054 494f 4e3a  2m> DESCRIPTION:
-00006b60: 201b 5b31 3b34 393b 3937 6d57 6865 6e20   .[1;49;97mWhen 
-00006b70: 796f 7520 7479 7065 2060 6578 6974 6020  you type `exit` 
-00006b80: 6f72 2060 7175 6974 602c 2074 6865 2070  or `quit`, the p
-00006b90: 726f 6772 616d 2077 696c 6c20 6265 2074  rogram will be t
-00006ba0: 6572 6d69 6e61 7465 640a 2020 2020 1b5b  erminated.    .[
-00006bb0: 313b 3439 3b39 326d 3e20 5359 4e54 4158  1;49;92m> SYNTAX
-00006bc0: 3a20 1b5b 313b 3439 3b39 376d 6578 6974  : .[1;49;97mexit
-00006bd0: 201b 5b31 3b34 393b 3932 6d4f 5220 1b5b   .[1;49;92mOR .[
-00006be0: 313b 3439 3b39 376d 7175 6974 0a20 2020  1;49;97mquit.   
-00006bf0: 201b 5b30 6d72 0500 0000 7ac7 2020 1b5b   .[0mr....z.  .[
-00006c00: 313b 3439 3b39 336d 5b2b 5d20 436f 6d6d  1;49;93m[+] Comm
-00006c10: 616e 6420 496e 666f 3a20 1b5b 313b 3439  and Info: .[1;49
-00006c20: 3b39 336d 646f 726b 0a0a 2020 2020 1b5b  ;93mdork..    .[
-00006c30: 313b 3439 3b39 326d 3e20 4445 5343 5249  1;49;92m> DESCRI
-00006c40: 5054 494f 4e3a 201b 5b31 3b34 393b 3937  PTION: .[1;49;97
-00006c50: 6d57 6865 6e20 796f 7520 7479 7065 2060  mWhen you type `
-00006c60: 646f 726b 602c 2061 2072 616e 646f 6d20  dork`, a random 
-00006c70: 676f 6f67 6c65 2064 6f72 6b20 7175 6572  google dork quer
-00006c80: 7920 7769 6c6c 2062 6520 6469 7370 6c61  y will be displa
-00006c90: 7965 640a 2020 2020 1b5b 313b 3439 3b39  yed.    .[1;49;9
-00006ca0: 326d 3e20 5359 4e54 4158 3a20 1b5b 313b  2m> SYNTAX: .[1;
-00006cb0: 3439 3b39 376d 646f 726b 0a20 2020 201b  49;97mdork.    .
-00006cc0: 5b30 6d72 0600 0000 7ace 2020 1b5b 313b  [0mr....z.  .[1;
-00006cd0: 3439 3b39 336d 5b2b 5d20 436f 6d6d 616e  49;93m[+] Comman
-00006ce0: 6420 496e 666f 3a20 1b5b 313b 3439 3b39  d Info: .[1;49;9
-00006cf0: 336d 6578 700a 0a20 2020 201b 5b31 3b34  3mexp..    .[1;4
-00006d00: 393b 3932 6d3e 2044 4553 4352 4950 5449  9;92m> DESCRIPTI
-00006d10: 4f4e 3a20 1b5b 313b 3439 3b39 376d 5768  ON: .[1;49;97mWh
-00006d20: 656e 2079 6f75 2074 7970 6520 6065 7870  en you type `exp
-00006d30: 602c 2069 6e66 6f20 6162 6f75 7420 616c  `, info about al
-00006d40: 6c20 6176 6169 6c61 626c 6520 6578 7072  l available expr
-00006d50: 6573 7369 6f6e 7320 7769 6c6c 2062 6520  essions will be 
-00006d60: 6469 7370 6c61 7965 640a 2020 2020 1b5b  displayed.    .[
-00006d70: 313b 3439 3b39 326d 3e20 5359 4e54 4158  1;49;92m> SYNTAX
-00006d80: 3a20 1b5b 313b 3439 3b39 376d 6578 700a  : .[1;49;97mexp.
-00006d90: 2020 2020 1b5b 306d 7207 0000 007a d020      .[0mr....z. 
-00006da0: 201b 5b31 3b34 393b 3933 6d5b 2b5d 2043   .[1;49;93m[+] C
-00006db0: 6f6d 6d61 6e64 2049 6e66 6f3a 201b 5b31  ommand Info: .[1
-00006dc0: 3b34 393b 3933 6d63 6865 636b 0a0a 2020  ;49;93mcheck..  
-00006dd0: 2020 1b5b 313b 3439 3b39 326d 3e20 4445    .[1;49;92m> DE
-00006de0: 5343 5249 5054 494f 4e3a 201b 5b31 3b34  SCRIPTION: .[1;4
-00006df0: 393b 3937 6d57 6865 6e20 796f 7520 7479  9;97mWhen you ty
-00006e00: 7065 2060 6368 6563 6b60 2c20 6974 2077  pe `check`, it w
-00006e10: 696c 6c20 6368 6563 6b20 666f 7220 696e  ill check for in
-00006e20: 7465 726e 6574 2063 6f6e 6e65 6374 696f  ternet connectio
-00006e30: 6e20 6176 6169 6c61 6269 6c69 7479 0a20  n availability. 
-00006e40: 2020 201b 5b31 3b34 393b 3932 6d3e 2053     .[1;49;92m> S
-00006e50: 594e 5441 583a 201b 5b31 3b34 393b 3937  YNTAX: .[1;49;97
-00006e60: 6d63 6865 636b 0a20 2020 201b 5b30 6d72  mcheck.    .[0mr
-00006e70: 0800 0000 7ab6 2020 1b5b 313b 3439 3b39  ....z.  .[1;49;9
-00006e80: 336d 5b2b 5d20 436f 6d6d 616e 6420 496e  3m[+] Command In
-00006e90: 666f 3a20 1b5b 313b 3439 3b39 336d 636c  fo: .[1;49;93mcl
-00006ea0: 6561 720a 0a20 2020 201b 5b31 3b34 393b  ear..    .[1;49;
-00006eb0: 3932 6d3e 2044 4553 4352 4950 5449 4f4e  92m> DESCRIPTION
-00006ec0: 3a20 1b5b 313b 3439 3b39 376d 5768 656e  : .[1;49;97mWhen
-00006ed0: 2079 6f75 2074 7970 6520 6063 6c65 6172   you type `clear
-00006ee0: 602c 2069 7420 7769 6c6c 2063 6c65 6172  `, it will clear
-00006ef0: 2074 6865 2073 6372 6565 6e0a 2020 2020   the screen.    
-00006f00: 1b5b 313b 3439 3b39 326d 3e20 5359 4e54  .[1;49;92m> SYNT
-00006f10: 4158 3a20 1b5b 313b 3439 3b39 376d 636c  AX: .[1;49;97mcl
-00006f20: 6561 720a 2020 2020 1b5b 306d 7209 0000  ear.    .[0mr...
-00006f30: 007a ee20 201b 5b31 3b34 393b 3933 6d5b  .z.  .[1;49;93m[
-00006f40: 2b5d 2043 6f6d 6d61 6e64 2049 6e66 6f3a  +] Command Info:
-00006f50: 201b 5b31 3b34 393b 3933 6d73 6176 650a   .[1;49;93msave.
-00006f60: 0a20 2020 201b 5b31 3b34 393b 3932 6d3e  .    .[1;49;92m>
-00006f70: 2044 4553 4352 4950 5449 4f4e 3a20 1b5b   DESCRIPTION: .[
-00006f80: 313b 3439 3b39 376d 5768 656e 2079 6f75  1;49;97mWhen you
-00006f90: 2074 7970 6520 6073 6176 6560 2c20 6974   type `save`, it
-00006fa0: 2077 696c 6c20 7361 7665 2074 6865 206f   will save the o
-00006fb0: 7574 7075 7420 6f66 2070 7265 7669 6f75  utput of previou
-00006fc0: 7320 636f 6d6d 616e 640a 2020 2020 1b5b  s command.    .[
-00006fd0: 313b 3439 3b39 326d 3e20 5359 4e54 4158  1;49;92m> SYNTAX
-00006fe0: 3a20 1b5b 313b 3439 3b39 376d 7361 7665  : .[1;49;97msave
-00006ff0: 0a20 2020 201b 5b31 3b34 393b 3932 6d3e  .    .[1;49;92m>
-00007000: 2045 5841 4d50 4c45 3a20 1b5b 313b 3439   EXAMPLE: .[1;49
-00007010: 3b39 376d 7361 7665 0a20 2020 201b 5b30  ;97msave.    .[0
-00007020: 6d72 0a00 0000 6101 0100 0020 201b 5b31  mr....a....  .[1
-00007030: 3b34 393b 3933 6d5b 2b5d 2043 6f6d 6d61  ;49;93m[+] Comma
-00007040: 6e64 2049 6e66 6f3a 201b 5b31 3b34 393b  nd Info: .[1;49;
-00007050: 3933 6d73 6865 6c6c 0a0a 2020 2020 1b5b  93mshell..    .[
-00007060: 313b 3439 3b39 326d 3e20 4445 5343 5249  1;49;92m> DESCRI
-00007070: 5054 494f 4e3a 201b 5b31 3b34 393b 3937  PTION: .[1;49;97
-00007080: 6d57 6865 6e20 796f 7520 7479 7065 2060  mWhen you type `
-00007090: 7368 656c 6c60 2c20 6974 2077 696c 6c20  shell`, it will 
-000070a0: 6578 6563 7574 6520 6769 7665 6e20 636f  execute given co
-000070b0: 6d6d 616e 6420 696e 206e 6174 6976 6520  mmand in native 
-000070c0: 7368 656c 6c2f 636d 640a 2020 2020 1b5b  shell/cmd.    .[
-000070d0: 313b 3439 3b39 326d 3e20 5359 4e54 4158  1;49;92m> SYNTAX
-000070e0: 3a20 1b5b 313b 3439 3b39 376d 7368 656c  : .[1;49;97mshel
-000070f0: 6c20 3c63 6d64 3e0a 2020 2020 1b5b 313b  l <cmd>.    .[1;
-00007100: 3439 3b39 326d 3e20 4558 414d 504c 453a  49;92m> EXAMPLE:
-00007110: 201b 5b31 3b34 393b 3937 6d73 6865 6c6c   .[1;49;97mshell
-00007120: 206c 730a 2020 2020 1b5b 306d 720b 0000   ls.    .[0mr...
-00007130: 007a c520 201b 5b31 3b34 393b 3933 6d5b  .z.  .[1;49;93m[
-00007140: 2b5d 2043 6f6d 6d61 6e64 2049 6e66 6f3a  +] Command Info:
-00007150: 201b 5b31 3b34 393b 3933 6d69 6e66 6f0a   .[1;49;93minfo.
-00007160: 0a20 2020 201b 5b31 3b34 393b 3932 6d3e  .    .[1;49;92m>
-00007170: 2044 4553 4352 4950 5449 4f4e 3a20 1b5b   DESCRIPTION: .[
-00007180: 313b 3439 3b39 376d 5768 656e 2079 6f75  1;49;97mWhen you
-00007190: 2074 7970 6520 6069 6e66 6f60 2c20 6974   type `info`, it
-000071a0: 2077 696c 6c20 7368 6f77 2069 6e66 6f20   will show info 
-000071b0: 6162 6f75 7420 6672 616d 6577 6f72 6b20  about framework 
-000071c0: 2620 7379 7374 656d 0a20 2020 201b 5b31  & system.    .[1
-000071d0: 3b34 393b 3932 6d3e 2053 594e 5441 583a  ;49;92m> SYNTAX:
-000071e0: 201b 5b31 3b34 393b 3937 6d69 6e66 6f0a   .[1;49;97minfo.
-000071f0: 2020 2020 1b5b 306d 720c 0000 0061 8a01      .[0mr....a..
-00007200: 0000 2020 1b5b 313b 3439 3b39 336d 5b2b  ..  .[1;49;93m[+
-00007210: 5d20 436f 6d6d 616e 6420 496e 666f 3a20  ] Command Info: 
-00007220: 1b5b 313b 3439 3b39 336d 6368 616e 6765  .[1;49;93mchange
-00007230: 0a0a 2020 2020 1b5b 313b 3439 3b39 326d  ..    .[1;49;92m
-00007240: 3e20 4445 5343 5249 5054 494f 4e3a 201b  > DESCRIPTION: .
-00007250: 5b31 3b34 393b 3937 6d57 6865 6e20 796f  [1;49;97mWhen yo
-00007260: 7520 7479 7065 2060 6368 616e 6765 602c  u type `change`,
-00007270: 2069 7420 7769 6c6c 2063 6861 6e67 6520   it will change 
-00007280: 7573 6572 2063 6f6d 6d61 6e64 2069 6e70  user command inp
-00007290: 7574 2063 6f6c 6f72 0a20 2020 201b 5b31  ut color.    .[1
-000072a0: 3b34 393b 3932 6d3e 204f 5054 494f 4e53  ;49;92m> OPTIONS
-000072b0: 3a20 1b5b 313b 3439 3b39 376d 3020 2d3e  : .[1;49;97m0 ->
-000072c0: 201b 5b31 3b34 393b 3930 6d42 6c61 636b   .[1;49;90mBlack
-000072d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000072e0: 1b5b 313b 3439 3b39 376d 3120 2d3e 2057  .[1;49;97m1 -> W
-000072f0: 6869 7465 2020 2020 2020 2020 0a20 2020  hite        .   
-00007300: 201b 5b31 3b34 393b 3932 6d3e 2044 6566   .[1;49;92m> Def
-00007310: 6175 6c74 3a20 1b5b 313b 3439 3b39 376d  ault: .[1;49;97m
-00007320: 310a 2020 2020 1b5b 313b 3439 3b39 326d  1.    .[1;49;92m
-00007330: 3e20 5359 4e54 4158 3a20 1b5b 313b 3439  > SYNTAX: .[1;49
-00007340: 3b39 376d 6368 616e 6765 203c 636f 6c6f  ;97mchange <colo
-00007350: 725f 636f 6465 3e0a 2020 2020 1b5b 313b  r_code>.    .[1;
-00007360: 3439 3b39 326d 3e20 4558 414d 504c 453a  49;92m> EXAMPLE:
-00007370: 201b 5b31 3b34 393b 3937 6d63 6861 6e67   .[1;49;97mchang
-00007380: 6520 300a 2020 2020 1b5b 306d 720d 0000  e 0.    .[0mr...
-00007390: 0061 1101 0000 2020 1b5b 313b 3439 3b39  .a....  .[1;49;9
-000073a0: 336d 5b2b 5d20 436f 6d6d 616e 6420 496e  3m[+] Command In
-000073b0: 666f 3a20 1b5b 313b 3439 3b39 336d 6e75  fo: .[1;49;93mnu
-000073c0: 6d62 6572 0a0a 2020 2020 1b5b 313b 3439  mber..    .[1;49
-000073d0: 3b39 326d 3e20 4445 5343 5249 5054 494f  ;92m> DESCRIPTIO
-000073e0: 4e3a 201b 5b31 3b34 393b 3937 6d57 6865  N: .[1;49;97mWhe
-000073f0: 6e20 796f 7520 7479 7065 2060 6e75 6d62  n you type `numb
-00007400: 6572 602c 2069 7420 7769 6c6c 2070 6572  er`, it will per
-00007410: 666f 726d 2072 6576 6572 7365 2070 686f  form reverse pho
-00007420: 6e65 206e 756d 6265 7220 6c6f 6f6b 7570  ne number lookup
-00007430: 0a20 2020 201b 5b31 3b34 393b 3932 6d3e  .    .[1;49;92m>
-00007440: 2053 594e 5441 583a 201b 5b31 3b34 393b   SYNTAX: .[1;49;
-00007450: 3937 6d6e 756d 6265 7220 3c70 686f 6e65  97mnumber <phone
-00007460: 5f6e 756d 6265 723e 0a20 2020 201b 5b31  _number>.    .[1
-00007470: 3b34 393b 3932 6d3e 2045 5841 4d50 4c45  ;49;92m> EXAMPLE
-00007480: 3a20 1b5b 313b 3439 3b39 376d 6e75 6d62  : .[1;49;97mnumb
-00007490: 6572 202b 3132 3334 3536 3738 3930 0a20  er +1234567890. 
-000074a0: 2020 201b 5b30 6dda 0565 6d61 696c 7af3     .[0m..emailz.
-000074b0: 2020 1b5b 313b 3439 3b39 336d 5b2b 5d20    .[1;49;93m[+] 
-000074c0: 436f 6d6d 616e 6420 496e 666f 3a20 1b5b  Command Info: .[
-000074d0: 313b 3439 3b39 336d 656d 6169 6c0a 0a20  1;49;93memail.. 
-000074e0: 2020 201b 5b31 3b34 393b 3932 6d3e 2044     .[1;49;92m> D
-000074f0: 4553 4352 4950 5449 4f4e 3a20 1b5b 313b  ESCRIPTION: .[1;
-00007500: 3439 3b39 376d 5768 656e 2079 6f75 2074  49;97mWhen you t
-00007510: 7970 6520 6065 6d61 696c 602c 2069 7420  ype `email`, it 
-00007520: 7769 6c6c 2070 6572 666f 726d 2072 6576  will perform rev
-00007530: 6572 7365 2065 6d61 696c 206c 6f6f 6b75  erse email looku
-00007540: 700a 2020 2020 1b5b 313b 3439 3b39 326d  p.    .[1;49;92m
-00007550: 3e20 5359 4e54 4158 3a20 1b5b 313b 3439  > SYNTAX: .[1;49
-00007560: 3b39 376d 656d 6169 6c20 3c65 6d61 696c  ;97memail <email
-00007570: 5f61 6464 7265 7373 3e0a 2020 2020 1b5b  _address>.    .[
-00007580: 313b 3439 3b39 326d 3e20 4558 414d 504c  1;49;92m> EXAMPL
-00007590: 453a 201b 5b31 3b34 393b 3937 6d65 6d61  E: .[1;49;97mema
-000075a0: 696c 207a 1d1b 5b31 3b34 393b 3936 6d40  il z..[1;49;96m@
-000075b0: 676d 6169 6c2e 636f 6d0a 2020 2020 1b5b  gmail.com.    .[
-000075c0: 306d 720e 0000 007a f920 201b 5b31 3b34  0mr....z.  .[1;4
-000075d0: 393b 3933 6d5b 2b5d 2043 6f6d 6d61 6e64  9;93m[+] Command
-000075e0: 2049 6e66 6f3a 201b 5b31 3b34 393b 3933   Info: .[1;49;93
-000075f0: 6d69 700a 0a20 2020 201b 5b31 3b34 393b  mip..    .[1;49;
-00007600: 3932 6d3e 2044 4553 4352 4950 5449 4f4e  92m> DESCRIPTION
-00007610: 3a20 1b5b 313b 3439 3b39 376d 5768 656e  : .[1;49;97mWhen
-00007620: 2079 6f75 2074 7970 6520 6069 7060 2c20   you type `ip`, 
-00007630: 6974 2077 696c 6c20 7065 7266 6f72 6d20  it will perform 
-00007640: 7265 7665 7273 6520 6970 2061 6464 7265  reverse ip addre
-00007650: 7373 206c 6f6f 6b75 700a 2020 2020 1b5b  ss lookup.    .[
-00007660: 313b 3439 3b39 326d 3e20 5359 4e54 4158  1;49;92m> SYNTAX
-00007670: 3a20 1b5b 313b 3439 3b39 376d 6970 203c  : .[1;49;97mip <
-00007680: 6970 5f61 6464 7265 7373 3e0a 2020 2020  ip_address>.    
-00007690: 1b5b 313b 3439 3b39 326d 3e20 4558 414d  .[1;49;92m> EXAM
-000076a0: 504c 453a 201b 5b31 3b34 393b 3937 6d69  PLE: .[1;49;97mi
-000076b0: 7020 382e 382e 382e 380a 2020 2020 1b5b  p 8.8.8.8.    .[
-000076c0: 306d e903 0000 007a 4720 2020 205b 215d  0m.....zG    [!]
-000076d0: 2049 6e76 616c 6964 2073 7562 2d63 6f6d   Invalid sub-com
-000076e0: 6d61 6e64 2120 5479 7065 2060 6865 6c70  mand! Type `help
-000076f0: 6020 746f 2073 6565 2061 6c6c 2061 7661  ` to see all ava
-00007700: 696c 6162 6c65 2063 6f6d 6d61 6e64 732e  ilable commands.
-00007710: 7226 0000 0072 2800 0000 7a43 2020 2020  r&...r(...zC    
-00007720: 5b21 5d20 496e 7661 6c69 6420 636f 6d6d  [!] Invalid comm
-00007730: 616e 6421 2054 7970 6520 6068 656c 7060  and! Type `help`
-00007740: 2074 6f20 7365 6520 616c 6c20 6176 6169   to see all avai
-00007750: 6c61 626c 6520 636f 6d6d 616e 6473 2e7a  lable commands.z
-00007760: 3820 2020 205b 405d 2054 6861 6e6b 2079  8    [@] Thank y
-00007770: 6f75 2066 6f72 2075 7369 6e67 2060 5048  ou for using `PH
-00007780: 304d 4245 5260 206f 7369 6e74 2066 7261  0MBER` osint fra
-00007790: 6d65 776f 726b 203a 297a 2720 2020 205b  mework :)z'    [
-000077a0: 2b5d 2047 656e 6572 6174 696e 6720 7261  +] Generating ra
-000077b0: 6e64 6f6d 2064 6f72 6b20 7175 6572 792e  ndom dork query.
-000077c0: 2e2e 721d 0000 0072 2100 0000 7a06 2020  ..r....r!...z.  
-000077d0: 2020 3e20 2903 721e 0000 0072 1f00 0000    > ).r....r....
-000077e0: 72a4 0000 007a 2720 2020 205b 2b5d 2043  r....z'    [+] C
-000077f0: 6865 636b 696e 6720 696e 7465 726e 6574  hecking internet
-00007800: 2063 6f6e 6e65 6374 696f 6e2e 2e2e 7a17   connection...z.
-00007810: 6874 7470 733a 2f2f 7777 772e 676f 6f67  https://www.goog
-00007820: 6c65 2e63 6f6d 2f7a 2720 2020 203e 2049  le.com/z'    > I
-00007830: 6e74 6572 6e65 7420 636f 6e6e 6563 7469  nternet connecti
-00007840: 6f6e 2069 7320 6176 6169 6c61 626c 6521  on is available!
-00007850: 7a16 6874 7470 733a 2f2f 6874 7470 6269  z.https://httpbi
-00007860: 6e2e 6f72 672f 6970 da06 6f72 6967 696e  n.org/ip..origin
-00007870: 7a10 6874 7470 733a 2f2f 6964 656e 742e  z.https://ident.
-00007880: 6d65 7a15 6874 7470 733a 2f2f 6170 692e  mez.https://api.
-00007890: 6970 6966 792e 6f72 6746 7a19 2020 2020  ipify.orgFz.    
-000078a0: 3e20 5075 626c 6963 2049 5020 6164 6472  > Public IP addr
-000078b0: 6573 733a 207a 2b20 2020 203e 2049 6e74  ess: z+    > Int
-000078c0: 6572 6e65 7420 636f 6e6e 6563 7469 6f6e  ernet connection
-000078d0: 2069 7320 6e6f 7420 6176 6169 6c61 626c   is not availabl
-000078e0: 6521 7a21 2020 2020 3e20 4c6f 6361 6c20  e!z!    > Local 
-000078f0: 4950 2061 6464 7265 7373 3a20 3132 372e  IP address: 127.
-00007900: 302e 302e 3172 8f00 0000 72a3 0000 007a  0.0.1r....r....z
-00007910: 2c20 2020 205b 2b5d 2053 6176 696e 6720  ,    [+] Saving 
-00007920: 6f75 7470 7574 206f 6620 7072 6576 696f  output of previo
-00007930: 7573 2063 6f6d 6d61 6e64 2e2e 2e7a 4520  us command...zE 
-00007940: 2020 203e 204e 6f20 6f75 7470 7574 2066     > No output f
-00007950: 6f75 6e64 2120 5361 7665 7320 6f75 7470  ound! Saves outp
-00007960: 7574 206f 6620 7072 6576 696f 7573 2073  ut of previous s
-00007970: 6361 6e6e 6572 2063 6f6d 6d61 6e64 206f  canner command o
-00007980: 6e6c 7921 724a 0000 007a 3b20 2020 203e  nly!rJ...z;    >
-00007990: 204e 6f20 636f 6d6d 616e 6420 666f 756e   No command foun
-000079a0: 6421 2054 7970 6520 6068 656c 7020 7368  d! Type `help sh
-000079b0: 656c 6c60 2074 6f20 7365 6520 6d6f 7265  ell` to see more
-000079c0: 2069 6e66 6f2e e906 0000 007a 2520 2020   info......z%   
-000079d0: 201b 5b37 3b34 393b 3933 6d5b 2b5d 2045   .[7;49;93m[+] E
-000079e0: 7865 6375 7469 6e67 2063 6f6d 6d61 6e64  xecuting command
-000079f0: 3a20 7a05 1b5b 306d 0a7a 203e 2043 6f6d  : z..[0m.z > Com
-00007a00: 6d61 6e64 2065 7865 6375 7465 6420 7375  mand executed su
-00007a10: 6363 6573 7366 756c 6c79 2129 03e9 0700  ccessfully!)....
-00007a20: 0000 721f 0000 0072 a400 0000 7a05 0a20  ..r....r....z.. 
-00007a30: 2020 2029 0272 2200 0000 728a 0000 007a     ).r"...r....z
-00007a40: 200a 2020 2020 3e20 436f 6d6d 616e 6420   .    > Command 
-00007a50: 6578 6563 7574 696f 6e20 6661 696c 6564  execution failed
-00007a60: 217a 3f20 2020 203e 204e 6f20 636f 6c6f  !z?    > No colo
-00007a70: 7220 636f 6465 2066 6f75 6e64 2120 5479  r code found! Ty
-00007a80: 7065 2060 6865 6c70 2063 6861 6e67 6560  pe `help change`
-00007a90: 2074 6f20 7365 6520 6d6f 7265 2069 6e66   to see more inf
-00007aa0: 6f2e 72c2 0000 00da 0130 7a2a 2020 2020  o.r......0z*    
-00007ab0: 3e20 436f 6c6f 7220 6368 616e 6765 6420  > Color changed 
-00007ac0: 7375 6363 6573 7366 756c 6c79 2074 6f20  successfully to 
-00007ad0: 424c 4143 4b21 da01 317a 2a20 2020 203e  BLACK!..1z*    >
-00007ae0: 2043 6f6c 6f72 2063 6861 6e67 6564 2073   Color changed s
-00007af0: 7563 6365 7373 6675 6c6c 7920 746f 2057  uccessfully to W
-00007b00: 4849 5445 217a 4020 2020 205b 215d 2049  HITE!z@    [!] I
-00007b10: 6e76 616c 6964 2063 6f6c 6f72 2063 6f64  nvalid color cod
-00007b20: 6521 2054 7970 6520 6068 656c 7020 6368  e! Type `help ch
-00007b30: 616e 6765 6020 746f 2073 6565 206d 6f72  ange` to see mor
-00007b40: 6520 696e 666f 2e7a 4020 2020 203e 204e  e info.z@    > N
-00007b50: 6f20 7068 6f6e 6520 6e75 6d62 6572 2066  o phone number f
-00007b60: 6f75 6e64 2120 5479 7065 2060 6865 6c70  ound! Type `help
-00007b70: 206e 756d 6265 7260 2074 6f20 7365 6520   number` to see 
-00007b80: 6d6f 7265 2069 6e66 6f7a 3120 2020 205b  more infoz1    [
-00007b90: 2b5d 2050 6572 666f 726d 696e 6720 7265  +] Performing re
-00007ba0: 7665 7273 6520 7068 6f6e 6520 6e75 6d62  verse phone numb
-00007bb0: 6572 206c 6f6f 6b75 702e 2e2e 7a3a 2020  er lookup...z:  
-00007bc0: 2020 3e20 4e6f 2069 7020 6164 6472 6573    > No ip addres
-00007bd0: 7320 666f 756e 6421 2054 7970 6520 6068  s found! Type `h
-00007be0: 656c 7020 6970 6020 746f 2073 6565 206d  elp ip` to see m
-00007bf0: 6f72 6520 696e 666f 7a2f 2020 2020 5b2b  ore infoz/    [+
-00007c00: 5d20 5065 7266 6f72 6d69 6e67 2072 6576  ] Performing rev
-00007c10: 6572 7365 2069 7020 6164 6472 6573 7320  erse ip address 
-00007c20: 6c6f 6f6b 7570 2e2e 2e29 23da 0b73 696c  lookup...)#..sil
-00007c30: 656e 745f 6d6f 6465 7237 0000 0072 7500  ent_moder7...ru.
-00007c40: 0000 7276 0000 0072 3b00 0000 7281 0000  ..rv...r;...r...
-00007c50: 00da 0867 6574 6c6f 6769 6e72 3f00 0000  ...getloginr?...
-00007c60: 7240 0000 0072 9300 0000 da08 6e6f 6465  r@...r......node
-00007c70: 6e61 6d65 da07 7379 736e 616d 65da 0670  name..sysname..p
-00007c80: 7375 7469 6c5a 0e76 6972 7475 616c 5f6d  sutilZ.virtual_m
-00007c90: 656d 6f72 79da 0770 6572 6365 6e74 5a0b  emory..percentZ.
-00007ca0: 6370 755f 7065 7263 656e 74da 0a64 6973  cpu_percent..dis
-00007cb0: 6b5f 7573 6167 65da 0872 6561 646c 696e  k_usage..readlin
-00007cc0: 65da 0e70 6172 7365 5f61 6e64 5f62 696e  e..parse_and_bin
-00007cd0: 645a 0d73 6574 5f63 6f6d 706c 6574 6572  dZ.set_completer
-00007ce0: 72b6 0000 0072 3d00 0000 7236 0000 0072  r....r=...r6...r
-00007cf0: 4100 0000 da11 4b65 7962 6f61 7264 496e  A.....KeyboardIn
-00007d00: 7465 7272 7570 7472 a200 0000 7212 0000  terruptr....r...
-00007d10: 0072 1300 0000 7277 0000 0072 8500 0000  .r....rw...r....
-00007d20: 72a9 0000 0072 aa00 0000 729c 0000 0072  r....r....r....r
-00007d30: 4800 0000 727c 0000 0029 2072 0600 0000  H...r|...) r....
-00007d40: 5a07 6372 745f 6578 705a 0865 7870 5f69  Z.crt_expZ.exp_i
-00007d50: 6e66 6fda 0475 7365 72da 0868 6f73 746e  nfo..user..hostn
-00007d60: 616d 6572 9900 0000 5a03 7261 6d5a 0363  amer....Z.ramZ.c
-00007d70: 7075 5a04 6469 736b da03 7665 725a 0773  puZ.disk..verZ.s
-00007d80: 7973 696e 666f 7202 0000 0072 9600 0000  ysinfor....r....
-00007d90: 5a09 636d 645f 636f 6c6f 725a 0963 7274  Z.cmd_colorZ.crt
-00007da0: 5f63 6f6c 6f72 da03 636d 645a 0968 656c  _color..cmdZ.hel
-00007db0: 705f 6865 6c70 5a09 6578 6974 5f68 656c  p_helpZ.exit_hel
-00007dc0: 705a 0964 6f72 6b5f 6865 6c70 5a08 6578  pZ.dork_helpZ.ex
-00007dd0: 705f 6865 6c70 5a0a 6368 6563 6b5f 6865  p_helpZ.check_he
-00007de0: 6c70 5a0a 636c 6561 725f 6865 6c70 5a09  lpZ.clear_helpZ.
-00007df0: 7361 7665 5f68 656c 705a 0a73 6865 6c6c  save_helpZ.shell
-00007e00: 5f68 656c 705a 0969 6e66 6f5f 6865 6c70  _helpZ.info_help
-00007e10: 5a0b 6368 616e 6765 5f68 656c 705a 0b6e  Z.change_helpZ.n
-00007e20: 756d 6265 725f 6865 6c70 5a0a 656d 6169  umber_helpZ.emai
-00007e30: 6c5f 6865 6c70 5a07 6970 5f68 656c 705a  l_helpZ.ip_helpZ
-00007e40: 0970 7562 6c69 635f 6970 5a08 6578 6563  .public_ipZ.exec
-00007e50: 5f63 6d64 da06 6f75 7470 7574 7215 0000  _cmd..outputr...
-00007e60: 0072 1500 0000 7216 0000 00da 0e63 6f6e  .r....r......con
-00007e70: 7472 6f6c 5f63 656e 7465 729b 0200 0073  trol_center....s
-00007e80: b001 0000 0005 2609 0807 0802 040f 3001  ......&.......0.
-00007e90: 3401 3401 3801 3401 3c02 1c02 0204 02fc  4.4.8.4.<.......
-00007ea0: 0405 02fb 0406 02fa 0407 02f9 0408 02f8  ................
-00007eb0: 0409 02f7 0410 02f0 0817 041f 0404 0a01  ................
-00007ec0: 0a03 0801 0805 2802 0a01 0801 0401 0c01  ......(.........
-00007ed0: 1201 1201 0c01 0a01 0801 0405 0c01 1401  ................
-00007ee0: 0801 0404 0c01 0a01 0801 0404 0c01 0a01  ................
-00007ef0: 0801 0404 0c01 0a01 0801 0404 0c01 0a01  ................
-00007f00: 0801 0404 0c01 0a01 0801 0405 0a01 1201  ................
-00007f10: 0801 0405 0a01 0a01 0801 0404 0a01 0a01  ................
-00007f20: 0801 0408 0a01 0a01 0801 0405 0a01 0a01  ................
-00007f30: 0801 0203 06fd 0805 0a01 0a01 0801 0405  ................
-00007f40: 0a02 0801 1202 0801 1001 0803 1401 1c01  ................
-00007f50: 0801 0a01 0801 0401 1201 1a01 0a01 0801  ................
-00007f60: 0401 0c01 0a01 1201 0201 0a01 1001 0201  ................
-00007f70: 1601 0601 0201 1001 0601 0201 1001 0601  ................
-00007f80: 1601 0601 1601 0c01 0601 1001 1001 0e01  ................
-00007f90: 0801 0a01 0801 0401 1e01 0a01 1201 0a01  ................
-00007fa0: 1001 0a02 0a01 0a02 0801 0801 0a01 0801  ................
-00007fb0: 0401 1401 1201 1201 0c01 1001 0802 0a01  ................
-00007fc0: 0a01 1201 0a02 1001 0a02 0801 1001 0801  ................
-00007fd0: 0a01 0801 0401 0c01 0a01 0801 0401 1401  ................
-00007fe0: 1201 1201 0c01 0a01 0801 0801 1201 0a01  ................
-00007ff0: 0801 0801 1202 0801 1202 0801 1001 0803  ................
-00008000: 0a01 0801 1401 1201 1201 0c01 1201 0a01  ................
-00008010: 0a02 0a02 0801 1201 0a01 0801 1201 1201  ................
-00008020: 1201 0c01 1201 0a01 0a02 0a02 0801 1204  ................
-00008030: 0801 1003 72d4 0000 0063 0000 0000 0000  ....r....c......
-00008040: 0000 0000 0000 0000 0000 0b00 0000 4300  ..............C.
-00008050: 0000 7398 0000 007a 2474 006a 0164 0119  ..s....z$t.j.d..
-00008060: 0064 026b 0273 1e74 006a 0164 0119 0064  .d.k.s.t.j.d...d
-00008070: 036b 0272 2264 0461 0257 006e 1204 0074  .k.r"d.a.W.n...t
-00008080: 0379 3601 0001 0001 0059 006e 0230 0074  .y6......Y.n.0.t
-00008090: 0273 4274 0483 0001 007a 0a74 0583 0001  .sBt.....z.t....
-000080a0: 0057 006e 4604 0074 0679 9201 0001 0001  .W.nF..t.y......
-000080b0: 0074 0783 0001 0074 0273 8e74 0864 0564  .t.....t.s.t.d.d
-000080c0: 0164 0674 09a0 0a64 0764 0867 02a1 0167  .d.t...d.d.g...g
-000080d0: 0364 0464 0464 0464 0464 098d 0601 0074  .d.d.d.d.d.....t
-000080e0: 0b83 0001 0059 006e 0230 0064 0053 0029  .....Y.n.0.d.S.)
-000080f0: 0a4e 721e 0000 007a 022d 737a 082d 2d73  .Nr....z.-sz.--s
-00008100: 696c 656e 7454 7a26 5b23 5d20 5465 726d  ilentTz&[#] Term
-00008110: 696e 6174 696e 6720 6050 4830 4d42 4552  inating `PH0MBER
-00008120: 6020 6672 616d 6577 6f72 6b2e 2e2e 721f  ` framework...r.
-00008130: 0000 0072 2700 0000 7220 0000 0029 0572  ...r'...r ...).r
-00008140: 2200 0000 7223 0000 0072 8800 0000 7287  "...r#...r....r.
-00008150: 0000 0072 8900 0000 290c da03 7379 73da  ...r....)...sys.
-00008160: 0461 7267 7672 c500 0000 da0a 496e 6465  .argvr......Inde
-00008170: 7845 7272 6f72 72ab 0000 0072 d400 0000  xErrorr....r....
-00008180: 72ce 0000 0072 4100 0000 7237 0000 0072  r....rA...r7...r
-00008190: 7500 0000 7276 0000 0072 0300 0000 7215  u...rv...r....r.
-000081a0: 0000 0072 1500 0000 7215 0000 0072 1600  ...r....r....r..
-000081b0: 0000 da04 6d61 696e 0d04 0000 731a 0000  ....main....s...
-000081c0: 0000 0502 011c 0108 010c 0106 030a 0302  ................
-000081d0: 010a 010c 0106 0104 0124 0172 d800 0000  .........$.r....
-000081e0: 2917 7212 0000 0072 8100 0000 72d5 0000  ).r....r....r...
-000081f0: 0072 7500 0000 7290 0000 0072 cc00 0000  .ru...r....r....
-00008200: 7238 0000 0072 c900 0000 72a0 0000 0072  r8...r....r....r
-00008210: 3500 0000 72b2 0000 0072 3600 0000 72c5  5...r....r6...r.
-00008220: 0000 0072 1700 0000 7248 0000 0072 7c00  ...r....rH...r|.
-00008230: 0000 7237 0000 0072 9c00 0000 72a2 0000  ..r7...r....r...
-00008240: 0072 ab00 0000 72b6 0000 0072 d400 0000  .r....r....r....
-00008250: 72d8 0000 0072 1500 0000 7215 0000 0072  r....r....r....r
-00008260: 1500 0000 7216 0000 00da 083c 6d6f 6475  ....r......<modu
-00008270: 6c65 3e1f 0000 0073 3600 0000 0801 0801  le>....s6.......
-00008280: 0801 0801 0801 0801 0801 0801 0801 0804  ................
-00008290: 0801 0401 0405 0809 087f 0008 087f 007f  ................
-000082a0: 0070 241b 081f 081c 080a 080a 087f 007f  .p$.............
-000082b0: 0074                                     .t
+000030f0: 2d2d 2d2d 2d2d 2d7c 0a20 2020 207c 201b  -------|.    | .
+00003100: 5b31 3b34 393b 3937 6d43 6f75 6e74 7279  [1;49;97mCountry
+00003110: 2043 6170 6974 616c 1b5b 306d 2020 2020   Capital.[0m    
+00003120: 207c 207a 2d20 7c0a 2020 2020 7c20 1b5b   | z- |.    | .[
+00003130: 313b 3439 3b39 376d 436f 6e74 696e 656e  1;49;97mContinen
+00003140: 741b 5b30 6d20 2020 2020 2020 2020 2020  t.[0m           
+00003150: 7c20 7a2d 207c 0a20 2020 207c 201b 5b31  | z- |.    | .[1
+00003160: 3b34 393b 3937 6d53 6861 7269 6e67 2042  ;49;97mSharing B
+00003170: 6f72 6465 7220 7769 7468 1b5b 306d 207c  order with.[0m |
+00003180: 207a 2d20 7c0a 2020 2020 7c20 1b5b 313b   z- |.    | .[1;
+00003190: 3439 3b39 376d 466c 6167 2045 6d6f 6a69  49;97mFlag Emoji
+000031a0: 1b5b 306d 2020 2020 2020 2020 2020 7c20  .[0m          | 
+000031b0: 7a6a 207c 0a20 2020 207c 2d2d 2d2d 2d2d  zj |.    |------
+000031c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000031d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000031e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000031f0: 7c0a 2020 2020 7c20 1b5b 313b 3439 3b39  |.    | .[1;49;9
+00003200: 376d 5469 6d65 7a6f 6e65 1b5b 306d 2020  7mTimezone.[0m  
+00003210: 2020 2020 2020 2020 2020 7c20 7a2d 207c            | z- |
+00003220: 0a20 2020 207c 201b 5b31 3b34 393b 3937  .    | .[1;49;97
+00003230: 6d54 696d 657a 6f6e 6520 4162 6272 1b5b  mTimezone Abbr.[
+00003240: 306d 2020 2020 2020 207c 207a 2d20 7c0a  0m       | z- |.
+00003250: 2020 2020 7c20 1b5b 313b 3439 3b39 376d      | .[1;49;97m
+00003260: 5469 6d65 7a6f 6e65 2069 7320 4453 541b  Timezone is DST.
+00003270: 5b30 6d20 2020 2020 7c20 7a2d 207c 0a20  [0m     | z- |. 
+00003280: 2020 207c 201b 5b31 3b34 393b 3937 6d54     | .[1;49;97mT
+00003290: 696d 657a 6f6e 6520 4f66 6673 6574 1b5b  imezone Offset.[
+000032a0: 306d 2020 2020 207c 207a 2d20 7c0a 2020  0m     | z- |.  
+000032b0: 2020 7c20 1b5b 313b 3439 3b39 376d 5469    | .[1;49;97mTi
+000032c0: 6d65 7a6f 6e65 2055 5443 1b5b 306d 2020  mezone UTC.[0m  
+000032d0: 2020 2020 2020 7c20 7a2d 207c 0a20 2020        | z- |.   
+000032e0: 207c 201b 5b31 3b34 393b 3937 6d43 7572   | .[1;49;97mCur
+000032f0: 7265 6e74 2054 696d 651b 5b30 6d20 2020  rent Time.[0m   
+00003300: 2020 2020 207c 207a 2d20 7c0a 2020 2020       | z- |.    
+00003310: 7c20 1b5b 313b 3439 3b39 376d 446f 6d61  | .[1;49;97mDoma
+00003320: 696e 1b5b 306d 2020 2020 2020 2020 2020  in.[0m          
+00003330: 2020 2020 7c20 2910 723d 0000 0072 3e00      | ).r=...r>.
+00003340: 0000 721d 0000 0072 3f00 0000 7240 0000  ..r....r?...r@..
+00003350: 0072 4200 0000 7246 0000 0072 4700 0000  .rB...rF...rG...
+00003360: 7218 0000 0072 1900 0000 7216 0000 0072  r....r....r....r
+00003370: 1700 0000 da04 6a73 6f6e da0b 7374 6174  ......json..stat
+00003380: 7573 5f63 6f64 65da 0945 7863 6570 7469  us_code..Excepti
+00003390: 6f6e 7248 0000 0029 365a 0a69 705f 6164  onrH...)6Z.ip_ad
+000033a0: 6472 6573 735a 0c69 705f 6164 6472 6573  dressZ.ip_addres
+000033b0: 7365 7372 5400 0000 5a0a 7261 6e64 6f6d  sesrT...Z.random
+000033c0: 5f61 7069 da08 7265 7370 6f6e 7365 5a0d  _api..responseZ.
+000033d0: 7265 7370 6f6e 7365 5f6a 736f 6e72 4d00  response_jsonrM.
+000033e0: 0000 7258 0000 0072 5900 0000 5a0a 7265  ..rX...rY...Z.re
+000033f0: 6769 6f6e 436f 6465 725a 0000 0072 5b00  gionCoderZ...r[.
+00003400: 0000 725c 0000 0072 1e00 0000 7268 0000  ..r\...r....rh..
+00003410: 0072 6900 0000 726a 0000 0072 0c00 0000  .ri...rj...r....
+00003420: 724e 0000 00da 0165 7260 0000 0072 6100  rN.....er`...ra.
+00003430: 0000 724c 0000 0072 6200 0000 724a 0000  ..rL...rb...rJ..
+00003440: 0072 6300 0000 7264 0000 0072 6500 0000  .rc...rd...re...
+00003450: 7266 0000 0072 6700 0000 726b 0000 0072  rf...rg...rk...r
+00003460: 6c00 0000 726d 0000 0072 6e00 0000 726f  l...rm...rn...ro
+00003470: 0000 0072 7000 0000 7271 0000 0072 7200  ...rp...rq...rr.
+00003480: 0000 5a07 6970 5f74 7970 6572 7400 0000  ..Z.ip_typert...
+00003490: 7275 0000 0072 7600 0000 7277 0000 0072  ru...rv...rw...r
+000034a0: 7800 0000 5a08 666c 6167 5f69 6d67 5a0a  x...Z.flag_imgZ.
+000034b0: 666c 6167 5f65 6d6f 6a69 5a12 666c 6167  flag_emojiZ.flag
+000034c0: 5f65 6d6f 6a69 5f75 6e69 636f 6465 727b  _emoji_unicoder{
+000034d0: 0000 005a 0b74 696d 657a 6f6e 655f 6964  ...Z.timezone_id
+000034e0: 5a0d 7469 6d65 7a6f 6e65 5f61 6262 725a  Z.timezone_abbrZ
+000034f0: 0f74 696d 657a 6f6e 655f 6973 5f64 7374  .timezone_is_dst
+00003500: 5a0f 7469 6d65 7a6f 6e65 5f6f 6666 7365  Z.timezone_offse
+00003510: 745a 0c74 696d 657a 6f6e 655f 7574 635a  tZ.timezone_utcZ
+00003520: 1574 696d 657a 6f6e 655f 6375 7272 656e  .timezone_curren
+00003530: 745f 7469 6d65 721b 0000 0072 1b00 0000  t_timer....r....
+00003540: 721c 0000 00da 0969 705f 6c6f 6f6b 7570  r......ip_lookup
+00003550: d100 0000 7390 0200 0000 0304 0312 0106  ....s...........
+00003560: 0112 0104 031a 0114 030c 0110 0104 031e  ................
+00003570: 0120 0404 ff04 050e 030a 0104 0214 0108  . ..............
+00003580: 031a 0108 0108 0108 0108 0108 0108 0108  ................
+00003590: 0108 0108 0108 0108 010a 0208 0320 0120  ............. . 
+000035a0: 0120 0120 0120 0120 0120 0120 0120 0120  . . . . . . . . 
+000035b0: 0120 0120 0302 0202 fe04 0602 fa04 0702  . . ............
+000035c0: f904 0802 f804 0902 f704 0a02 f604 0c02  ................
+000035d0: f404 0d02 f304 0e02 f204 0f02 f104 1102  ................
+000035e0: ef04 1202 ee08 1508 0110 0210 0108 0102  ................
+000035f0: 0202 fe08 0708 0126 030a 0104 0214 0108  .......&........
+00003600: 030c 0108 0108 0108 0108 0108 0108 0108  ................
+00003610: 0108 0108 0108 0108 0108 0108 0108 0108  ................
+00003620: 0108 0108 0108 0108 0108 0108 0108 0108  ................
+00003630: 0108 0108 0108 010a 0208 0320 0120 0120  ........... . . 
+00003640: 0120 0120 0120 0120 0120 0120 0120 0120  . . . . . . . . 
+00003650: 0120 0120 0120 0120 0120 0120 0120 0120  . . . . . . . . 
+00003660: 0120 0120 0120 0120 0120 0120 0120 0120  . . . . . . . . 
+00003670: 0302 0202 fe04 0602 fa04 0702 f904 0902  ................
+00003680: f704 0a02 f604 0b02 f504 0c02 f404 0d02  ................
+00003690: f304 0e02 f204 0f02 f104 1002 f004 1202  ................
+000036a0: ee04 1302 ed04 1402 ec04 1502 eb04 1602  ................
+000036b0: ea04 1702 e904 1802 e804 1902 e704 1a02  ................
+000036c0: e604 1c02 e404 1d02 e304 1e02 e204 1f02  ................
+000036d0: e104 2002 e004 2202 de04 2302 dd08 2608  .. ..."...#...&.
+000036e0: 0110 0206 0102 0202 fe08 0708 0116 030a  ................
+000036f0: 0104 0214 0108 031a 0108 0108 0108 0108  ................
+00003700: 0108 0108 0108 0108 0108 0108 0108 0108  ................
+00003710: 0108 0108 0108 0108 010c 010c 010c 010c  ................
+00003720: 010c 010c 010c 010c 010c 010c 010c 010c  ................
+00003730: 010e 0208 0320 0120 0120 0120 0120 0120  ..... . . . . . 
+00003740: 0120 0120 0120 0120 0120 0120 0120 0120  . . . . . . . . 
+00003750: 0120 0120 0120 0120 0120 0120 0120 0120  . . . . . . . . 
+00003760: 0120 0120 0120 0120 0120 0120 0120 0302  . . . . . . . ..
+00003770: 0202 fe04 0602 fa04 0802 f804 0902 f704  ................
+00003780: 0a02 f604 0b02 f504 0c02 f404 0e02 f204  ................
+00003790: 0f02 f104 1002 f004 1102 ef04 1202 ee04  ................
+000037a0: 1302 ed04 1502 eb04 1602 ea04 1702 e904  ................
+000037b0: 1802 e804 1a02 e604 1b02 e504 1c02 e404  ................
+000037c0: 1d02 e304 1e02 e204 1f02 e104 2102 df04  ............!...
+000037d0: 2202 de04 2302 dd08 2608 0110 0206 0102  "...#...&.......
+000037e0: 0202 fe08 0708 0112 0272 8400 0000 6301  .........r....c.
+000037f0: 0000 0000 0000 0000 0000 0004 0000 0008  ................
+00003800: 0000 0043 0000 0073 ec00 0000 6401 6100  ...C...s....d.a.
+00003810: 7401 6402 7c00 9b00 6403 9d03 6700 6404  t.d.|...d...g.d.
+00003820: a201 6405 6406 8d03 0100 7400 6407 7c00  ..d.d.....t.d.|.
+00003830: 9b00 6408 9d03 6409 1700 3700 6100 7402  ..d...d...7.a.t.
+00003840: a003 640a 7c00 a102 7352 7401 640b 6700  ..d.|...sRt.d.g.
+00003850: 640c a201 640d 8d02 0100 640e 5300 7a14  d...d.....d.S.z.
+00003860: 7404 8300 a005 7c00 a101 7d01 6405 7d02  t.....|...}.d.}.
+00003870: 5700 6e1a 0400 7406 7980 0100 0100 0100  W.n...t.y.......
+00003880: 640f 7d01 640e 7d02 5900 6e02 3000 7407  d.}.d.}.Y.n.0.t.
+00003890: 7c00 8301 6410 7408 6411 7409 7407 7c00  |...d.t.d.t.t.|.
+000038a0: 8301 8301 1800 8301 1400 1700 7d00 7407  ............}.t.
+000038b0: 7c01 8301 6410 7408 6412 7409 7407 7c01  |...d.t.d.t.t.|.
+000038c0: 8301 8301 1800 8301 1400 1700 7d01 6413  ............}.d.
+000038d0: 7c00 9b00 6414 7c01 9b00 6415 9d05 7d03  |...d.|...d...}.
+000038e0: 740a 7c03 8301 0100 7400 7c03 6416 1700  t.|.....t.|.d...
+000038f0: 3700 6100 7c02 5300 2917 4e72 1300 0000  7.a.|.S.).Nr....
+00003900: 7221 0000 0072 2200 0000 7223 0000 0054  r!...r"...r#...T
+00003910: 7227 0000 007a 3b20 2020 201b 5b31 3b34  r'...z;    .[1;4
+00003920: 393b 3933 6d5b 235d 2052 6576 6572 7365  9;93m[#] Reverse
+00003930: 206d 6163 2061 6464 7265 7373 206c 6f6f   mac address loo
+00003940: 6b75 7020 666f 7220 1b5b 313b 3439 3b39  kup for .[1;49;9
+00003950: 366d 722a 0000 0072 2b00 0000 7a29 5e28  6mr*...r+...z)^(
+00003960: 5b30 2d39 412d 4661 2d66 5d7b 327d 5b3a  [0-9A-Fa-f]{2}[:
+00003970: 2d5d 297b 357d 285b 302d 3941 2d46 612d  -]){5}([0-9A-Fa-
+00003980: 665d 7b32 7d29 247a 3e20 2020 203e 2049  f]{2})$z>    > I
+00003990: 6e76 616c 6964 206d 6163 2061 6464 7265  nvalid mac addre
+000039a0: 7373 2066 6f72 6d61 7421 2028 4578 616d  ss format! (Exam
+000039b0: 706c 653a 2030 303a 3030 3a30 303a 3030  ple: 00:00:00:00
+000039c0: 3a30 303a 3030 2972 2c00 0000 722e 0000  :00:00)r,...r...
+000039d0: 0046 fa17 1b5b 313b 3439 3b39 316d 4e6f  .F...[1;49;91mNo
+000039e0: 7420 466f 756e 641b 5b30 6d72 3600 0000  t Found.[0mr6...
+000039f0: e91f 0000 00e9 2400 0000 75d3 0000 000a  ......$...u.....
+00003a00: 2020 2020 e294 8ce2 9480 e294 80e2 9480      ............
+00003a10: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00003a20: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00003a30: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00003a40: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00003a50: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00003a60: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00003a70: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00003a80: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00003a90: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00003aa0: e294 80e2 9480 e294 80e2 9490 0a20 2020  .............   
+00003ab0: 207c 2053 6361 6e6e 6564 204d 4143 2041   | Scanned MAC A
+00003ac0: 6464 7265 7373 3a20 1b5b 313b 3439 3b39  ddress: .[1;49;9
+00003ad0: 366d 7ae2 1b5b 306d 207c 0a20 2020 207c  6mz..[0m |.    |
+00003ae0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00003af0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00003b00: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00003b10: 2d2d 2d2d 2d2d 7c0a 2020 2020 7c20 494e  ------|.    | IN
+00003b20: 464f 524d 4154 494f 4e20 2020 7c20 4445  FORMATION   | DE
+00003b30: 5343 5249 5054 494f 4e20 2020 2020 2020  SCRIPTION       
+00003b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003b50: 2020 207c 0a20 2020 207c 2d2d 2d2d 2d2d     |.    |------
+00003b60: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00003b70: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00003b80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00003b90: 7c0a 2020 2020 7c20 1b5b 313b 3439 3b39  |.    | .[1;49;9
+00003ba0: 376d 5665 6e64 6f72 1b5b 306d 2020 2020  7mVendor.[0m    
+00003bb0: 2020 2020 7c20 725f 0000 0072 3a00 0000      | r_...r:...
+00003bc0: 290b 723d 0000 0072 3e00 0000 723f 0000  ).r=...r>...r?..
+00003bd0: 0072 4000 0000 7202 0000 00da 066c 6f6f  .r@...r......loo
+00003be0: 6b75 70da 084b 6579 4572 726f 7272 4200  kup..KeyErrorrB.
+00003bf0: 0000 7246 0000 0072 4700 0000 7248 0000  ..rF...rG...rH..
+00003c00: 0029 04da 0b6d 6163 5f61 6464 7265 7373  .)...mac_address
+00003c10: da06 7665 6e64 6f72 da07 626f 6c5f 7661  ..vendor..bol_va
+00003c20: 6c72 4e00 0000 721b 0000 0072 1b00 0000  lrN...r....r....
+00003c30: 721c 0000 00da 0a6d 6163 5f6c 6f6f 6b75  r......mac_looku
+00003c40: 7035 0200 0073 2c00 0000 0005 0403 1a01  p5...s,.........
+00003c50: 1403 0c01 1001 0403 0201 0c01 0801 0c01  ................
+00003c60: 0401 0a03 2001 2003 0202 02fe 0406 02fa  .... . .........
+00003c70: 0809 0801 0c02 728d 0000 0063 0100 0000  ......r....c....
+00003c80: 0000 0000 0000 0000 0900 0000 0a00 0000  ................
+00003c90: 4300 0000 7380 0200 0064 0161 0074 0164  C...s....d.a.t.d
+00003ca0: 0267 0064 03a2 0164 0464 058d 0301 0074  .g.d...d.d.....t
+00003cb0: 0283 0073 3274 0164 0667 0064 07a2 0164  ...s2t.d.g.d...d
+00003cc0: 0464 058d 0301 0064 0853 0074 0164 097c  .d.....d.S.t.d.|
+00003cd0: 009b 0064 0a9d 0367 0064 03a2 0164 0464  ...d...g.d...d.d
+00003ce0: 058d 0301 0074 0064 0b7c 009b 0064 0c9d  .....t.d.|...d..
+00003cf0: 0364 0d17 0037 0061 0074 03a0 0464 0e7c  .d...7.a.t...d.|
+00003d00: 00a1 0273 8074 0164 0f67 0064 07a2 0164  ...s.t.d.g.d...d
+00003d10: 108d 0201 0064 0853 007a 1274 05a0 057c  .....d.S.z.t...|
+00003d20: 00a1 017d 0164 047d 0257 006e 1001 0001  ...}.d.}.W.n....
+00003d30: 0001 0064 087d 0259 006e 0230 0074 067c  ...d.}.Y.n.0.t.|
+00003d40: 0083 0164 1174 0764 1274 0874 067c 0083  ...d.t.d.t.t.|..
+00003d50: 0183 0118 0083 0114 0017 007d 0064 137c  ...........}.d.|
+00003d60: 009b 0064 149d 037d 037c 0290 0272 407c  ...d...}.|...r@|
+00003d70: 01a0 09a1 0044 0090 015d 5c5c 027d 047d  .....D...]\\.}.}
+00003d80: 057c 0464 156b 0272 f271 de7c 0464 166b  .|.d.k.r.q.|.d.k
+00003d90: 0272 fe64 177d 047c 0464 186b 0290 0172  .r.d.}.|.d.k...r
+00003da0: 0c64 197d 047c 04a0 0a64 1a64 11a1 02a0  .d.}.|...d.d....
+00003db0: 0ba1 007d 0474 0c7c 0583 0174 0d6b 0290  ...}.t.|...t.k..
+00003dc0: 0172 e674 067c 0483 0164 1174 0764 1b74  .r.t.|...d.t.d.t
+00003dd0: 0874 067c 0483 0183 0118 0083 0114 0017  .t.|............
+00003de0: 007d 0474 067c 0564 1c19 0083 0164 1174  .}.t.|.d.....d.t
+00003df0: 0764 1274 0874 067c 0564 1c19 0083 0183  .d.t.t.|.d......
+00003e00: 0118 0083 0114 0017 007d 067c 0364 1d7c  .........}.|.d.|
+00003e10: 049b 0064 1e7c 069b 0064 1f9d 0537 007d  ...d.|...d...7.}
+00003e20: 0374 087c 0583 0164 206b 0490 0272 3c74  .t.|...d k...r<t
+00003e30: 0e64 2074 087c 0583 0183 0244 005d 3e7d  .d t.|.....D.]>}
+00003e40: 0774 067c 057c 0719 0083 0164 1174 0764  .t.|.|.....d.t.d
+00003e50: 1274 0874 067c 057c 0719 0083 0183 0118  .t.t.|.|........
+00003e60: 0083 0114 0017 007d 087c 0364 217c 089b  .......}.|.d!|..
+00003e70: 0064 1f9d 0337 007d 0390 0171 a471 de74  .d...7.}...q.q.t
+00003e80: 067c 0483 0164 1174 0764 1b74 0874 067c  .|...d.t.d.t.t.|
+00003e90: 0483 0183 0118 0083 0114 0017 007d 0474  .............}.t
+00003ea0: 067c 0583 0164 1174 0764 1274 0874 067c  .|...d.t.d.t.t.|
+00003eb0: 0583 0183 0118 0083 0114 0017 007d 057c  .............}.|
+00003ec0: 0364 1d7c 049b 0064 1e7c 059b 0064 1f9d  .d.|...d.|...d..
+00003ed0: 0537 007d 0371 de6e 207c 0364 2264 1174  .7.}.q.n |.d"d.t
+00003ee0: 0764 1274 0864 2383 0118 0083 0114 009b  .d.t.d#.........
+00003ef0: 0064 1f9d 0337 007d 037c 0364 2437 007d  .d...7.}.|.d$7.}
+00003f00: 0374 0f7c 0383 0101 0074 007c 0364 2517  .t.|.....t.|.d%.
+00003f10: 0037 0061 007c 0253 0029 264e 7213 0000  .7.a.|.S.)&Nr...
+00003f20: 0072 5000 0000 7223 0000 0054 7227 0000  .rP...r#...Tr'..
+00003f30: 0072 5100 0000 722c 0000 0046 7221 0000  .rQ...r,...Fr!..
+00003f40: 0072 2200 0000 7a35 2020 2020 1b5b 313b  .r"...z5    .[1;
+00003f50: 3439 3b39 336d 5b23 5d20 5265 7665 7273  49;93m[#] Revers
+00003f60: 6520 7768 6f69 7320 6c6f 6f6b 7570 2066  e whois lookup f
+00003f70: 6f72 201b 5b31 3b34 393b 3936 6d72 2a00  or .[1;49;96mr*.
+00003f80: 0000 722b 0000 00fa 2f5e 285b 612d 7a41  ..r+..../^([a-zA
+00003f90: 2d5a 302d 395d 2b28 2d5b 612d 7a41 2d5a  -Z0-9]+(-[a-zA-Z
+00003fa0: 302d 395d 2b29 2a5c 2e29 2b5b 612d 7a41  0-9]+)*\.)+[a-zA
+00003fb0: 2d5a 5d7b 322c 7d24 7a33 2020 2020 3e20  -Z]{2,}$z3    > 
+00003fc0: 496e 7661 6c69 6420 646f 6d61 696e 2066  Invalid domain f
+00003fd0: 6f72 6d61 7421 2028 4578 616d 706c 653a  ormat! (Example:
+00003fe0: 2065 7861 6d70 6c65 2e63 6f6d 2972 2e00   example.com)r..
+00003ff0: 0000 7236 0000 0072 8700 0000 75ce 0000  ..r6...r....u...
+00004000: 000a 2020 2020 e294 8ce2 9480 e294 80e2  ..    ..........
+00004010: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00004020: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00004030: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00004040: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00004050: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00004060: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00004070: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00004080: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00004090: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+000040a0: 9480 e294 80e2 9480 e294 80e2 9490 0a20  ............... 
+000040b0: 2020 207c 2053 6361 6e6e 6564 2044 6f6d     | Scanned Dom
+000040c0: 6169 6e3a 201b 5b31 3b34 393b 3936 6d7a  ain: .[1;49;96mz
+000040d0: bd1b 5b30 6d20 7c0a 2020 2020 7c2d 2d2d  ..[0m |.    |---
+000040e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000040f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00004100: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00004110: 2d2d 2d7c 0a20 2020 207c 2049 4e46 4f52  ---|.    | INFOR
+00004120: 4d41 5449 4f4e 2020 207c 2044 4553 4352  MATION   | DESCR
+00004130: 4950 5449 4f4e 2020 2020 2020 2020 2020  IPTION          
+00004140: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004150: 7c0a 2020 2020 7c2d 2d2d 2d2d 2d2d 2d2d  |.    |---------
+00004160: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00004170: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00004180: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d7c 7256  -------------|rV
+00004190: 0000 005a 0f65 7870 6972 6174 696f 6e5f  ...Z.expiration_
+000041a0: 6461 7465 5a0b 6578 7069 7279 5f64 6174  dateZ.expiry_dat
+000041b0: 655a 1672 6567 6973 7472 616e 745f 706f  eZ.registrant_po
+000041c0: 7374 616c 5f63 6f64 655a 0b70 6f73 7461  stal_codeZ.posta
+000041d0: 6c5f 636f 6465 da01 5fe9 0d00 0000 7201  l_code.._.....r.
+000041e0: 0000 007a 110a 2020 2020 7c20 1b5b 313b  ...z..    | .[1;
+000041f0: 3439 3b39 376d 7a07 1b5b 306d 207c 207a  49;97mz..[0m | z
+00004200: 0220 7c72 2400 0000 7a17 0a20 2020 207c  . |r$...z..    |
+00004210: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+00004220: 207a 3c0a 2020 2020 7c20 1b5b 313b 3439   z<.    | .[1;49
+00004230: 3b39 376d 496e 666f 726d 6174 696f 6e1b  ;97mInformation.
+00004240: 5b30 6d20 2020 7c20 1b5b 313b 3439 3b39  [0m   | .[1;49;9
+00004250: 316d 4e6f 7420 466f 756e 641b 5b30 6dfa  1mNot Found.[0m.
+00004260: 094e 6f74 2046 6f75 6e64 75ad 0000 000a  .Not Foundu.....
+00004270: 2020 2020 e294 94e2 9480 e294 80e2 9480      ............
+00004280: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00004290: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+000042a0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+000042b0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+000042c0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+000042d0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+000042e0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+000042f0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00004300: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00004310: e294 80e2 9480 e294 80e2 9498 723a 0000  ............r:..
+00004320: 0029 1072 3d00 0000 723e 0000 0072 1d00  .).r=...r>...r..
+00004330: 0000 723f 0000 0072 4000 0000 7212 0000  ..r?...r@...r...
+00004340: 0072 4200 0000 7246 0000 0072 4700 0000  .rB...rF...rG...
+00004350: da05 6974 656d 7372 4500 0000 da0a 6361  ..itemsrE.....ca
+00004360: 7069 7461 6c69 7a65 7273 0000 00da 046c  pitalizers.....l
+00004370: 6973 74da 0572 616e 6765 7248 0000 0029  ist..rangerH...)
+00004380: 0972 7b00 0000 5a0a 7768 6f69 735f 696e  .r{...Z.whois_in
+00004390: 666f 728c 0000 0072 4e00 0000 da03 6b65  for....rN.....ke
+000043a0: 79da 0576 616c 7565 5a07 7661 6c75 655f  y..valueZ.value_
+000043b0: 31da 0169 5a07 7661 6c75 655f 3272 1b00  1..iZ.value_2r..
+000043c0: 0000 721b 0000 0072 1c00 0000 da0c 7768  ..r....r......wh
+000043d0: 6f69 735f 6c6f 6f6b 7570 6102 0000 7352  ois_lookupa...sR
+000043e0: 0000 0000 0304 0312 0106 0112 0104 031a  ................
+000043f0: 0114 030c 0110 0104 0302 010a 0108 0106  ................
+00004400: 010a 0320 0302 0202 fe08 0806 0212 020a  ... ............
+00004410: 010c 010e 0310 030e 0120 0128 0116 010e  ......... .(....
+00004420: 0112 0128 0116 0220 0120 011a 0220 0308  ...(... . ... ..
+00004430: 0208 010c 0272 9900 0000 6301 0000 0000  .....r....c.....
+00004440: 0000 0000 0000 0005 0000 0009 0000 0043  ...............C
+00004450: 0000 0073 d201 0000 6401 6100 7401 6402  ...s....d.a.t.d.
+00004460: 6700 6403 a201 6404 6405 8d03 0100 7402  g.d...d.d.....t.
+00004470: 8300 7332 7401 6406 6700 6407 a201 6404  ..s2t.d.g.d...d.
+00004480: 6405 8d03 0100 6408 5300 7401 6409 7c00  d.....d.S.t.d.|.
+00004490: 9b00 640a 9d03 6700 6403 a201 6404 6405  ..d...g.d...d.d.
+000044a0: 8d03 0100 7403 a004 640b 7c00 a102 72e6  ....t...d.|...r.
+000044b0: 7400 640c 7c00 9b00 640d 9d03 640e 1700  t.d.|...d...d...
+000044c0: 3700 6100 7c00 640f 7405 6410 7406 7c00  7.a.|.d.t.d.t.|.
+000044d0: 8301 1800 8301 1400 1700 7d01 6411 7c01  ..........}.d.|.
+000044e0: 9b00 6412 9d03 7d02 7a2e 7407 a008 7c00  ..d...}.z.t...|.
+000044f0: a101 7d03 7409 7c03 8301 640f 7405 6410  ..}.t.|...d.t.d.
+00004500: 7406 7409 7c03 8301 8301 1800 8301 1400  t.t.|...........
+00004510: 1700 7d03 5700 6e24 0100 0100 0100 6413  ..}.W.n$......d.
+00004520: 640f 7405 6410 7406 6414 8301 1800 8301  d.t.d.t.d.......
+00004530: 1400 1700 7d03 5900 6e02 3000 6eb6 7403  ....}.Y.n.0.n.t.
+00004540: a004 6415 7c00 a102 9001 7286 7400 6416  ..d.|.....r.t.d.
+00004550: 7c00 9b00 640d 9d03 640e 1700 3700 6100  |...d...d...7.a.
+00004560: 7c00 640f 7405 6410 7406 7c00 8301 1800  |.d.t.d.t.|.....
+00004570: 8301 1400 1700 7d03 6417 7c03 9b00 6418  ......}.d.|...d.
+00004580: 9d03 7d02 7a32 7407 a00a 7c00 a101 6419  ..}.z2t...|...d.
+00004590: 1900 7d01 7409 7c01 8301 640f 7405 6410  ..}.t.|...d.t.d.
+000045a0: 7406 7409 7c01 8301 8301 1800 8301 1400  t.t.|...........
+000045b0: 1700 7d01 5700 6e24 0100 0100 0100 6413  ..}.W.n$......d.
+000045c0: 640f 7405 6410 7406 6414 8301 1800 8301  d.t.d.t.d.......
+000045d0: 1400 1700 7d01 5900 6e02 3000 6e16 7401  ....}.Y.n.0.n.t.
+000045e0: 641a 6700 6407 a201 6404 6405 8d03 0100  d.g.d...d.d.....
+000045f0: 6408 5300 641b 7c03 9b00 641c 7c01 9b00  d.S.d.|...d.|...
+00004600: 641d 9d05 7d04 740b 641e 7c02 1700 7c04  d...}.t.d.|...|.
+00004610: 1700 8301 0100 7400 641e 7c02 1700 7c04  ......t.d.|...|.
+00004620: 1700 3700 6100 6404 5300 291f 4e72 1300  ..7.a.d.S.).Nr..
+00004630: 0000 7250 0000 0072 2300 0000 5472 2700  ..rP...r#...Tr'.
+00004640: 0000 7251 0000 0072 2c00 0000 4672 2100  ..rQ...r,...Fr!.
+00004650: 0000 7222 0000 0072 8e00 0000 7a2b 2020  ..r"...r....z+  
+00004660: 2020 1b5b 313b 3439 3b39 336d 5b23 5d20    .[1;49;93m[#] 
+00004670: 444e 5320 6c6f 6f6b 7570 2066 6f72 201b  DNS lookup for .
+00004680: 5b31 3b34 393b 3936 6d72 2a00 0000 722b  [1;49;96mr*...r+
+00004690: 0000 0072 3600 0000 7287 0000 007a 2020  ...r6...r....z  
+000046a0: 2020 207c 2053 6361 6e6e 6564 2044 6f6d     | Scanned Dom
+000046b0: 6169 6e3a 201b 5b31 3b34 393b 3936 6d7a  ain: .[1;49;96mz
+000046c0: 061b 5b30 6d20 7c72 8500 0000 7291 0000  ..[0m |r....r...
+000046d0: 007a 1d5e 285b 302d 395d 7b31 2c33 7d5c  .z.^([0-9]{1,3}\
+000046e0: 2e29 7b33 7d5b 302d 395d 7b31 2c33 7d24  .){3}[0-9]{1,3}$
+000046f0: 7a33 2020 2020 1b5b 313b 3439 3b39 336d  z3    .[1;49;93m
+00004700: 5b23 5d20 5265 7665 7273 6520 444e 5320  [#] Reverse DNS 
+00004710: 6c6f 6f6b 7570 2066 6f72 201b 5b31 3b34  lookup for .[1;4
+00004720: 393b 3936 6d7a 1c20 2020 207c 2053 6361  9;96mz.    | Sca
+00004730: 6e6e 6564 2049 503a 201b 5b31 3b34 393b  nned IP: .[1;49;
+00004740: 3936 6d7a 0a1b 5b30 6d20 2020 2020 7c72  96mz..[0m     |r
+00004750: 0100 0000 7a28 2020 2020 3e20 496e 7661  ....z(    > Inva
+00004760: 6c69 6420 6970 2061 6464 7265 7373 206f  lid ip address o
+00004770: 7220 646f 6d61 696e 206e 616d 6521 7adc  r domain name!z.
+00004780: 0a20 2020 207c 2d2d 2d2d 2d2d 2d2d 2d2d  .    |----------
+00004790: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000047a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000047b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 7c0a 2020  ------------|.  
+000047c0: 2020 7c20 494e 464f 524d 4154 494f 4e20    | INFORMATION 
+000047d0: 2020 7c20 4445 5343 5249 5054 494f 4e20    | DESCRIPTION 
+000047e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000047f0: 2020 2020 2020 2020 207c 0a20 2020 207c           |.    |
+00004800: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00004810: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00004820: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00004830: 2d2d 2d2d 2d2d 7c0a 2020 2020 7c20 1b5b  ------|.    | .[
+00004840: 313b 3439 3b39 376d 4950 1b5b 306d 2020  1;49;97mIP.[0m  
+00004850: 2020 2020 2020 2020 2020 7c20 7a27 207c            | z' |
+00004860: 0a20 2020 207c 201b 5b31 3b34 393b 3937  .    | .[1;49;97
+00004870: 6d44 6f6d 6169 6e1b 5b30 6d20 2020 2020  mDomain.[0m     
+00004880: 2020 207c 2072 5f00 0000 75ae 0000 000a     | r_...u.....
+00004890: 2020 2020 e294 8ce2 9480 e294 80e2 9480      ............
+000048a0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+000048b0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+000048c0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+000048d0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+000048e0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+000048f0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00004900: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00004910: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00004920: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00004930: e294 80e2 9480 e294 80e2 9490 0a29 0c72  .............).r
+00004940: 3d00 0000 723e 0000 0072 1d00 0000 723f  =...r>...r....r?
+00004950: 0000 0072 4000 0000 7246 0000 0072 4700  ...r@...rF...rG.
+00004960: 0000 da06 736f 636b 6574 da0d 6765 7468  ....socket..geth
+00004970: 6f73 7462 796e 616d 6572 4200 0000 da0d  ostbynamerB.....
+00004980: 6765 7468 6f73 7462 7961 6464 7272 4800  gethostbyaddrrH.
+00004990: 0000 2905 5a0c 6970 5f6f 725f 646f 6d61  ..).Z.ip_or_doma
+000049a0: 696e 727b 0000 005a 1466 696e 616c 5f6f  inr{...Z.final_o
+000049b0: 7574 7075 745f 7363 616e 6e65 6472 0c00  utput_scannedr..
+000049c0: 0000 5a16 6669 6e61 6c5f 6f75 7470 7574  ..Z.final_output
+000049d0: 5f72 656d 6169 6e69 6e67 721b 0000 0072  _remainingr....r
+000049e0: 1b00 0000 721c 0000 00da 0a64 6e73 5f6c  ....r......dns_l
+000049f0: 6f6f 6b75 70ac 0200 0073 4400 0000 0003  ookup....sD.....
+00004a00: 0403 1201 0601 1201 0403 1a03 0c01 1401  ................
+00004a10: 1801 0c01 0201 0a01 2401 0601 2001 0e01  ........$... ...
+00004a20: 1401 1801 0c01 0201 0e01 2401 0601 2002  ..........$... .
+00004a30: 1201 0405 0204 02fc 0405 02fb 0809 1001  ................
+00004a40: 1002 729d 0000 0029 0372 0100 0000 7201  ..r....).r....r.
+00004a50: 0000 0072 0100 0000 630c 0000 0000 0000  ...r....c.......
+00004a60: 0000 0000 000f 0000 0008 0000 0043 0000  .............C..
+00004a70: 0073 5e01 0000 7c09 720a 7c0a 9001 725a  .s^...|.r.|...rZ
+00004a80: 7400 a001 a100 6a02 7d0c 7c04 721e 7403  t.....j.}.|.r.t.
+00004a90: 8300 0100 7c02 722e 7403 6401 7c0c 1400  ....|.r.t.d.|...
+00004aa0: 8301 0100 7403 7c07 6402 6403 8d02 0100  ....t.|.d.d.....
+00004ab0: 7404 7c00 8301 7c0c 6b00 72ce 7405 7c0c  t.|...|.k.r.t.|.
+00004ac0: 7404 7c00 8301 1800 6404 1b00 8301 7d0d  t.|.....d.....}.
+00004ad0: 7403 7c01 7c0d 1400 6402 6403 8d02 0100  t.|.|...d.d.....
+00004ae0: 7403 6405 7c06 6406 1900 9b00 6407 7c06  t.d.|.d.....d.|.
+00004af0: 6408 1900 9b00 6407 7c06 6404 1900 9b00  d.....d.|.d.....
+00004b00: 6409 9d07 6402 6403 8d02 0100 7c0b 72a4  d...d.d.....|.r.
+00004b10: 7406 7c00 8301 7d0e 6e10 7403 7407 7c00  t.|...}.n.t.t.|.
+00004b20: 8301 6402 6403 8d02 0100 7403 640a 6402  ..d.d.....t.d.d.
+00004b30: 6403 8d02 0100 7403 7c01 7c0d 1400 8301  d.....t.|.|.....
+00004b40: 0100 6e58 7403 6405 7c06 6406 1900 9b00  ..nXt.d.|.d.....
+00004b50: 6407 7c06 6408 1900 9b00 6407 7c06 6404  d.|.d.....d.|.d.
+00004b60: 1900 9b00 6409 9d07 6402 6403 8d02 0100  ....d...d.d.....
+00004b70: 7c0b 9001 720a 7406 7c00 8301 7d0e 6e10  |...r.t.|...}.n.
+00004b80: 7403 7407 7c00 8301 6402 6403 8d02 0100  t.t.|...d.d.....
+00004b90: 7403 640a 6402 6403 8d02 0100 7403 7c08  t.d.d.d.....t.|.
+00004ba0: 6402 6403 8d02 0100 7c03 9001 7244 7403  d.d.....|...rDt.
+00004bb0: 6401 7c0c 1400 8301 0100 7c05 9001 7250  d.|.......|...rP
+00004bc0: 7403 8300 0100 7c0b 9001 725a 7c0e 5300  t.....|...rZ|.S.
+00004bd0: 6400 5300 290b 4e75 0300 0000 e2b8 ba72  d.S.).Nu.......r
+00004be0: 1300 0000 2901 da03 656e 6472 5300 0000  ....)...endrS...
+00004bf0: 7a02 1b5b 7201 0000 00fa 013b 7224 0000  z..[r......;r$..
+00004c00: 00da 016d fa04 1b5b 306d 2908 da02 6f73  ...m...[0m)...os
+00004c10: da11 6765 745f 7465 726d 696e 616c 5f73  ..get_terminal_s
+00004c20: 697a 65da 0763 6f6c 756d 6e73 7248 0000  ize..columnsrH..
+00004c30: 0072 4700 0000 7246 0000 00da 0569 6e70  .rG...rF.....inp
+00004c40: 7574 7242 0000 0029 0fda 0474 6578 74da  utrB...)...text.
+00004c50: 0663 656e 7465 72da 076c 696e 655f 7570  .center..line_up
+00004c60: da09 6c69 6e65 5f64 6f77 6eda 0873 7061  ..line_down..spa
+00004c70: 6365 5f75 7072 2900 0000 7228 0000 00da  ce_upr)...r(....
+00004c80: 0f6e 6f72 6d61 6c74 7874 5f73 7461 7274  .normaltxt_start
+00004c90: 5a0d 6e6f 726d 616c 7478 745f 656e 645a  Z.normaltxt_endZ
+00004ca0: 0468 6964 655a 0c76 6572 626f 7365 5f6d  .hideZ.verbose_m
+00004cb0: 6f64 65da 0a69 6e70 7574 5f6d 6f64 65da  ode..input_mode.
+00004cc0: 0577 6964 7468 5a09 6e65 775f 7769 6474  .widthZ.new_widt
+00004cd0: 685a 0969 6e70 7574 5f76 6172 721b 0000  hZ.input_varr...
+00004ce0: 0072 1b00 0000 721c 0000 0072 3e00 0000  .r....r....r>...
+00004cf0: e402 0000 732a 0000 0000 010a 020a 030a  ....s*..........
+00004d00: 0110 020c 020c 0114 0110 012c 010e 0110  ...........,....
+00004d10: 010c 010e 022c 0110 0110 010c 020c 0212  .....,..........
+00004d20: 010c 0272 3e00 0000 6301 0000 0000 0000  ...r>...c.......
+00004d30: 0000 0000 0009 0000 000b 0000 0043 0000  .............C..
+00004d40: 0073 4201 0000 9001 7a1a 7c00 6401 1700  .sB.....z.|.d...
+00004d50: 7400 7401 a002 6402 a101 8301 1700 6403  t.t...d.......d.
+00004d60: 1700 7d01 7403 a004 a100 7d02 7403 a005  ..}.t.....}.t...
+00004d70: a100 7d03 7c02 6404 1700 7c01 1700 7d04  ..}.|.d...|...}.
+00004d80: 6405 7c01 9b00 6406 7c04 9b00 6407 9d05  d.|...d.|...d...
+00004d90: 7d05 7406 7c05 8301 0100 6408 7c01 9b00  }.t.|.....d.|...
+00004da0: 6409 7c04 9b00 640a 7400 7401 a002 640b  d.|...d.t.t...d.
+00004db0: a101 8301 9b00 640c 7400 7401 a002 640d  ......d.t.t...d.
+00004dc0: a101 8301 9b00 640e 7407 a008 a100 9b00  ......d.t.......
+00004dd0: 640f 9d0b 7d06 7409 7c04 6410 8302 8f24  d...}.t.|.d....$
+00004de0: 7d07 7c07 a00a 7c06 a101 0100 7c07 a00a  }.|...|.....|...
+00004df0: 740b a101 0100 5700 6400 0400 0400 8303  t.....W.d.......
+00004e00: 0100 6e10 3100 73c4 3000 0100 0100 0100  ..n.1.s.0.......
+00004e10: 5900 0100 740c 6411 6700 6412 a201 6413  Y...t.d.g.d...d.
+00004e20: 6413 6414 8d04 0100 7c03 6415 6b02 72fe  d.d.....|.d.k.r.
+00004e30: 6416 7c01 9b00 6417 7c01 9b00 6418 9d05  d.|...d.|...d...
+00004e40: 7d08 6e12 6419 7c01 9b00 641a 7c01 9b00  }.n.d.|...d.|...
+00004e50: 6418 9d05 7d08 7406 7c08 8301 0100 5700  d...}.t.|.....W.
+00004e60: 6413 5300 0100 0100 0100 740c 641b 6700  d.S.......t.d.g.
+00004e70: 641c a201 6413 641d 8d03 0100 5900 641e  d...d.d.....Y.d.
+00004e80: 5300 3000 6400 5300 291f 4e5a 095f 7068  S.0.d.S.).NZ._ph
+00004e90: 306d 6265 725f 7a11 2564 2d25 6d2d 2559  0mber_z.%d-%m-%Y
+00004ea0: 5f25 482d 254d 2d25 537a 042e 7478 7472  _%H-%M-%Sz..txtr
+00004eb0: 3b00 0000 7a2f 0a20 2020 201b 5b31 3b34  ;...z/.    .[1;4
+00004ec0: 393b 3933 6d5b 235d 204f 7574 7075 7420  9;93m[#] Output 
+00004ed0: 4669 6c65 204e 616d 653a 201b 5b31 3b34  File Name: .[1;4
+00004ee0: 393b 3937 6d7a 331b 5b30 6d0a 2020 2020  9;97mz3.[0m.    
+00004ef0: 1b5b 313b 3439 3b39 336d 5b23 5d20 4f75  .[1;49;93m[#] Ou
+00004f00: 7470 7574 2046 696c 6520 5061 7468 3a20  tput File Path: 
+00004f10: 1b5b 313b 3439 3b39 376d 7a0d 1b5b 306d  .[1;49;97mz..[0m
+00004f20: 0a20 2020 2020 2020 207a ab0a 2020 2020  .        z..    
+00004f30: 1b5b 313b 3439 3b39 336d 5b40 5d20 4f73  .[1;49;93m[@] Os
+00004f40: 696e 7420 6672 616d 6577 6f72 6b3a 201b  int framework: .
+00004f50: 5b31 3b34 393b 3936 6d50 4830 4d42 4552  [1;49;96mPH0MBER
+00004f60: 0a20 2020 201b 5b31 3b34 393b 3933 6d5b  .    .[1;49;93m[
+00004f70: 405d 2047 6974 6875 623a 201b 5b31 3b34  @] Github: .[1;4
+00004f80: 393b 3936 6d68 7474 7073 3a2f 2f67 6974  9;96mhttps://git
+00004f90: 6875 622e 636f 6d2f 7334 3172 346a 2f70  hub.com/s41r4j/p
+00004fa0: 686f 6d62 6572 0a0a 2020 2020 1b5b 313b  homber..    .[1;
+00004fb0: 3439 3b39 336d 5b23 5d20 4f75 7470 7574  49;93m[#] Output
+00004fc0: 2046 696c 6520 4e61 6d65 3a20 1b5b 313b   File Name: .[1;
+00004fd0: 3439 3b39 376d 7a2f 0a20 2020 201b 5b31  49;97mz/.    .[1
+00004fe0: 3b34 393b 3933 6d5b 235d 204f 7574 7075  ;49;93m[#] Outpu
+00004ff0: 7420 4669 6c65 2050 6174 683a 201b 5b31  t File Path: .[1
+00005000: 3b34 393b 3937 6d7a 230a 2020 2020 1b5b  ;49;97mz#.    .[
+00005010: 313b 3439 3b39 336d 5b23 5d20 4461 7465  1;49;93m[#] Date
+00005020: 3a20 1b5b 313b 3439 3b39 376d 7a08 2564  : .[1;49;97mz.%d
+00005030: 2d25 6d2d 2559 7a23 0a20 2020 201b 5b31  -%m-%Yz#.    .[1
+00005040: 3b34 393b 3933 6d5b 235d 2054 696d 653a  ;49;93m[#] Time:
+00005050: 201b 5b31 3b34 393b 3937 6d7a 0825 483a   .[1;49;97mz.%H:
+00005060: 254d 3a25 537a 300a 0a20 2020 201b 5b31  %M:%Sz0..    .[1
+00005070: 3b34 393b 3933 6d5b 235d 2043 6f6d 6d61  ;49;93m[#] Comma
+00005080: 6e64 2045 7865 6375 7465 643a 201b 5b31  nd Executed: .[1
+00005090: 3b34 393b 3936 6d72 3a00 0000 da01 777a  ;49;96mr:.....wz
+000050a0: 3120 2020 205b 2b5d 2045 7863 7574 6520  1    [+] Excute 
+000050b0: 666f 6c6c 6f77 696e 6720 636f 6d6d 616e  following comman
+000050c0: 6473 2074 6f20 7669 6577 206f 7574 7075  ds to view outpu
+000050d0: 743a 7223 0000 0054 2903 7228 0000 0072  t:r#...T).r(...r
+000050e0: 2900 0000 72aa 0000 00da 026e 747a 2520  )...r......ntz% 
+000050f0: 2020 201b 5b31 3b34 393b 3933 6d3e 201b     .[1;49;93m> .
+00005100: 5b31 3b34 393b 3932 6d73 6865 6c6c 206d  [1;49;92mshell m
+00005110: 6f72 6520 7a2a 1b5b 306d 0a20 2020 201b  ore z*.[0m.    .
+00005120: 5b31 3b34 393b 3933 6d3e 201b 5b31 3b34  [1;49;93m> .[1;4
+00005130: 393b 3932 6d73 6865 6c6c 2074 7970 6520  9;92mshell type 
+00005140: 72a1 0000 007a 2420 2020 201b 5b31 3b34  r....z$    .[1;4
+00005150: 393b 3933 6d3e 201b 5b31 3b34 393b 3932  9;93m> .[1;49;92
+00005160: 6d73 6865 6c6c 2063 6174 207a 2a1b 5b30  mshell cat z*.[0
+00005170: 6d0a 2020 2020 1b5b 313b 3439 3b39 336d  m.    .[1;49;93m
+00005180: 3e20 1b5b 313b 3439 3b39 326d 7368 656c  > .[1;49;92mshel
+00005190: 6c20 6c65 7373 207a 2220 2020 205b 215d  l less z"    [!]
+000051a0: 204f 7574 7075 7420 636f 756c 6420 6e6f   Output could no
+000051b0: 7420 6265 2073 6176 6564 2172 2c00 0000  t be saved!r,...
+000051c0: 7227 0000 0046 290d 7242 0000 00da 0474  r'...F).rB.....t
+000051d0: 696d 65da 0873 7472 6674 696d 6572 a200  ime..strftimer..
+000051e0: 0000 da06 6765 7463 7764 da05 756e 616d  ....getcwd..unam
+000051f0: 6572 4800 0000 da08 6675 6c6c 5f63 6d64  erH.....full_cmd
+00005200: 7244 0000 00da 046f 7065 6eda 0577 7269  rD.....open..wri
+00005210: 7465 723d 0000 0072 3e00 0000 2909 da07  ter=...r>...)...
+00005220: 7072 765f 636d 64da 0866 696c 656e 616d  prv_cmd..filenam
+00005230: 65da 0370 7764 da07 6f73 5f6e 616d 65da  e..pwd..os_name.
+00005240: 0470 6174 685a 0e66 696c 655f 7361 7665  .pathZ.file_save
+00005250: 5f69 6e66 6fda 0668 6561 6465 72da 0166  _info..header..f
+00005260: 5a07 6578 655f 636d 6472 1b00 0000 721b  Z.exe_cmdr....r.
+00005270: 0000 0072 1c00 0000 da0b 7361 7665 5f6f  ...r......save_o
+00005280: 7574 7075 7404 0300 0073 4400 0000 0001  utput....sD.....
+00005290: 0401 1a01 0801 0801 0c02 0201 02ff 0402  ................
+000052a0: 02fe 0804 0802 0204 02fc 0405 02fb 0406  ................
+000052b0: 0cfa 0407 0cf9 0409 06f7 080b 0c01 0a01  ................
+000052c0: 2802 1402 0801 1403 1202 0802 0601 0601  (...............
+000052d0: 1201 72be 0000 0063 0000 0000 0000 0000  ..r....c........
+000052e0: 0000 0000 0500 0000 0700 0000 4300 0000  ............C...
+000052f0: 7380 0000 007a 6064 0164 0269 017d 0074  s....z`d.d.i.}.t
+00005300: 006a 0164 0374 0274 03a0 0464 0464 05a1  .j.d.t.t...d.d..
+00005310: 0283 0117 007c 0064 068d 027d 017c 016a  .....|.d...}.|.j
+00005320: 0564 076b 0272 5e74 06a0 077c 016a 0864  .d.k.r^t...|.j.d
+00005330: 08a1 027d 027c 026a 0964 0964 0a64 0b69  ...}.|.j.d.d.d.i
+00005340: 0164 0c8d 026a 08a0 0aa1 007d 037c 0357  .d...j.....}.|.W
+00005350: 0053 0057 006e 0c01 0001 0001 0059 006e  .S.W.n.......Y.n
+00005360: 0230 0067 0064 0da2 017d 0474 03a0 0b7c  .0.g.d...}.t...|
+00005370: 04a1 0153 0029 0e4e 7252 0000 007a 444d  ...S.).NrR...zDM
+00005380: 6f7a 696c 6c61 2f35 2e30 2028 5831 313b  ozilla/5.0 (X11;
+00005390: 204c 696e 7578 2078 3836 5f36 343b 2072   Linux x86_64; r
+000053a0: 763a 3930 2e30 2920 4765 636b 6f2f 3230  v:90.0) Gecko/20
+000053b0: 3130 3031 3031 2046 6972 6566 6f78 2f39  100101 Firefox/9
+000053c0: 302e 307a 2068 7474 7073 3a2f 2f77 7777  0.0z https://www
+000053d0: 2e65 7870 6c6f 6974 2d64 622e 636f 6d2f  .exploit-db.com/
+000053e0: 6768 6462 2f69 e803 0000 6940 1f00 0029  ghdb/i....i@...)
+000053f0: 0172 5400 0000 7255 0000 007a 0b68 746d  .rT...rU...z.htm
+00005400: 6c2e 7061 7273 6572 5a02 6831 da05 636c  l.parserZ.h1..cl
+00005410: 6173 737a 0a63 6172 642d 7469 746c 6529  assz.card-title)
+00005420: 01da 0561 7474 7273 2916 7a1d 7369 7465  ...attrs).z.site
+00005430: 3a64 6f6d 6169 6e2e 636f 6d20 6669 6c65  :domain.com file
+00005440: 7479 7065 3a20 7064 667a 0f69 6e75 726c  type: pdfz.inurl
+00005450: 3a20 7061 7373 776f 7264 7515 0000 0069  : passwordu....i
+00005460: 6e74 6578 743a e280 9d75 7365 726e 616d  ntext:...usernam
+00005470: 65e2 809d 7a0c 6669 6c65 7479 7065 3a78  e...z.filetype:x
+00005480: 6c73 751b 0000 0066 696c 6574 7970 653a  lsu....filetype:
+00005490: 7478 7420 e280 9c75 7365 726e 616d 65e2  txt ...username.
+000054a0: 809d 7548 0000 0066 696c 6574 7970 653a  ..uH...filetype:
+000054b0: 6c6f 6720 e280 9c50 4850 2050 6172 7365  log ...PHP Parse
+000054c0: 2065 7272 6f72 e280 9d20 7c20 e280 9c50   error... | ...P
+000054d0: 4850 2057 6172 6e69 6e67 e280 9d20 7c20  HP Warning... | 
+000054e0: e280 9c50 4850 2045 7272 6f72 e280 9d75  ...PHP Error...u
+000054f0: 1700 0000 696e 7469 746c 653a 20e2 809c  ....intitle: ...
+00005500: 696e 6465 7820 6f66 e280 9d75 2200 0000  index of...u"...
+00005510: 696e 7469 746c 653a 20e2 809c 696e 6465  intitle: ...inde
+00005520: 7820 6f66 e280 9d20 e280 9c2e 6769 74e2  x of... ....git.
+00005530: 809d 7522 0000 0069 6e74 6974 6c65 3a20  ..u"...intitle: 
+00005540: e280 9c69 6e64 6578 206f 66e2 809d 20e2  ...index of... .
+00005550: 809c 2e73 766e e280 9d75 1900 0000 696e  ...svn...u....in
+00005560: 7572 6c3a e280 9d76 6965 7765 7266 7261  url:...viewerfra
+00005570: 6d65 3f6d 6f64 6575 2800 0000 696e 7572  me?modeu(...inur
+00005580: 6c3a e280 9d4d 756c 7469 4361 6d65 7261  l:...MultiCamera
+00005590: 4672 616d 653f 4d6f 6465 3d4d 6f74 696f  Frame?Mode=Motio
+000055a0: 6ee2 809d 752b 0000 0069 6e74 6974 6c65  n...u+...intitle
+000055b0: 3a20 e280 9c69 6e64 6578 206f 66e2 809d  : ...index of...
+000055c0: 20e2 809c 2e62 6173 685f 6869 7374 6f72   ....bash_histor
+000055d0: 79e2 809d 751b 0000 0069 6e74 6578 743a  y...u....intext:
+000055e0: 20e2 809c 4c61 7374 206d 6f64 6966 6965   ...Last modifie
+000055f0: 64e2 809d 7518 0000 0069 6e74 6578 743a  d...u....intext:
+00005600: 20e2 809c 496e 6465 7820 6f66 202f e280   ...Index of /..
+00005610: 9d75 1e00 0000 696e 7465 7874 3a20 e280  .u....intext: ..
+00005620: 9c50 6172 656e 7420 4469 7265 6374 6f72  .Parent Director
+00005630: 79e2 809d 7512 0000 0069 6e75 726c 3a20  y...u....inurl: 
+00005640: e280 9c61 646d 696e e280 9d75 1200 0000  ...admin...u....
+00005650: 696e 7572 6c3a 20e2 809c 6c6f 6769 6ee2  inurl: ...login.
+00005660: 809d 751e 0000 0069 6e75 726c 3a20 e280  ..u....inurl: ..
+00005670: 9c6c 6f67 696e e280 9d20 e280 9c61 646d  .login... ...adm
+00005680: 696e e280 9d75 2900 0000 696e 7572 6c3a  in...u)...inurl:
+00005690: 20e2 809c 6c6f 6769 6ee2 809d 20e2 809c   ...login... ...
+000056a0: 6164 6d69 6ee2 809d 20e2 809c 7573 6572  admin... ...user
+000056b0: e280 9d75 1b00 0000 696e 7465 7874 3ae2  ...u....intext:.
+000056c0: 809d 7072 6976 6163 7920 706f 6c69 6379  ..privacy policy
+000056d0: e280 9d7a 2222 7061 7373 776f 7264 732e  ...z""passwords.
+000056e0: 7478 7422 2069 6e74 6974 6c65 3a22 496e  txt" intitle:"In
+000056f0: 6465 7820 6f66 2275 1700 0000 696e 7465  dex of"u....inte
+00005700: 7874 3ae2 809d 4067 6d61 696c 2e63 6f6d  xt:...@gmail.com
+00005710: e280 9d29 0c72 1600 0000 7217 0000 0072  ...).r....r....r
+00005720: 4200 0000 7218 0000 00da 0772 616e 6469  B...r......randi
+00005730: 6e74 7280 0000 00da 0362 7334 5a0d 4265  ntr......bs4Z.Be
+00005740: 6175 7469 6675 6c53 6f75 7072 a600 0000  autifulSoupr....
+00005750: da04 6669 6e64 7244 0000 0072 1900 0000  ..findrD...r....
+00005760: 2905 7254 0000 00da 0a64 6f72 6b5f 7175  ).rT.....dork_qu
+00005770: 6572 795a 0b70 6172 7365 645f 6874 6d6c  eryZ.parsed_html
+00005780: 725e 0000 005a 106c 6f63 616c 5f64 6f72  r^...Z.local_dor
+00005790: 6b5f 7175 6572 7972 1b00 0000 721b 0000  k_queryr....r...
+000057a0: 0072 1c00 0000 72c4 0000 002f 0300 0073  .r....r..../...s
+000057b0: 1600 0000 0002 0201 0801 1e03 0a02 0e03  ................
+000057c0: 1802 0a01 0601 0603 0807 72c4 0000 0063  ..........r....c
+000057d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000057e0: 0900 0000 4300 0000 739a 0000 0074 00a0  ....C...s....t..
+000057f0: 0174 006a 0264 016b 0272 1264 026e 0264  .t.j.d.k.r.d.n.d
+00005800: 03a1 0101 0074 0364 0464 0564 0664 0774  .....t.d.d.d.d.t
+00005810: 04a0 0567 0064 08a2 01a1 0167 0364 0964  ...g.d.....g.d.d
+00005820: 0a8d 0401 0074 0364 0b64 0564 0664 0774  .....t.d.d.d.d.t
+00005830: 04a0 0567 0064 08a2 01a1 0167 0364 0c8d  ...g.d.....g.d..
+00005840: 0301 0074 0364 0d64 0564 0664 0774 04a0  ...t.d.d.d.d.t..
+00005850: 0567 0064 08a2 01a1 0167 0364 0964 0e8d  .g.d.....g.d.d..
+00005860: 0401 0074 0364 0f64 0564 0664 0774 04a0  ...t.d.d.d.d.t..
+00005870: 0567 0064 08a2 01a1 0167 0364 0964 0e8d  .g.d.....g.d.d..
+00005880: 0401 0064 0053 0029 104e 72af 0000 00da  ...d.S.).Nr.....
+00005890: 0363 6c73 7205 0000 0075 7700 0000 e294  .clsr....uw.....
+000058a0: 8020 e296 92e2 9688 e296 80e2 9680 e296  . ..............
+000058b0: 8820 e296 92e2 9688 e296 91e2 9692 e296  . ..............
+000058c0: 8820 e296 88e2 9680 e296 80e2 9688 20e2  . ............ .
+000058d0: 9692 e296 88e2 9680 e296 84e2 9680 e296  ................
+000058e0: 8820 e296 92e2 9688 e296 80e2 9680 e296  . ..............
+000058f0: 8820 e296 92e2 9688 e296 80e2 9680 e296  . ..............
+00005900: 8020 e296 92e2 9688 e296 80e2 9680 e296  . ..............
+00005910: 8820 e294 8072 3600 0000 7224 0000 0072  . ...r6...r$...r
+00005920: 2500 0000 2907 722d 0000 00e9 5c00 0000  %...).r-....\...
+00005930: 7226 0000 00e9 5e00 0000 e95f 0000 00e9  r&....^...._....
+00005940: 6000 0000 e961 0000 0054 2903 72a7 0000  `....a...T).r...
+00005950: 0072 2800 0000 72aa 0000 0075 7700 0000  .r(...r....uw...
+00005960: e294 8020 e296 92e2 9688 e296 84e2 9684  ... ............
+00005970: e296 8820 e296 92e2 9688 e296 80e2 9680  ... ............
+00005980: e296 8820 e296 88e2 9684 e296 80e2 9688  ... ............
+00005990: 20e2 9692 e296 88e2 9692 e296 88e2 9692   ...............
+000059a0: e296 8820 e296 92e2 9688 e296 80e2 9680  ... ............
+000059b0: e296 8420 e296 92e2 9688 e296 80e2 9680  ... ............
+000059c0: e296 8020 e296 92e2 9688 e296 84e2 9684  ... ............
+000059d0: e296 8020 e294 8029 0272 a700 0000 7228  ... ...).r....r(
+000059e0: 0000 0075 7700 0000 e294 8020 e296 92e2  ...uw...... ....
+000059f0: 9688 e296 91e2 9691 e296 9120 e296 92e2  ........... ....
+00005a00: 9688 e296 91e2 9692 e296 8820 e296 88e2  ........... ....
+00005a10: 9684 e296 84e2 9688 20e2 9692 e296 88e2  ........ .......
+00005a20: 9691 e296 91e2 9692 e296 8820 e296 92e2  ........... ....
+00005a30: 9688 e296 84e2 9684 e296 8820 e296 92e2  ........... ....
+00005a40: 9688 e296 84e2 9684 e296 8420 e296 92e2  ........... ....
+00005a50: 9688 e296 91e2 9692 e296 8820 e294 8029  ........... ...)
+00005a60: 0372 a700 0000 7228 0000 0072 2900 0000  .r....r(...r)...
+00005a70: 7a29 4f53 494e 542d 4652 414d 4557 4f52  z)OSINT-FRAMEWOR
+00005a80: 4b20 2020 2020 2020 2020 2020 2020 2020  K               
+00005a90: 2020 2020 4073 3431 7234 6a29 0672 a200      @s41r4j).r..
+00005aa0: 0000 da06 7379 7374 656d da04 6e61 6d65  ....system..name
+00005ab0: 723e 0000 0072 1800 0000 7219 0000 0072  r>...r....r....r
+00005ac0: 1b00 0000 721b 0000 0072 1b00 0000 721c  ....r....r....r.
+00005ad0: 0000 00da 046c 6f67 6f4b 0300 0073 0a00  .....logoK...s..
+00005ae0: 0000 0002 1803 2001 1e01 2001 72cd 0000  ...... ... .r...
+00005af0: 0063 0200 0000 0000 0000 0000 0000 0400  .c..............
+00005b00: 0000 0300 0000 0300 0000 7332 0000 0074  ..........s2...t
+00005b10: 007d 0287 0066 0164 0164 0284 087c 0244  .}...f.d.d...|.D
+00005b20: 0083 017d 037c 0174 017c 0383 016b 0072  ...}.|.t.|...k.r
+00005b30: 2a7c 037c 0119 0053 0064 0053 0064 0053  *|.|...S.d.S.d.S
+00005b40: 0029 034e 6301 0000 0000 0000 0000 0000  .).Nc...........
+00005b50: 0002 0000 0005 0000 0013 0000 0073 1a00  .............s..
+00005b60: 0000 6700 7c00 5d12 7d01 7c01 a000 8800  ..g.|.].}.|.....
+00005b70: a101 7204 7c01 9102 7104 5300 721b 0000  ..r.|...q.S.r...
+00005b80: 0029 01da 0a73 7461 7274 7377 6974 6829  .)...startswith)
+00005b90: 02da 022e 3072 9800 0000 a901 72a6 0000  ....0r......r...
+00005ba0: 0072 1b00 0000 721c 0000 00da 0a3c 6c69  .r....r......<li
+00005bb0: 7374 636f 6d70 3e57 0300 00f3 0000 0000  stcomp>W........
+00005bc0: 7a1d 636f 6d70 6c65 7465 722e 3c6c 6f63  z.completer.<loc
+00005bd0: 616c 733e 2e3c 6c69 7374 636f 6d70 3e29  als>.<listcomp>)
+00005be0: 02da 1261 7661 6c69 6162 6c65 5f63 6f6d  ...avaliable_com
+00005bf0: 6d61 6e64 7372 4700 0000 2904 72a6 0000  mandsrG...).r...
+00005c00: 00da 0573 7461 7465 da08 636f 6d6d 616e  ...state..comman
+00005c10: 6473 da07 6f70 7469 6f6e 7372 1b00 0000  ds..optionsr....
+00005c20: 72d0 0000 0072 1c00 0000 da09 636f 6d70  r....r......comp
+00005c30: 6c65 7465 7255 0300 0073 0a00 0000 0001  leterU...s......
+00005c40: 0401 1201 0c01 0802 72d7 0000 0063 0000  ........r....c..
+00005c50: 0000 0000 0000 0000 0000 2600 0000 1300  ..........&.....
+00005c60: 0000 4300 0000 73f2 0c00 0074 0073 2674  ..C...s....t.s&t
+00005c70: 0164 0164 0264 0374 02a0 0367 0064 04a2  .d.d.d.t...g.d..
+00005c80: 01a1 0167 0364 0564 0564 0564 068d 0501  ...g.d.d.d.d....
+00005c90: 0067 0064 07a2 017d 007c 0064 0819 007d  .g.d...}.|.d...}
+00005ca0: 0164 097d 0264 0a74 0474 05a0 06a1 0083  .d.}.d.t.t......
+00005cb0: 0117 0064 0b17 0064 0c74 0764 0d74 0874  ...d...d.t.d.t.t
+00005cc0: 0474 05a0 06a1 0083 0183 0118 0083 0114  .t..............
+00005cd0: 0017 007d 0364 0a74 0474 05a0 09a1 006a  ...}.d.t.t.....j
+00005ce0: 0a83 0117 0064 0b17 0064 0c74 0764 0d74  .....d...d.t.d.t
+00005cf0: 0874 0474 05a0 09a1 006a 0a83 0183 0118  .t.t.....j......
+00005d00: 0083 0114 0017 007d 0464 0a74 0474 05a0  .......}.d.t.t..
+00005d10: 09a1 006a 0b83 0117 0064 0b17 0064 0c74  ...j.....d...d.t
+00005d20: 0764 0d74 0874 0474 05a0 09a1 006a 0b83  .d.t.t.t.....j..
+00005d30: 0183 0118 0083 0114 0017 007d 0564 0a74  ...........}.d.t
+00005d40: 0474 0ca0 0da1 006a 0e83 0117 0064 0e17  .t.....j.....d..
+00005d50: 0064 0b17 0064 0c74 0764 0f74 0874 0474  .d...d.t.d.t.t.t
+00005d60: 0ca0 0da1 006a 0e83 0183 0118 0083 0114  .....j..........
+00005d70: 0017 007d 0664 0a74 0474 0ca0 0fa1 0083  ...}.d.t.t......
+00005d80: 0117 0064 0e17 0064 0b17 0064 0c74 0764  ...d...d...d.t.d
+00005d90: 1074 0874 0474 0ca0 0fa1 0083 0183 0118  .t.t.t..........
+00005da0: 0083 0114 0017 007d 0764 0a74 0474 0ca0  .......}.d.t.t..
+00005db0: 1064 11a1 016a 0e83 0117 0064 0e17 0064  .d...j.....d...d
+00005dc0: 0b17 0064 0c74 0764 0f74 0874 0474 0ca0  ...d.t.d.t.t.t..
+00005dd0: 1064 11a1 016a 0e83 0183 0118 0083 0114  .d...j..........
+00005de0: 0017 007d 0864 0a74 0464 12a0 1174 12a0  ...}.d.t.d...t..
+00005df0: 1364 1364 1474 14a0 15a1 0016 00a1 02a1  .d.d.t..........
+00005e00: 0183 0117 0064 0b17 0064 0c74 0764 0d74  .....d...d.t.d.t
+00005e10: 0874 0464 12a0 1174 12a0 1364 1364 1474  .t.d...t...d.d.t
+00005e20: 14a0 15a1 0016 00a1 02a1 0183 0183 0118  ................
+00005e30: 0083 0114 0017 007d 0964 0a74 0474 05a0  .......}.d.t.t..
+00005e40: 09a1 006a 1683 0117 0064 0b17 0064 0c74  ...j.....d...d.t
+00005e50: 0764 0d74 0874 0474 05a0 09a1 006a 1683  .d.t.t.t.....j..
+00005e60: 0183 0118 0083 0114 0017 007d 0a64 1564  ...........}.d.d
+00005e70: 0c74 0764 0d74 0874 0464 1683 0183 0118  .t.d.t.t.d......
+00005e80: 0083 0114 0017 007d 0b64 177c 039b 0064  .......}.d.|...d
+00005e90: 187c 049b 0064 197c 059b 0064 1a7c 0a9b  .|...d.|...d.|..
+00005ea0: 0064 1b7c 099b 0064 1c7c 069b 0064 1d7c  .d.|...d.|...d.|
+00005eb0: 079b 0064 1e7c 089b 0064 1f7c 0b9b 0064  ...d.|...d.|...d
+00005ec0: 209d 137d 0c64 217d 0d67 0064 22a2 017d   ..}.d!}.g.d"..}
+00005ed0: 0e64 237d 0f74 17a0 1864 24a1 0101 0074  .d#}.t...d$....t
+00005ee0: 17a0 1974 1aa1 0101 0064 2564 2667 027d  ...t.....d%d&g.}
+00005ef0: 107c 1064 0219 007d 1174 0164 277c 03a0  .|.d...}.t.d'|..
+00005f00: 1ba1 009b 0064 287c 019b 0064 297c 119b  .....d(|...d)|..
+00005f10: 009d 0664 0564 0564 2a8d 03a0 1ba1 007d  ...d.d.d*......}
+00005f20: 127c 1264 2b6b 0290 0272 f27c 0064 0219  .|.d+k...r.|.d..
+00005f30: 007d 0164 2361 1c74 1d7c 0d83 0101 0074  .}.d#a.t.|.....t
+00005f40: 02a0 037c 0ea1 017d 1374 1d64 2c7c 139b  ...|...}.t.d,|..
+00005f50: 0064 0b9d 0383 0101 0090 096e f47c 1264  .d.........n.|.d
+00005f60: 0064 2d85 0219 0064 2b6b 0290 0572 5c7c  .d-....d+k...r\|
+00005f70: 1264 2e17 0064 2d19 0064 0c6b 0290 0572  .d...d-..d.k...r
+00005f80: 3c7c 1264 2f64 0085 0219 007d 127c 1264  <|.d/d.....}.|.d
+00005f90: 2b6b 0290 0372 447c 0064 0219 007d 0164  +k...rD|.d...}.d
+00005fa0: 307d 1474 1d7c 1483 0101 0090 0571 547c  0}.t.|.......qT|
+00005fb0: 1264 316b 0290 0373 587c 1264 326b 0290  .d1k...sX|.d2k..
+00005fc0: 0372 707c 0064 0219 007d 0164 337d 1574  .rp|.d...}.d3}.t
+00005fd0: 1d7c 1583 0101 0090 0571 547c 1264 346b  .|.......qT|.d4k
+00005fe0: 0290 0372 927c 0064 0219 007d 0164 357d  ...r.|.d...}.d5}
+00005ff0: 1674 1d7c 1683 0101 0090 0571 547c 1264  .t.|.......qT|.d
+00006000: 366b 0290 0372 b47c 0064 0219 007d 0164  6k...r.|.d...}.d
+00006010: 377d 1774 1d7c 1783 0101 0090 0571 547c  7}.t.|.......qT|
+00006020: 1264 386b 0290 0372 d67c 0064 0219 007d  .d8k...r.|.d...}
+00006030: 0164 397d 1874 1d7c 1883 0101 0090 0571  .d9}.t.|.......q
+00006040: 547c 1264 3a6b 0290 0372 f87c 0064 0219  T|.d:k...r.|.d..
+00006050: 007d 0164 3b7d 1974 1d7c 1983 0101 0090  .}.d;}.t.|......
+00006060: 0571 547c 1264 3c6b 0290 0472 1a7c 0064  .qT|.d<k...r.|.d
+00006070: 0219 007d 0164 3d7d 1a74 1d7c 1a83 0101  ...}.d=}.t.|....
+00006080: 0090 0571 547c 1264 0064 2f85 0219 0064  ...qT|.d.d/....d
+00006090: 3e6b 0290 0472 427c 0064 0219 007d 0164  >k...rB|.d...}.d
+000060a0: 3f7d 1b74 1d7c 1b83 0101 006e f87c 1264  ?}.t.|.....n.|.d
+000060b0: 406b 0290 0472 627c 0064 0219 007d 0164  @k...rb|.d...}.d
+000060c0: 417d 1c74 1d7c 1c83 0101 006e d87c 1264  A}.t.|.....n.|.d
+000060d0: 426b 0290 0472 827c 0064 0219 007d 0164  Bk...r.|.d...}.d
+000060e0: 437d 1d74 1d7c 1d83 0101 006e b87c 1264  C}.t.|.....n.|.d
+000060f0: 446b 0290 0472 a27c 0064 0219 007d 0164  Dk...r.|.d...}.d
+00006100: 457d 1e74 1d7c 1e83 0101 006e 987c 1264  E}.t.|.....n.|.d
+00006110: 466b 0290 0472 c27c 0064 0219 007d 0164  Fk...r.|.d...}.d
+00006120: 477d 1f74 1d7c 1f83 0101 006e 787c 1264  G}.t.|.....nx|.d
+00006130: 486b 0290 0472 e27c 0064 0219 007d 0164  Hk...r.|.d...}.d
+00006140: 497d 2074 1d7c 2083 0101 006e 587c 1264  I} t.| ....nX|.d
+00006150: 4a6b 0290 0572 027c 0064 0219 007d 0164  Jk...r.|.d...}.d
+00006160: 4b7d 2174 1d7c 2183 0101 006e 387c 1264  K}!t.|!....n8|.d
+00006170: 4c6b 0290 0572 227c 0064 0219 007d 0164  Lk...r"|.d...}.d
+00006180: 4d7d 2274 1d7c 2283 0101 006e 187c 0064  M}"t.|"....n.|.d
+00006190: 4e19 007d 0174 0164 4f67 0064 50a2 0164  N..}.t.dOg.dP..d
+000061a0: 518d 0201 006e 187c 0064 4e19 007d 0174  Q....n.|.dN..}.t
+000061b0: 0164 5267 0064 50a2 0164 518d 0201 0064  .dRg.dP..dQ....d
+000061c0: 2361 1c90 076e 8a7c 1264 316b 0290 0573  #a...n.|.d1k...s
+000061d0: 707c 1264 326b 0290 0572 9a74 0090 0573  p|.d2k...r.t...s
+000061e0: 9274 0164 5364 0264 0374 02a0 0367 0064  .t.dSd.d.t...g.d
+000061f0: 04a2 01a1 0167 0364 518d 0201 0074 1e82  .....g.dQ....t..
+00006200: 0190 076e 4c7c 1264 346b 0290 0572 dc7c  ...nL|.d4k...r.|
+00006210: 0064 0219 007d 0164 2361 1c74 0164 5467  .d...}.d#a.t.dTg
+00006220: 0064 55a2 0164 0564 568d 0301 0074 0164  .dU..d.dV....t.d
+00006230: 5774 1f83 0017 0067 0064 58a2 0164 518d  Wt.....g.dX..dQ.
+00006240: 0201 0090 076e 0a7c 1264 366b 0290 0572  .....n.|.d6k...r
+00006250: fe7c 0064 0219 007d 0164 2361 1c74 1d7c  .|.d...}.d#a.t.|
+00006260: 0283 0101 0090 066e e87c 1264 386b 0290  .......n.|.d8k..
+00006270: 0672 fe74 0164 5967 0064 55a2 0164 0564  .r.t.dYg.dU..d.d
+00006280: 568d 0301 007a a674 20a0 2164 5aa1 0101  V....z.t .!dZ...
+00006290: 0074 0164 5b67 0064 58a2 0164 518d 0201  .t.d[g.dX..dQ...
+000062a0: 007a 1674 20a0 2164 5ca1 01a0 22a1 0064  .z.t .!d\..."..d
+000062b0: 5d19 007d 2357 006e 4c01 0001 0001 007a  ]..}#W.nL......z
+000062c0: 1074 20a0 2164 5ea1 016a 237d 2357 006e  .t .!d^..j#}#W.n
+000062d0: 2e01 0001 0001 007a 1074 20a0 2164 5fa1  .......z.t .!d_.
+000062e0: 016a 237d 2357 006e 1001 0001 0001 0064  .j#}#W.n.......d
+000062f0: 607d 2359 006e 0230 0059 006e 0230 0059  `}#Y.n.0.Y.n.0.Y
+00006300: 006e 0230 007c 2390 0672 b674 0164 617c  .n.0.|#..r.t.da|
+00006310: 239b 009d 0267 0064 58a2 0164 518d 0201  #....g.dX..dQ...
+00006320: 007c 0064 0819 007d 0157 006e 3401 0001  .|.d...}.W.n4...
+00006330: 0001 0074 0164 6267 0064 50a2 0164 518d  ...t.dbg.dP..dQ.
+00006340: 0201 0074 0164 6367 0064 58a2 0164 518d  ...t.dcg.dX..dQ.
+00006350: 0201 007c 0064 4e19 007d 0159 006e 0230  ...|.dN..}.Y.n.0
+00006360: 0064 2361 1c90 056e e87c 1264 3a6b 0290  .d#a...n.|.d:k..
+00006370: 0772 327c 0064 0819 007d 0164 2361 1c74  .r2|.d...}.d#a.t
+00006380: 05a0 2474 056a 2564 646b 0290 0772 2864  ..$t.j%ddk...r(d
+00006390: 656e 0264 3aa1 0101 0090 056e b47c 1264  en.d:......n.|.d
+000063a0: 3c6b 0290 0772 9674 0164 6667 0064 55a2  <k...r.t.dfg.dU.
+000063b0: 0164 0564 568d 0301 0074 1c64 236b 0290  .d.dV....t.d#k..
+000063c0: 0772 7274 0164 6767 0064 50a2 0164 518d  .rrt.dgg.dP..dQ.
+000063d0: 0201 007c 0064 6819 007d 016e 1c74 267c  ...|.dh..}.n.t&|
+000063e0: 0f83 0190 0772 867c 0064 0819 007d 016e  .....r.|.d...}.n
+000063f0: 087c 0064 4e19 007d 0164 2361 1c90 056e  .|.dN..}.d#a...n
+00006400: 507c 1264 3e6b 0290 0772 c07c 0064 6819  P|.d>k...r.|.dh.
+00006410: 007d 0164 2361 1c74 0164 6967 0064 50a2  .}.d#a.t.dig.dP.
+00006420: 0164 518d 0201 0090 056e 267c 1264 0064  .dQ......n&|.d.d
+00006430: 2f85 0219 0064 3e6b 0290 0872 747c 1264  /....d>k...rt|.d
+00006440: 2e17 0064 2f19 0064 0c6b 0290 0872 547c  ...d/..d.k...rT|
+00006450: 1264 6a64 0085 0219 007d 1264 6b74 047c  .djd.....}.dkt.|
+00006460: 1283 019b 0064 6c9d 037d 2474 1d7c 2483  .....dl..}$t.|$.
+00006470: 0101 0074 05a0 247c 12a1 017d 257c 2564  ...t..$|...}%|%d
+00006480: 086b 0290 0872 3874 0164 6d67 0064 6ea2  .k...r8t.dmg.dn.
+00006490: 0164 6f64 708d 0301 007c 0064 0819 007d  .dodp....|.d...}
+000064a0: 016e 1a74 0164 7167 0064 72a2 0164 6f64  .n.t.dqg.dr..dod
+000064b0: 708d 0301 007c 0064 4e19 007d 016e 187c  p....|.dN..}.n.|
+000064c0: 0064 4e19 007d 0174 0164 5267 0064 50a2  .dN..}.t.dRg.dP.
+000064d0: 0164 518d 0201 0064 2361 1c90 046e 727c  .dQ....d#a...nr|
+000064e0: 1264 406b 0290 0872 967c 0064 0219 007d  .d@k...r.|.d...}
+000064f0: 0164 2361 1c74 1d7c 0c83 0101 0090 046e  .d#a.t.|.......n
+00006500: 507c 1264 426b 0290 0872 c07c 0064 6819  P|.dBk...r.|.dh.
+00006510: 007d 0164 2361 1c74 0164 7367 0064 50a2  .}.d#a.t.dsg.dP.
+00006520: 0164 518d 0201 0090 046e 267c 1264 0064  .dQ......n&|.d.d
+00006530: 6a85 0219 0064 426b 0290 0972 827c 1264  j....dBk...r.|.d
+00006540: 2e17 0064 6a19 0064 0c6b 0290 0972 627c  ...dj..d.k...rb|
+00006550: 1264 7464 0085 0219 007d 127c 1264 756b  .dtd.....}.|.duk
+00006560: 0290 0972 1c7c 1064 0819 007d 117c 0064  ...r.|.d...}.|.d
+00006570: 0819 007d 0174 0164 7667 0064 58a2 0164  ...}.t.dvg.dX..d
+00006580: 518d 0201 006e 447c 1264 776b 0290 0972  Q....nD|.dwk...r
+00006590: 487c 1064 0219 007d 117c 0064 0819 007d  H|.d...}.|.d...}
+000065a0: 0174 0164 7867 0064 58a2 0164 518d 0201  .t.dxg.dX..dQ...
+000065b0: 006e 187c 0064 4e19 007d 0174 0164 7967  .n.|.dN..}.t.dyg
+000065c0: 0064 50a2 0164 518d 0201 006e 187c 0064  .dP..dQ....n.|.d
+000065d0: 4e19 007d 0174 0164 5267 0064 50a2 0164  N..}.t.dRg.dP..d
+000065e0: 518d 0201 0064 2361 1c90 036e 647c 1264  Q....d#a...nd|.d
+000065f0: 446b 0290 0972 a87c 0064 6819 007d 0174  Dk...r.|.dh..}.t
+00006600: 0164 7a67 0064 50a2 0164 518d 0201 0090  .dzg.dP..dQ.....
+00006610: 036e 3e7c 1264 0064 6a85 0219 0064 446b  .n>|.d.dj....dDk
+00006620: 0290 0a72 2c7c 1261 277c 1264 2e17 0064  ...r,|.a'|.d...d
+00006630: 6a19 0064 0c6b 0290 0a72 107c 1264 7464  j..d.k...r.|.dtd
+00006640: 0085 0219 007d 1274 0164 7b67 0064 55a2  .....}.t.d{g.dU.
+00006650: 0164 0564 568d 0301 0074 287c 1283 0190  .d.dV....t(|....
+00006660: 0a72 027c 0064 2d19 007d 016e 0c7c 0064  .r.|.d-..}.n.|.d
+00006670: 4e19 007d 0164 2361 1c6e 187c 0064 4e19  N..}.d#a.n.|.dN.
+00006680: 007d 0174 0164 5267 0064 50a2 0164 518d  .}.t.dRg.dP..dQ.
+00006690: 0201 0090 026e ba7c 1264 4a6b 0290 0a72  .....n.|.dJk...r
+000066a0: 527c 0064 6819 007d 0174 0164 7c67 0064  R|.dh..}.t.d|g.d
+000066b0: 50a2 0164 518d 0201 0090 026e 947c 1264  P..dQ......n.|.d
+000066c0: 0064 6885 0219 0064 4a6b 0290 0a72 d67c  .dh....dJk...r.|
+000066d0: 1261 277c 1264 2e17 0064 6819 0064 0c6b  .a'|.d...dh..d.k
+000066e0: 0290 0a72 ba7c 1264 4e64 0085 0219 007d  ...r.|.dNd.....}
+000066f0: 1274 0164 7d67 0064 55a2 0164 0564 568d  .t.d}g.dU..d.dV.
+00006700: 0301 0074 297c 1283 0190 0a72 ac7c 0064  ...t)|.....r.|.d
+00006710: 2d19 007d 016e 0c7c 0064 4e19 007d 0164  -..}.n.|.dN..}.d
+00006720: 2361 1c6e 187c 0064 4e19 007d 0174 0164  #a.n.|.dN..}.t.d
+00006730: 5267 0064 50a2 0164 518d 0201 0090 026e  Rg.dP..dQ......n
+00006740: 107c 1264 4c6b 0290 0a72 fc7c 0064 6819  .|.dLk...r.|.dh.
+00006750: 007d 0174 0164 7e67 0064 50a2 0164 518d  .}.t.d~g.dP..dQ.
+00006760: 0201 0090 016e ea7c 1264 0064 4e85 0219  .....n.|.d.dN...
+00006770: 0064 4c6b 0290 0b72 807c 1261 277c 1264  .dLk...r.|.a'|.d
+00006780: 2e17 0064 4e19 0064 0c6b 0290 0b72 647c  ...dN..d.k...rd|
+00006790: 1264 2d64 0085 0219 007d 1274 0164 7f67  .d-d.....}.t.d.g
+000067a0: 0064 55a2 0164 0564 568d 0301 0074 2a7c  .dU..d.dV....t*|
+000067b0: 1283 0190 0b72 567c 0064 2d19 007d 016e  .....rV|.d-..}.n
+000067c0: 0c7c 0064 4e19 007d 0164 2361 1c6e 187c  .|.dN..}.d#a.n.|
+000067d0: 0064 4e19 007d 0174 0164 5267 0064 50a2  .dN..}.t.dRg.dP.
+000067e0: 0164 518d 0201 0090 016e 667c 1264 466b  .dQ......nf|.dFk
+000067f0: 0290 0b72 a67c 0064 6819 007d 0174 0164  ...r.|.dh..}.t.d
+00006800: 8067 0064 50a2 0164 518d 0201 0090 016e  .g.dP..dQ......n
+00006810: 407c 1264 0064 2f85 0219 0064 466b 0290  @|.d.d/....dFk..
+00006820: 0c72 287c 1261 277c 1264 2e17 0064 2f19  .r(|.a'|.d...d/.
+00006830: 0064 0c6b 0290 0c72 0e7c 1264 6a64 0085  .d.k...r.|.djd..
+00006840: 0219 007d 1274 0164 8167 0064 55a2 0164  ...}.t.d.g.dU..d
+00006850: 0564 568d 0301 0074 2b7c 1283 0190 0c72  .dV....t+|.....r
+00006860: 007c 0064 2d19 007d 016e 0c7c 0064 4e19  .|.d-..}.n.|.dN.
+00006870: 007d 0164 2361 1c6e 187c 0064 4e19 007d  .}.d#a.n.|.dN..}
+00006880: 0174 0164 5267 0064 50a2 0164 518d 0201  .t.dRg.dP..dQ...
+00006890: 006e be7c 1264 486b 0290 0c72 4c7c 0064  .n.|.dHk...rL|.d
+000068a0: 6819 007d 0174 0164 8267 0064 50a2 0164  h..}.t.d.g.dP..d
+000068b0: 518d 0201 006e 9a7c 1264 0064 4e85 0219  Q....n.|.d.dN...
+000068c0: 0064 486b 0290 0c72 ce7c 1261 277c 1264  .dHk...r.|.a'|.d
+000068d0: 2e17 0064 4e19 0064 0c6b 0290 0c72 b47c  ...dN..d.k...r.|
+000068e0: 1264 2d64 0085 0219 007d 1274 0164 8367  .d-d.....}.t.d.g
+000068f0: 0064 55a2 0164 0564 568d 0301 0074 2c7c  .dU..d.dV....t,|
+00006900: 1283 0190 0c72 a67c 0064 2d19 007d 016e  .....r.|.d-..}.n
+00006910: 0c7c 0064 4e19 007d 0164 2361 1c6e 187c  .|.dN..}.d#a.n.|
+00006920: 0064 4e19 007d 0174 0164 5267 0064 50a2  .dN..}.t.dRg.dP.
+00006930: 0164 518d 0201 006e 187c 0064 4e19 007d  .dQ....n.|.dN..}
+00006940: 0174 0164 5267 0064 50a2 0164 518d 0201  .t.dRg.dP..dQ...
+00006950: 007c 127d 0f90 0271 8e64 0053 0029 844e  .|.}...q.d.S.).N
+00006960: 7a27 5b23 5d20 496e 6974 6961 6c69 7a69  z'[#] Initializi
+00006970: 6e67 2060 5048 304d 4245 5260 2066 7261  ng `PH0MBER` fra
+00006980: 6d65 776f 726b 2e2e 2e72 2400 0000 7225  mework...r$...r%
+00006990: 0000 0029 0372 c600 0000 72c9 0000 0072  ...).r....r....r
+000069a0: ca00 0000 5429 0472 2800 0000 72a9 0000  ....T).r(...r...
+000069b0: 0072 a800 0000 72aa 0000 0029 057a 101b  .r....r....).z..
+000069c0: 5b31 3b34 393b 3932 6d3a 441b 5b30 6d7a  [1;49;92m:D.[0mz
+000069d0: 101b 5b31 3b34 393b 3936 6d3a 291b 5b30  ..[1;49;96m:).[0
+000069e0: 6d7a 101b 5b31 3b34 393b 3933 6d3a 7c1b  mz..[1;49;93m:|.
+000069f0: 5b30 6d7a 101b 5b31 3b34 393b 3931 6d3a  [0mz..[1;49;91m:
+00006a00: 281b 5b30 6d7a 101b 5b31 3b34 393b 3937  (.[0mz..[1;49;97
+00006a10: 6d3a 6f1b 5b30 6d72 0100 0000 75f3 0300  m:o.[0mr....u...
+00006a20: 0020 2020 201b 5b31 3b34 393b 3933 6d3e  .    .[1;49;93m>
+00006a30: 2045 7870 7265 7373 696f 6e73 2061 7265   Expressions are
+00006a40: 2075 7365 6420 746f 2073 686f 7720 7468   used to show th
+00006a50: 6520 7374 6174 7573 206f 6620 7468 6520  e status of the 
+00006a60: 7072 6576 696f 7573 2063 6f6d 6d61 6e64  previous command
+00006a70: 1b5b 306d 0a0a 2020 2020 1b5b 313b 3439  .[0m..    .[1;49
+00006a80: 3b39 336d 3e20 5379 6e74 6178 3a1b 5b30  ;93m> Syntax:.[0
+00006a90: 6d20 1b5b 313b 3439 3b39 376d 5b3c 7573  m .[1;49;97m[<us
+00006aa0: 6572 3e40 7068 306d 6265 725d e2b8 ba20  er>@ph0mber]... 
+00006ab0: 1b5b 313b 3439 3b39 366d 5b3c 6578 7072  .[1;49;96m[<expr
+00006ac0: 6573 7369 6f6e 3e5d 1b5b 313b 3439 3b39  ession>].[1;49;9
+00006ad0: 376d 2024 203c 636f 6d6d 616e 643e 1b5b  7m $ <command>.[
+00006ae0: 306d 0a0a 2020 2020 e294 8ce2 9480 e294  0m..    ........
+00006af0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00006b00: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00006b10: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00006b20: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00006b30: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00006b40: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00006b50: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00006b60: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00006b70: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00006b80: 80e2 9480 e294 80e2 9490 0a20 2020 207c  ...........    |
+00006b90: 2045 5850 5245 5353 494f 4e53 2020 207c   EXPRESSIONS   |
+00006ba0: 2044 4553 4352 4950 5449 4f4e 2020 2020   DESCRIPTION    
+00006bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006bc0: 2020 2020 7c0a 2020 2020 7c2d 2d2d 2d2d      |.    |-----
+00006bd0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00006be0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00006bf0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d7c  ---------------|
+00006c00: 0a20 2020 207c 201b 5b31 3b34 393b 3932  .    | .[1;49;92
+00006c10: 6d3a 441b 5b30 6d20 2020 2020 2020 2020  m:D.[0m         
+00006c20: 2020 207c 2045 7665 7279 7468 696e 6720     | Everything 
+00006c30: 6973 2066 696e 6520 2020 2020 2020 2020  is fine         
+00006c40: 2020 2020 2020 2020 7c0a 2020 2020 7c20          |.    | 
+00006c50: 1b5b 313b 3439 3b39 366d 3a29 1b5b 306d  .[1;49;96m:).[0m
+00006c60: 2020 2020 2020 2020 2020 2020 7c20 496e              | In
+00006c70: 666f 726d 6174 696f 6e20 6176 6169 6c61  formation availa
+00006c80: 626c 6520 2020 2020 2020 2020 2020 2020  ble             
+00006c90: 207c 0a20 2020 207c 201b 5b31 3b34 393b   |.    | .[1;49;
+00006ca0: 3933 6d3a 7c1b 5b30 6d20 2020 2020 2020  93m:|.[0m       
+00006cb0: 2020 2020 207c 2049 7427 7320 6120 7761       | It's a wa
+00006cc0: 726e 696e 6720 2872 656d 656d 6265 7229  rning (remember)
+00006cd0: 2020 2020 2020 2020 2020 7c0a 2020 2020            |.    
+00006ce0: 7c20 1b5b 313b 3439 3b39 316d 3a28 1b5b  | .[1;49;91m:(.[
+00006cf0: 306d 2020 2020 2020 2020 2020 2020 7c20  0m            | 
+00006d00: 536f 6d65 7468 696e 6720 7765 6e74 2077  Something went w
+00006d10: 726f 6e67 2020 2020 2020 2020 2020 2020  rong            
+00006d20: 2020 207c 0a20 2020 207c 201b 5b31 3b34     |.    | .[1;4
+00006d30: 393b 3937 6d3a 6f1b 5b30 6d20 2020 2020  9;97m:o.[0m     
+00006d40: 2020 2020 2020 207c 2053 6361 6e20 7265         | Scan re
+00006d50: 7375 6c74 7320 6176 6169 6c61 626c 6520  sults available 
+00006d60: 2020 2020 2020 2020 2020 2020 7c0a 2020              |.  
+00006d70: 2020 e294 94e2 9480 e294 80e2 9480 e294    ..............
+00006d80: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00006d90: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00006da0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00006db0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00006dc0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00006dd0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00006de0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00006df0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00006e00: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00006e10: 80e2 9498 7a0a 1b5b 313b 3439 3b39 366d  ....z..[1;49;96m
+00006e20: 72a1 0000 0072 3600 0000 e922 0000 00fa  r....r6...."....
+00006e30: 0125 e921 0000 00e9 2000 0000 723b 0000  .%.!.... ...r;..
+00006e40: 00fa 013a 7a02 2e2e 7a05 2530 3132 787a  ...:z...z.%012xz
+00006e50: 1a1b 5b31 3b34 393b 3936 6d33 2e30 2e32  ..[1;49;96m3.0.2
+00006e60: 2028 6265 7461 291b 5b30 6d7a 0c33 2e30   (beta).[0mz.3.0
+00006e70: 2e32 2028 6265 7461 2975 4201 0000 0a20  .2 (beta)uB.... 
+00006e80: 2020 20e2 948c e294 80e2 9480 e294 80e2     .............
+00006e90: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00006ea0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00006eb0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00006ec0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00006ed0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00006ee0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00006ef0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00006f00: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00006f10: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00006f20: 9480 e294 900a 2020 2020 7c20 5359 5354  ......    | SYST
+00006f30: 454d 2049 4e46 4f20 2020 7c20 4445 5343  EM INFO   | DESC
+00006f40: 5249 5054 494f 4e20 2020 2020 2020 2020  RIPTION         
+00006f50: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+00006f60: 0a20 2020 207c 2d2d 2d2d 2d2d 2d2d 2d2d  .    |----------
+00006f70: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00006f80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00006f90: 2d2d 2d2d 2d2d 2d2d 2d2d 7c0a 2020 2020  ----------|.    
+00006fa0: 7c20 1b5b 313b 3439 3b39 376d 5573 6572  | .[1;49;97mUser
+00006fb0: 1b5b 306d 2020 2020 2020 2020 2020 7c20  .[0m          | 
+00006fc0: 7a27 207c 0a20 2020 207c 201b 5b31 3b34  z' |.    | .[1;4
+00006fd0: 393b 3937 6d48 6f73 746e 616d 651b 5b30  9;97mHostname.[0
+00006fe0: 6d20 2020 2020 207c 207a 2720 7c0a 2020  m      | z' |.  
+00006ff0: 2020 7c20 1b5b 313b 3439 3b39 376d 4f53    | .[1;49;97mOS
+00007000: 1b5b 306d 2020 2020 2020 2020 2020 2020  .[0m            
+00007010: 7c20 7a27 207c 0a20 2020 207c 201b 5b31  | z' |.    | .[1
+00007020: 3b34 393b 3937 6d41 7263 6869 7465 6374  ;49;97mArchitect
+00007030: 7572 651b 5b30 6d20 207c 207a 2720 7c0a  ure.[0m  | z' |.
+00007040: 2020 2020 7c20 1b5b 313b 3439 3b39 376d      | .[1;49;97m
+00007050: 5379 7374 656d 204d 4143 1b5b 306d 2020  System MAC.[0m  
+00007060: 2020 7c20 7a62 207c 0a20 2020 207c 2d2d    | zb |.    |--
+00007070: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00007080: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00007090: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000070a0: 2d2d 7c0a 2020 2020 7c20 1b5b 313b 3439  --|.    | .[1;49
+000070b0: 3b39 376d 5241 4d20 5573 6167 651b 5b30  ;97mRAM Usage.[0
+000070c0: 6d20 2020 2020 7c20 7a27 207c 0a20 2020  m     | z' |.   
+000070d0: 207c 201b 5b31 3b34 393b 3937 6d43 5055   | .[1;49;97mCPU
+000070e0: 2055 7361 6765 1b5b 306d 2020 2020 207c   Usage.[0m     |
+000070f0: 207a 2720 7c0a 2020 2020 7c20 1b5b 313b   z' |.    | .[1;
+00007100: 3439 3b39 376d 4469 736b 2055 7361 6765  49;97mDisk Usage
+00007110: 1b5b 306d 2020 2020 7c20 7543 0200 0020  .[0m    | uC... 
+00007120: 7c0a 2020 2020 e294 94e2 9480 e294 80e2  |.    ..........
+00007130: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00007140: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00007150: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00007160: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00007170: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00007180: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00007190: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+000071a0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+000071b0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+000071c0: 9480 e294 80e2 9498 0a0a 2020 2020 e294  ..........    ..
+000071d0: 8ce2 9480 e294 80e2 9480 e294 80e2 9480  ................
+000071e0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+000071f0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00007200: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00007210: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00007220: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00007230: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00007240: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00007250: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00007260: 80e2 9480 e294 80e2 9480 e294 80e2 9490  ................
+00007270: 0a20 2020 207c 2046 5241 4d45 574f 524b  .    | FRAMEWORK
+00007280: 2049 4e46 4f7c 2044 4553 4352 4950 5449   INFO| DESCRIPTI
+00007290: 4f4e 2020 2020 2020 2020 2020 2020 2020  ON              
+000072a0: 2020 2020 2020 2020 2020 7c0a 2020 2020            |.    
+000072b0: 7c2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  |---------------
+000072c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000072d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000072e0: 2d2d 2d2d 2d7c 0a20 2020 207c 201b 5b31  -----|.    | .[1
+000072f0: 3b34 393b 3937 6d4e 616d 651b 5b30 6d20  ;49;97mName.[0m 
+00007300: 2020 2020 2020 2020 207c 201b 5b31 3b34           | .[1;4
+00007310: 393b 3936 6d50 4830 4d42 4552 1b5b 306d  9;96mPH0MBER.[0m
+00007320: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007330: 2020 2020 2020 2020 2020 2020 7c0a 2020              |.  
+00007340: 2020 7c20 1b5b 313b 3439 3b39 376d 5665    | .[1;49;97mVe
+00007350: 7273 696f 6e1b 5b30 6d20 2020 2020 2020  rsion.[0m       
+00007360: 7c20 75b3 0100 0020 7c0a 2020 2020 7c20  | u.... |.    | 
+00007370: 1b5b 313b 3439 3b39 376d 5479 7065 1b5b  .[1;49;97mType.[
+00007380: 306d 2020 2020 2020 2020 2020 7c20 1b5b  0m          | .[
+00007390: 313b 3439 3b39 366d 4f53 494e 5420 4672  1;49;96mOSINT Fr
+000073a0: 616d 6577 6f72 6b1b 5b30 6d20 2020 2020  amework.[0m     
+000073b0: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+000073c0: 0a20 2020 207c 201b 5b31 3b34 393b 3937  .    | .[1;49;97
+000073d0: 6d44 6576 656c 6f70 6572 1b5b 306d 2020  mDeveloper.[0m  
+000073e0: 2020 207c 201b 5b31 3b34 393b 3936 6d73     | .[1;49;96ms
+000073f0: 3431 7234 6a1b 5b30 6d20 2020 2020 2020  41r4j.[0m       
+00007400: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007410: 2020 2020 2020 7c0a 2020 2020 7c20 1b5b        |.    | .[
+00007420: 313b 3439 3b39 376d 4769 7468 7562 1b5b  1;49;97mGithub.[
+00007430: 306d 2020 2020 2020 2020 7c20 1b5b 313b  0m        | .[1;
+00007440: 3439 3b39 366d 6874 7470 733a 2f2f 6769  49;96mhttps://gi
+00007450: 7468 7562 2e63 6f6d 2f73 3431 7234 6a2f  thub.com/s41r4j/
+00007460: 7068 6f6d 6265 721b 5b30 6d20 207c 0a20  phomber.[0m  |. 
+00007470: 2020 20e2 9494 e294 80e2 9480 e294 80e2     .............
+00007480: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00007490: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+000074a0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+000074b0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+000074c0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+000074d0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+000074e0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+000074f0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00007500: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00007510: 9480 e294 980a 2020 2020 753b 0800 000a  ......    u;....
+00007520: 2020 2020 e294 8ce2 9480 e294 80e2 9480      ............
+00007530: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00007540: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00007550: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00007560: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00007570: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00007580: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00007590: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+000075a0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+000075b0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+000075c0: e294 80e2 9490 0a20 2020 207c 2043 4f4d  .......    | COM
+000075d0: 4d41 4e44 5320 2020 2020 207c 2044 4553  MANDS      | DES
+000075e0: 4352 4950 5449 4f4e 2020 2020 2020 2020  CRIPTION        
+000075f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007600: 7c0a 2020 2020 7c2d 2d2d 2d2d 2d2d 2d2d  |.    |---------
+00007610: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00007620: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00007630: 2d2d 2d2d 2d2d 2d2d 2d2d 2d7c 0a20 2020  -----------|.   
+00007640: 207c 2020 2020 2020 2020 2020 2020 2020   |              
+00007650: 2020 3c42 6173 6963 2043 6f6d 6d61 6e64    <Basic Command
+00007660: 733e 2020 2020 2020 2020 2020 2020 2020  s>              
+00007670: 2020 2020 2020 7c0a 2020 2020 7c2d 2d2d        |.    |---
+00007680: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00007690: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000076a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000076b0: 2d7c 0a20 2020 207c 201b 5b31 3b34 393b  -|.    | .[1;49;
+000076c0: 3937 6d68 656c 701b 5b30 6d20 2020 2020  97mhelp.[0m     
+000076d0: 2020 2020 207c 2044 6973 706c 6179 2074       | Display t
+000076e0: 6869 7320 6865 6c70 206d 656e 7520 2020  his help menu   
+000076f0: 2020 2020 2020 2020 2020 7c20 0a20 2020            | .   
+00007700: 207c 201b 5b31 3b34 393b 3937 6d65 7869   | .[1;49;97mexi
+00007710: 742f 7175 6974 1b5b 306d 2020 2020 207c  t/quit.[0m     |
+00007720: 2045 7869 7420 7468 6520 6672 616d 6577   Exit the framew
+00007730: 6f72 6b20 2020 2020 2020 2020 2020 2020  ork             
+00007740: 2020 2020 7c0a 2020 2020 7c20 1b5b 313b      |.    | .[1;
+00007750: 3439 3b39 376d 646f 726b 1b5b 306d 2020  49;97mdork.[0m  
+00007760: 2020 2020 2020 2020 7c20 5368 6f77 2061          | Show a
+00007770: 2072 616e 646f 6d20 676f 6f67 6c65 2064   random google d
+00007780: 6f72 6b20 7175 6572 7920 2a20 207c 2020  ork query *  |  
+00007790: 0a20 2020 207c 201b 5b31 3b34 393b 3937  .    | .[1;49;97
+000077a0: 6d65 7870 1b5b 306d 2020 2020 2020 2020  mexp.[0m        
+000077b0: 2020 207c 2053 686f 7720 696e 666f 2061     | Show info a
+000077c0: 626f 7574 2061 6c6c 2061 7661 696c 6162  bout all availab
+000077d0: 6c65 2020 2020 2020 7c20 2020 2020 2020  le      |       
+000077e0: 0a20 2020 207c 2020 2020 2020 2020 2020  .    |          
+000077f0: 2020 2020 207c 2065 7870 7265 7373 696f       | expressio
+00007800: 6e73 2020 2020 2020 2020 2020 2020 2020  ns              
+00007810: 2020 2020 2020 2020 2020 7c0a 2020 2020            |.    
+00007820: 7c20 1b5b 313b 3439 3b39 376d 6368 6563  | .[1;49;97mchec
+00007830: 6b1b 5b30 6d20 2020 2020 2020 2020 7c20  k.[0m         | 
+00007840: 4368 6563 6b20 696e 7465 726e 6574 2063  Check internet c
+00007850: 6f6e 6e65 6374 696f 6e20 2020 2020 2020  onnection       
+00007860: 2020 207c 0a20 2020 207c 201b 5b31 3b34     |.    | .[1;4
+00007870: 393b 3937 6d63 6c65 6172 1b5b 306d 2020  9;97mclear.[0m  
+00007880: 2020 2020 2020 207c 2043 6c65 6172 2073         | Clear s
+00007890: 6372 6565 6e20 2020 2020 2020 2020 2020  creen           
+000078a0: 2020 2020 2020 2020 2020 2020 7c0a 2020              |.  
+000078b0: 2020 7c20 1b5b 313b 3439 3b39 376d 7361    | .[1;49;97msa
+000078c0: 7665 1b5b 306d 2020 2020 2020 2020 2020  ve.[0m          
+000078d0: 7c20 5361 7665 206f 7574 7075 7420 6f66  | Save output of
+000078e0: 2070 7265 7669 6f75 7320 7363 616e 6e65   previous scanne
+000078f0: 7220 2020 207c 0a20 2020 207c 2020 2020  r    |.    |    
+00007900: 2020 2020 2020 2020 2020 207c 2063 6f6d             | com
+00007910: 6d61 6e64 2069 6e20 6120 6669 6c65 2020  mand in a file  
+00007920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007930: 7c0a 2020 2020 7c20 1b5b 313b 3439 3b39  |.    | .[1;49;9
+00007940: 376d 7368 656c 6c20 3c63 6d64 3e1b 5b30  7mshell <cmd>.[0
+00007950: 6d20 2020 7c20 4578 6563 7574 6520 6e61  m   | Execute na
+00007960: 7469 7665 2073 6865 6c6c 2f63 6d64 2063  tive shell/cmd c
+00007970: 6f6d 6d61 6e64 7320 207c 0a20 2020 207c  ommands  |.    |
+00007980: 201b 5b31 3b34 393b 3937 6d69 6e66 6f1b   .[1;49;97minfo.
+00007990: 5b30 6d20 2020 2020 2020 2020 207c 2053  [0m          | S
+000079a0: 686f 7720 696e 666f 2061 626f 7574 2066  how info about f
+000079b0: 7261 6d65 776f 726b 2026 2073 7973 7465  ramework & syste
+000079c0: 6d20 7c0a 2020 2020 7c20 1b5b 313b 3439  m |.    | .[1;49
+000079d0: 3b39 376d 6368 616e 6765 1b5b 306d 2020  ;97mchange.[0m  
+000079e0: 2020 2020 2020 7c20 4368 616e 6765 2075        | Change u
+000079f0: 7365 7220 636f 6d6d 616e 6420 696e 7075  ser command inpu
+00007a00: 7420 636f 6c6f 7220 2020 207c 0a20 2020  t color    |.   
+00007a10: 207c 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   |--------------
+00007a20: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00007a30: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00007a40: 2d2d 2d2d 2d2d 7c0a 2020 2020 7c20 2020  ------|.    |   
+00007a50: 2020 2020 2020 2020 2020 2020 2020 3c53                <S
+00007a60: 6361 6e6e 6572 2043 6f6d 6d61 6e64 733e  canner Commands>
+00007a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007a80: 207c 0a20 2020 207c 2d2d 2d2d 2d2d 2d2d   |.    |--------
+00007a90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00007aa0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00007ab0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 7c0a 2020  ------------|.  
+00007ac0: 2020 7c20 1b5b 313b 3439 3b39 376d 6e75    | .[1;49;97mnu
+00007ad0: 6d62 6572 1b5b 306d 2020 2020 2020 2020  mber.[0m        
+00007ae0: 7c20 5265 7665 7273 6520 7068 6f6e 6520  | Reverse phone 
+00007af0: 6e75 6d62 6572 206c 6f6f 6b75 7020 2a20  number lookup * 
+00007b00: 2020 2020 207c 0a20 2020 207c 201b 5b31       |.    | .[1
+00007b10: 3b34 393b 3937 6d69 701b 5b30 6d20 2020  ;49;97mip.[0m   
+00007b20: 2020 2020 2020 2020 207c 2052 6576 6572           | Rever
+00007b30: 7365 2069 7020 6164 6472 6573 7320 6c6f  se ip address lo
+00007b40: 6f6b 7570 202a 2020 2020 2020 2020 7c0a  okup *        |.
+00007b50: 2020 2020 7c20 1b5b 313b 3439 3b39 376d      | .[1;49;97m
+00007b60: 6d61 631b 5b30 6d20 2020 2020 2020 2020  mac.[0m         
+00007b70: 2020 7c20 5265 7665 7273 6520 6d61 6320    | Reverse mac 
+00007b80: 6164 6472 6573 7320 6c6f 6f6b 7570 2020  address lookup  
+00007b90: 2020 2020 2020 207c 0a20 2020 207c 201b         |.    | .
+00007ba0: 5b31 3b34 393b 3937 6d77 686f 6973 1b5b  [1;49;97mwhois.[
+00007bb0: 306d 2020 2020 2020 2020 207c 2052 6576  0m         | Rev
+00007bc0: 6572 7365 2077 686f 6973 206c 6f6f 6b75  erse whois looku
+00007bd0: 7020 2a20 2020 2020 2020 2020 2020 2020  p *             
+00007be0: 7c0a 2020 2020 7c20 1b5b 313b 3439 3b39  |.    | .[1;49;9
+00007bf0: 376d 646e 731b 5b30 6d20 2020 2020 2020  7mdns.[0m       
+00007c00: 2020 2020 7c20 5265 7665 7273 6520 6f72      | Reverse or
+00007c10: 206e 6f72 6d61 6c20 444e 5320 6c6f 6f6b   normal DNS look
+00007c20: 7570 2020 2020 2020 207c 0a20 2020 207c  up       |.    |
+00007c30: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00007c40: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00007c50: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00007c60: 2d2d 2d2d 7c0a 2020 2020 7c20 1b5b 313b  ----|.    | .[1;
+00007c70: 3439 3b39 316d 4d4f 5245 2053 4341 4e4e  49;91mMORE SCANN
+00007c80: 4552 5320 434f 4d49 4e47 2053 4f4f 4e2c  ERS COMING SOON,
+00007c90: 2054 4849 5320 4953 2041 2042 4554 4120   THIS IS A BETA 
+00007ca0: 5645 521b 5b30 6d20 2020 2020 207c 0a20  VER.[0m      |. 
+00007cb0: 2020 20e2 9494 e294 80e2 9480 e294 80e2     .............
+00007cc0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00007cd0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00007ce0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00007cf0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00007d00: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00007d10: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00007d20: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00007d30: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00007d40: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00007d50: 9480 e294 980a 2020 2020 2905 7a4e 5479  ......    ).zNTy
+00007d60: 7065 2060 1b5b 373b 3439 3b39 336d 6865  pe `.[7;49;93mhe
+00007d70: 6c70 203c 636f 6d6d 616e 643e 1b5b 306d  lp <command>.[0m
+00007d80: 1b5b 313b 3439 3b39 336d 6020 746f 2073  .[1;49;93m` to s
+00007d90: 6565 206d 6f72 6520 696e 666f 2061 626f  ee more info abo
+00007da0: 7574 2061 2063 6f6d 6d61 6e64 7a3f 5573  ut a commandz?Us
+00007db0: 6520 601b 5b37 3b34 393b 3933 6d54 6162  e `.[7;49;93mTab
+00007dc0: 1b5b 306d 1b5b 313b 3439 3b39 336d 6020  .[0m.[1;49;93m` 
+00007dd0: 6b65 7920 746f 2061 7574 6f2d 636f 6d70  key to auto-comp
+00007de0: 6c65 7465 2063 6f6d 6d61 6e64 737a 5d54  lete commandsz]T
+00007df0: 7279 2073 696c 656e 7420 6d6f 6465 2062  ry silent mode b
+00007e00: 7920 7573 696e 6720 601b 5b37 3b34 393b  y using `.[7;49;
+00007e10: 3933 6d2d 731b 5b30 6d1b 5b31 3b34 393b  93m-s.[0m.[1;49;
+00007e20: 3933 6d60 2f60 1b5b 373b 3439 3b39 336d  93m`/`.[7;49;93m
+00007e30: 2d2d 7369 6c65 6e74 1b5b 306d 1b5b 313b  --silent.[0m.[1;
+00007e40: 3439 3b39 336d 6020 666c 6167 7a39 596f  49;93m` flagz9Yo
+00007e50: 7520 6361 6e20 616c 736f 2075 7365 2060  u can also use `
+00007e60: 1b5b 373b 3439 3b39 336d 4374 726c 2b43  .[7;49;93mCtrl+C
+00007e70: 1b5b 306d 1b5b 313b 3439 3b39 336d 6020  .[0m.[1;49;93m` 
+00007e80: 746f 2065 7869 747a 4e44 6573 6372 6970  to exitzNDescrip
+00007e90: 7469 6f6e 7320 656e 6469 6e67 2077 6974  tions ending wit
+00007ea0: 6820 601b 5b37 3b34 393b 3933 6d2a 1b5b  h `.[7;49;93m*.[
+00007eb0: 306d 1b5b 313b 3439 3b39 336d 6020 6e65  0m.[1;49;93m` ne
+00007ec0: 6564 7320 696e 7465 726e 6574 2063 6f6e  eds internet con
+00007ed0: 6e65 6374 696f 6e72 1300 0000 7a0d 7461  nectionr....z.ta
+00007ee0: 623a 2063 6f6d 706c 6574 657a 0a1b 5b31  b: completez..[1
+00007ef0: 3b34 393b 3930 6d7a 0a1b 5b31 3b34 393b  ;49;90mz..[1;49;
+00007f00: 3937 6d7a 060a 1b5b 306d 5b75 0e00 0000  97mz...[0m[u....
+00007f10: 4070 6830 6d62 6572 5de2 b8ba 205b 7a04  @ph0mber]... [z.
+00007f20: 5d20 2420 2902 72ac 0000 0072 aa00 0000  ] $ ).r....r....
+00007f30: 720a 0000 007a 101b 5b31 3b34 393b 3933  r....z..[1;49;93
+00007f40: 6d20 2020 203e 20e9 0400 0000 fa01 23e9  m    > .......#.
+00007f50: 0500 0000 612b 0100 0020 201b 5b31 3b34  ....a+...  .[1;4
+00007f60: 393b 3933 6d5b 2b5d 2043 6f6d 6d61 6e64  9;93m[+] Command
+00007f70: 2049 6e66 6f3a 201b 5b31 3b34 393b 3933   Info: .[1;49;93
+00007f80: 6d68 656c 700a 0a20 2020 201b 5b31 3b34  mhelp..    .[1;4
+00007f90: 393b 3932 6d3e 2044 4553 4352 4950 5449  9;92m> DESCRIPTI
+00007fa0: 4f4e 3a20 1b5b 313b 3439 3b39 376d 5768  ON: .[1;49;97mWh
+00007fb0: 656e 2079 6f75 2074 7970 6520 6068 656c  en you type `hel
+00007fc0: 7060 2c20 7468 6520 6865 6c70 206d 656e  p`, the help men
+00007fd0: 7520 7769 6c6c 2062 6520 6469 7370 6c61  u will be displa
+00007fe0: 7965 640a 2020 2020 1b5b 313b 3439 3b39  yed.    .[1;49;9
+00007ff0: 326d 3e20 5359 4e54 4158 3a20 1b5b 313b  2m> SYNTAX: .[1;
+00008000: 3439 3b39 376d 6865 6c70 201b 5b31 3b34  49;97mhelp .[1;4
+00008010: 393b 3932 6d4f 5220 1b5b 313b 3439 3b39  9;92mOR .[1;49;9
+00008020: 376d 6865 6c70 203c 636f 6d6d 616e 643e  7mhelp <command>
+00008030: 0a20 2020 201b 5b31 3b34 393b 3932 6d3e  .    .[1;49;92m>
+00008040: 2045 5841 4d50 4c45 3a20 1b5b 313b 3439   EXAMPLE: .[1;49
+00008050: 3b39 376d 6865 6c70 201b 5b31 3b34 393b  ;97mhelp .[1;49;
+00008060: 3932 6d4f 5220 1b5b 313b 3439 3b39 376d  92mOR .[1;49;97m
+00008070: 6865 6c70 206e 756d 6265 720a 2020 2020  help number.    
+00008080: 1b5b 306d 7208 0000 0072 0f00 0000 7aee  .[0mr....r....z.
+00008090: 2020 1b5b 313b 3439 3b39 336d 5b2b 5d20    .[1;49;93m[+] 
+000080a0: 436f 6d6d 616e 6420 496e 666f 3a20 1b5b  Command Info: .[
+000080b0: 313b 3439 3b39 336d 6578 6974 2f1b 5b31  1;49;93mexit/.[1
+000080c0: 3b34 393b 3933 6d71 7569 740a 0a20 2020  ;49;93mquit..   
+000080d0: 201b 5b31 3b34 393b 3932 6d3e 2044 4553   .[1;49;92m> DES
+000080e0: 4352 4950 5449 4f4e 3a20 1b5b 313b 3439  CRIPTION: .[1;49
+000080f0: 3b39 376d 5768 656e 2079 6f75 2074 7970  ;97mWhen you typ
+00008100: 6520 6065 7869 7460 206f 7220 6071 7569  e `exit` or `qui
+00008110: 7460 2c20 7468 6520 7072 6f67 7261 6d20  t`, the program 
+00008120: 7769 6c6c 2062 6520 7465 726d 696e 6174  will be terminat
+00008130: 6564 0a20 2020 201b 5b31 3b34 393b 3932  ed.    .[1;49;92
+00008140: 6d3e 2053 594e 5441 583a 201b 5b31 3b34  m> SYNTAX: .[1;4
+00008150: 393b 3937 6d65 7869 7420 1b5b 313b 3439  9;97mexit .[1;49
+00008160: 3b39 326d 4f52 201b 5b31 3b34 393b 3937  ;92mOR .[1;49;97
+00008170: 6d71 7569 740a 2020 2020 1b5b 306d 7206  mquit.    .[0mr.
+00008180: 0000 007a c720 201b 5b31 3b34 393b 3933  ...z.  .[1;49;93
+00008190: 6d5b 2b5d 2043 6f6d 6d61 6e64 2049 6e66  m[+] Command Inf
+000081a0: 6f3a 201b 5b31 3b34 393b 3933 6d64 6f72  o: .[1;49;93mdor
+000081b0: 6b0a 0a20 2020 201b 5b31 3b34 393b 3932  k..    .[1;49;92
+000081c0: 6d3e 2044 4553 4352 4950 5449 4f4e 3a20  m> DESCRIPTION: 
+000081d0: 1b5b 313b 3439 3b39 376d 5768 656e 2079  .[1;49;97mWhen y
+000081e0: 6f75 2074 7970 6520 6064 6f72 6b60 2c20  ou type `dork`, 
+000081f0: 6120 7261 6e64 6f6d 2067 6f6f 676c 6520  a random google 
+00008200: 646f 726b 2071 7565 7279 2077 696c 6c20  dork query will 
+00008210: 6265 2064 6973 706c 6179 6564 0a20 2020  be displayed.   
+00008220: 201b 5b31 3b34 393b 3932 6d3e 2053 594e   .[1;49;92m> SYN
+00008230: 5441 583a 201b 5b31 3b34 393b 3937 6d64  TAX: .[1;49;97md
+00008240: 6f72 6b0a 2020 2020 1b5b 306d 7209 0000  ork.    .[0mr...
+00008250: 007a ce20 201b 5b31 3b34 393b 3933 6d5b  .z.  .[1;49;93m[
+00008260: 2b5d 2043 6f6d 6d61 6e64 2049 6e66 6f3a  +] Command Info:
+00008270: 201b 5b31 3b34 393b 3933 6d65 7870 0a0a   .[1;49;93mexp..
+00008280: 2020 2020 1b5b 313b 3439 3b39 326d 3e20      .[1;49;92m> 
+00008290: 4445 5343 5249 5054 494f 4e3a 201b 5b31  DESCRIPTION: .[1
+000082a0: 3b34 393b 3937 6d57 6865 6e20 796f 7520  ;49;97mWhen you 
+000082b0: 7479 7065 2060 6578 7060 2c20 696e 666f  type `exp`, info
+000082c0: 2061 626f 7574 2061 6c6c 2061 7661 696c   about all avail
+000082d0: 6162 6c65 2065 7870 7265 7373 696f 6e73  able expressions
+000082e0: 2077 696c 6c20 6265 2064 6973 706c 6179   will be display
+000082f0: 6564 0a20 2020 201b 5b31 3b34 393b 3932  ed.    .[1;49;92
+00008300: 6d3e 2053 594e 5441 583a 201b 5b31 3b34  m> SYNTAX: .[1;4
+00008310: 393b 3937 6d65 7870 0a20 2020 201b 5b30  9;97mexp.    .[0
+00008320: 6d72 0400 0000 7ad0 2020 1b5b 313b 3439  mr....z.  .[1;49
+00008330: 3b39 336d 5b2b 5d20 436f 6d6d 616e 6420  ;93m[+] Command 
+00008340: 496e 666f 3a20 1b5b 313b 3439 3b39 336d  Info: .[1;49;93m
+00008350: 6368 6563 6b0a 0a20 2020 201b 5b31 3b34  check..    .[1;4
+00008360: 393b 3932 6d3e 2044 4553 4352 4950 5449  9;92m> DESCRIPTI
+00008370: 4f4e 3a20 1b5b 313b 3439 3b39 376d 5768  ON: .[1;49;97mWh
+00008380: 656e 2079 6f75 2074 7970 6520 6063 6865  en you type `che
+00008390: 636b 602c 2069 7420 7769 6c6c 2063 6865  ck`, it will che
+000083a0: 636b 2066 6f72 2069 6e74 6572 6e65 7420  ck for internet 
+000083b0: 636f 6e6e 6563 7469 6f6e 2061 7661 696c  connection avail
+000083c0: 6162 696c 6974 790a 2020 2020 1b5b 313b  ability.    .[1;
+000083d0: 3439 3b39 326d 3e20 5359 4e54 4158 3a20  49;92m> SYNTAX: 
+000083e0: 1b5b 313b 3439 3b39 376d 6368 6563 6b0a  .[1;49;97mcheck.
+000083f0: 2020 2020 1b5b 306d 7205 0000 007a b620      .[0mr....z. 
+00008400: 201b 5b31 3b34 393b 3933 6d5b 2b5d 2043   .[1;49;93m[+] C
+00008410: 6f6d 6d61 6e64 2049 6e66 6f3a 201b 5b31  ommand Info: .[1
+00008420: 3b34 393b 3933 6d63 6c65 6172 0a0a 2020  ;49;93mclear..  
+00008430: 2020 1b5b 313b 3439 3b39 326d 3e20 4445    .[1;49;92m> DE
+00008440: 5343 5249 5054 494f 4e3a 201b 5b31 3b34  SCRIPTION: .[1;4
+00008450: 393b 3937 6d57 6865 6e20 796f 7520 7479  9;97mWhen you ty
+00008460: 7065 2060 636c 6561 7260 2c20 6974 2077  pe `clear`, it w
+00008470: 696c 6c20 636c 6561 7220 7468 6520 7363  ill clear the sc
+00008480: 7265 656e 0a20 2020 201b 5b31 3b34 393b  reen.    .[1;49;
+00008490: 3932 6d3e 2053 594e 5441 583a 201b 5b31  92m> SYNTAX: .[1
+000084a0: 3b34 393b 3937 6d63 6c65 6172 0a20 2020  ;49;97mclear.   
+000084b0: 201b 5b30 6d72 1000 0000 7aee 2020 1b5b   .[0mr....z.  .[
+000084c0: 313b 3439 3b39 336d 5b2b 5d20 436f 6d6d  1;49;93m[+] Comm
+000084d0: 616e 6420 496e 666f 3a20 1b5b 313b 3439  and Info: .[1;49
+000084e0: 3b39 336d 7361 7665 0a0a 2020 2020 1b5b  ;93msave..    .[
+000084f0: 313b 3439 3b39 326d 3e20 4445 5343 5249  1;49;92m> DESCRI
+00008500: 5054 494f 4e3a 201b 5b31 3b34 393b 3937  PTION: .[1;49;97
+00008510: 6d57 6865 6e20 796f 7520 7479 7065 2060  mWhen you type `
+00008520: 7361 7665 602c 2069 7420 7769 6c6c 2073  save`, it will s
+00008530: 6176 6520 7468 6520 6f75 7470 7574 206f  ave the output o
+00008540: 6620 7072 6576 696f 7573 2063 6f6d 6d61  f previous comma
+00008550: 6e64 0a20 2020 201b 5b31 3b34 393b 3932  nd.    .[1;49;92
+00008560: 6d3e 2053 594e 5441 583a 201b 5b31 3b34  m> SYNTAX: .[1;4
+00008570: 393b 3937 6d73 6176 650a 2020 2020 1b5b  9;97msave.    .[
+00008580: 313b 3439 3b39 326d 3e20 4558 414d 504c  1;49;92m> EXAMPL
+00008590: 453a 201b 5b31 3b34 393b 3937 6d73 6176  E: .[1;49;97msav
+000085a0: 650a 2020 2020 1b5b 306d 7211 0000 0061  e.    .[0mr....a
+000085b0: 0101 0000 2020 1b5b 313b 3439 3b39 336d  ....  .[1;49;93m
+000085c0: 5b2b 5d20 436f 6d6d 616e 6420 496e 666f  [+] Command Info
+000085d0: 3a20 1b5b 313b 3439 3b39 336d 7368 656c  : .[1;49;93mshel
+000085e0: 6c0a 0a20 2020 201b 5b31 3b34 393b 3932  l..    .[1;49;92
+000085f0: 6d3e 2044 4553 4352 4950 5449 4f4e 3a20  m> DESCRIPTION: 
+00008600: 1b5b 313b 3439 3b39 376d 5768 656e 2079  .[1;49;97mWhen y
+00008610: 6f75 2074 7970 6520 6073 6865 6c6c 602c  ou type `shell`,
+00008620: 2069 7420 7769 6c6c 2065 7865 6375 7465   it will execute
+00008630: 2067 6976 656e 2063 6f6d 6d61 6e64 2069   given command i
+00008640: 6e20 6e61 7469 7665 2073 6865 6c6c 2f63  n native shell/c
+00008650: 6d64 0a20 2020 201b 5b31 3b34 393b 3932  md.    .[1;49;92
+00008660: 6d3e 2053 594e 5441 583a 201b 5b31 3b34  m> SYNTAX: .[1;4
+00008670: 393b 3937 6d73 6865 6c6c 203c 636d 643e  9;97mshell <cmd>
+00008680: 0a20 2020 201b 5b31 3b34 393b 3932 6d3e  .    .[1;49;92m>
+00008690: 2045 5841 4d50 4c45 3a20 1b5b 313b 3439   EXAMPLE: .[1;49
+000086a0: 3b39 376d 7368 656c 6c20 6c73 0a20 2020  ;97mshell ls.   
+000086b0: 201b 5b30 6d72 0b00 0000 7ac5 2020 1b5b   .[0mr....z.  .[
+000086c0: 313b 3439 3b39 336d 5b2b 5d20 436f 6d6d  1;49;93m[+] Comm
+000086d0: 616e 6420 496e 666f 3a20 1b5b 313b 3439  and Info: .[1;49
+000086e0: 3b39 336d 696e 666f 0a0a 2020 2020 1b5b  ;93minfo..    .[
+000086f0: 313b 3439 3b39 326d 3e20 4445 5343 5249  1;49;92m> DESCRI
+00008700: 5054 494f 4e3a 201b 5b31 3b34 393b 3937  PTION: .[1;49;97
+00008710: 6d57 6865 6e20 796f 7520 7479 7065 2060  mWhen you type `
+00008720: 696e 666f 602c 2069 7420 7769 6c6c 2073  info`, it will s
+00008730: 686f 7720 696e 666f 2061 626f 7574 2066  how info about f
+00008740: 7261 6d65 776f 726b 2026 2073 7973 7465  ramework & syste
+00008750: 6d0a 2020 2020 1b5b 313b 3439 3b39 326d  m.    .[1;49;92m
+00008760: 3e20 5359 4e54 4158 3a20 1b5b 313b 3439  > SYNTAX: .[1;49
+00008770: 3b39 376d 696e 666f 0a20 2020 201b 5b30  ;97minfo.    .[0
+00008780: 6d72 0300 0000 618a 0100 0020 201b 5b31  mr....a....  .[1
+00008790: 3b34 393b 3933 6d5b 2b5d 2043 6f6d 6d61  ;49;93m[+] Comma
+000087a0: 6e64 2049 6e66 6f3a 201b 5b31 3b34 393b  nd Info: .[1;49;
+000087b0: 3933 6d63 6861 6e67 650a 0a20 2020 201b  93mchange..    .
+000087c0: 5b31 3b34 393b 3932 6d3e 2044 4553 4352  [1;49;92m> DESCR
+000087d0: 4950 5449 4f4e 3a20 1b5b 313b 3439 3b39  IPTION: .[1;49;9
+000087e0: 376d 5768 656e 2079 6f75 2074 7970 6520  7mWhen you type 
+000087f0: 6063 6861 6e67 6560 2c20 6974 2077 696c  `change`, it wil
+00008800: 6c20 6368 616e 6765 2075 7365 7220 636f  l change user co
+00008810: 6d6d 616e 6420 696e 7075 7420 636f 6c6f  mmand input colo
+00008820: 720a 2020 2020 1b5b 313b 3439 3b39 326d  r.    .[1;49;92m
+00008830: 3e20 4f50 5449 4f4e 533a 201b 5b31 3b34  > OPTIONS: .[1;4
+00008840: 393b 3937 6d30 202d 3e20 1b5b 313b 3439  9;97m0 -> .[1;49
+00008850: 3b39 306d 426c 6163 6b0a 2020 2020 2020  ;90mBlack.      
+00008860: 2020 2020 2020 2020 201b 5b31 3b34 393b           .[1;49;
+00008870: 3937 6d31 202d 3e20 5768 6974 6520 2020  97m1 -> White   
+00008880: 2020 2020 200a 2020 2020 1b5b 313b 3439       .    .[1;49
+00008890: 3b39 326d 3e20 4465 6661 756c 743a 201b  ;92m> Default: .
+000088a0: 5b31 3b34 393b 3937 6d31 0a20 2020 201b  [1;49;97m1.    .
+000088b0: 5b31 3b34 393b 3932 6d3e 2053 594e 5441  [1;49;92m> SYNTA
+000088c0: 583a 201b 5b31 3b34 393b 3937 6d63 6861  X: .[1;49;97mcha
+000088d0: 6e67 6520 3c63 6f6c 6f72 5f63 6f64 653e  nge <color_code>
+000088e0: 0a20 2020 201b 5b31 3b34 393b 3932 6d3e  .    .[1;49;92m>
+000088f0: 2045 5841 4d50 4c45 3a20 1b5b 313b 3439   EXAMPLE: .[1;49
+00008900: 3b39 376d 6368 616e 6765 2030 0a20 2020  ;97mchange 0.   
+00008910: 201b 5b30 6d72 0e00 0000 613f 0100 0020   .[0mr....a?... 
+00008920: 201b 5b31 3b34 393b 3933 6d5b 2b5d 2043   .[1;49;93m[+] C
+00008930: 6f6d 6d61 6e64 2049 6e66 6f3a 201b 5b31  ommand Info: .[1
+00008940: 3b34 393b 3933 6d6e 756d 6265 720a 0a20  ;49;93mnumber.. 
+00008950: 2020 201b 5b31 3b34 393b 3932 6d3e 2044     .[1;49;92m> D
+00008960: 4553 4352 4950 5449 4f4e 3a20 1b5b 313b  ESCRIPTION: .[1;
+00008970: 3439 3b39 376d 5768 656e 2079 6f75 2074  49;97mWhen you t
+00008980: 7970 6520 606e 756d 6265 7260 2c20 6974  ype `number`, it
+00008990: 2077 696c 6c20 7265 7665 7273 6520 6c6f   will reverse lo
+000089a0: 6f6b 7570 2070 686f 6e65 206e 756d 6265  okup phone numbe
+000089b0: 7220 6f76 6572 2069 6e74 6572 6e65 7420  r over internet 
+000089c0: 616e 6420 7368 6f77 2070 7562 6c69 6320  and show public 
+000089d0: 696e 666f 2061 7373 6f63 6961 7465 6420  info associated 
+000089e0: 7769 7468 2069 740a 2020 2020 1b5b 313b  with it.    .[1;
+000089f0: 3439 3b39 326d 3e20 5359 4e54 4158 3a20  49;92m> SYNTAX: 
+00008a00: 1b5b 313b 3439 3b39 376d 6e75 6d62 6572  .[1;49;97mnumber
+00008a10: 203c 7068 6f6e 655f 6e75 6d62 6572 3e0a   <phone_number>.
+00008a20: 2020 2020 1b5b 313b 3439 3b39 326d 3e20      .[1;49;92m> 
+00008a30: 4558 414d 504c 453a 201b 5b31 3b34 393b  EXAMPLE: .[1;49;
+00008a40: 3937 6d6e 756d 6265 7220 2b31 3233 3435  97mnumber +12345
+00008a50: 3637 3839 300a 2020 2020 1b5b 306d 7212  67890.    .[0mr.
+00008a60: 0000 0061 0501 0000 2020 1b5b 313b 3439  ...a....  .[1;49
+00008a70: 3b39 336d 5b2b 5d20 436f 6d6d 616e 6420  ;93m[+] Command 
+00008a80: 496e 666f 3a20 1b5b 313b 3439 3b39 336d  Info: .[1;49;93m
+00008a90: 7768 6f69 730a 0a20 2020 201b 5b31 3b34  whois..    .[1;4
+00008aa0: 393b 3932 6d3e 2044 4553 4352 4950 5449  9;92m> DESCRIPTI
+00008ab0: 4f4e 3a20 1b5b 313b 3439 3b39 376d 5768  ON: .[1;49;97mWh
+00008ac0: 656e 2079 6f75 2074 7970 6520 6077 686f  en you type `who
+00008ad0: 6973 602c 2069 7420 7769 6c6c 2070 6572  is`, it will per
+00008ae0: 666f 726d 2072 6576 6572 7365 2077 686f  form reverse who
+00008af0: 6973 206c 6f6f 6b75 700a 2020 2020 1b5b  is lookup.    .[
+00008b00: 313b 3439 3b39 326d 3e20 5359 4e54 4158  1;49;92m> SYNTAX
+00008b10: 3a20 1b5b 313b 3439 3b39 376d 7768 6f69  : .[1;49;97mwhoi
+00008b20: 7320 3c64 6f6d 6169 6e5f 6e61 6d65 3e0a  s <domain_name>.
+00008b30: 2020 2020 1b5b 313b 3439 3b39 326d 3e20      .[1;49;92m> 
+00008b40: 4558 414d 504c 453a 201b 5b31 3b34 393b  EXAMPLE: .[1;49;
+00008b50: 3937 6d77 686f 6973 2065 7861 6d70 6c65  97mwhois example
+00008b60: 2e63 6f6d 0a20 2020 201b 5b30 6d72 0700  .com.    .[0mr..
+00008b70: 0000 6166 0100 0020 201b 5b31 3b34 393b  ..af...  .[1;49;
+00008b80: 3933 6d5b 2b5d 2043 6f6d 6d61 6e64 2049  93m[+] Command I
+00008b90: 6e66 6f3a 201b 5b31 3b34 393b 3933 6d64  nfo: .[1;49;93md
+00008ba0: 6e73 0a0a 2020 2020 1b5b 313b 3439 3b39  ns..    .[1;49;9
+00008bb0: 326d 3e20 4445 5343 5249 5054 494f 4e3a  2m> DESCRIPTION:
+00008bc0: 201b 5b31 3b34 393b 3937 6d57 6865 6e20   .[1;49;97mWhen 
+00008bd0: 796f 7520 7479 7065 2060 646e 7360 2c20  you type `dns`, 
+00008be0: 6974 2077 696c 6c20 7065 7266 6f72 6d20  it will perform 
+00008bf0: 646e 7320 6c6f 6f6b 7570 2066 6f72 2067  dns lookup for g
+00008c00: 6976 656e 2064 6f6d 6169 6e20 6e61 6d65  iven domain name
+00008c10: 206f 7220 7265 7665 7273 6520 646e 7320   or reverse dns 
+00008c20: 6c6f 6f6b 7570 2066 6f72 2067 6976 656e  lookup for given
+00008c30: 2069 7020 6164 6472 6573 730a 2020 2020   ip address.    
+00008c40: 1b5b 313b 3439 3b39 326d 3e20 5359 4e54  .[1;49;92m> SYNT
+00008c50: 4158 3a20 1b5b 313b 3439 3b39 376d 646e  AX: .[1;49;97mdn
+00008c60: 7320 3c69 705f 6164 6472 6573 732f 646f  s <ip_address/do
+00008c70: 6d61 696e 5f6e 616d 653e 0a20 2020 201b  main_name>.    .
+00008c80: 5b31 3b34 393b 3932 6d3e 2045 5841 4d50  [1;49;92m> EXAMP
+00008c90: 4c45 3a20 1b5b 313b 3439 3b39 376d 646e  LE: .[1;49;97mdn
+00008ca0: 7320 3139 322e 3136 382e 312e 3120 1b5b  s 192.168.1.1 .[
+00008cb0: 313b 3439 3b39 326d 4f52 201b 5b31 3b34  1;49;92mOR .[1;4
+00008cc0: 393b 3937 6d64 6e73 2065 7861 6d70 6c65  9;97mdns example
+00008cd0: 2e63 6f6d 0a20 2020 201b 5b30 6d72 0c00  .com.    .[0mr..
+00008ce0: 0000 6127 0100 0020 201b 5b31 3b34 393b  ..a'...  .[1;49;
+00008cf0: 3933 6d5b 2b5d 2043 6f6d 6d61 6e64 2049  93m[+] Command I
+00008d00: 6e66 6f3a 201b 5b31 3b34 393b 3933 6d69  nfo: .[1;49;93mi
+00008d10: 700a 0a20 2020 201b 5b31 3b34 393b 3932  p..    .[1;49;92
+00008d20: 6d3e 2044 4553 4352 4950 5449 4f4e 3a20  m> DESCRIPTION: 
+00008d30: 1b5b 313b 3439 3b39 376d 5768 656e 2079  .[1;49;97mWhen y
+00008d40: 6f75 2074 7970 6520 6069 7060 2c20 6974  ou type `ip`, it
+00008d50: 2077 696c 6c20 7065 7266 6f72 6d20 616e   will perform an
+00008d60: 2069 7020 6164 6472 6573 7320 6c6f 6f6b   ip address look
+00008d70: 7570 206f 7665 7220 696e 7465 726e 6574  up over internet
+00008d80: 2061 6e64 2073 686f 7720 696e 666f 2061   and show info a
+00008d90: 626f 7574 2067 6976 656e 2069 7020 6164  bout given ip ad
+00008da0: 6472 6573 730a 2020 2020 1b5b 313b 3439  dress.    .[1;49
+00008db0: 3b39 326d 3e20 5359 4e54 4158 3a20 1b5b  ;92m> SYNTAX: .[
+00008dc0: 313b 3439 3b39 376d 6970 203c 6970 5f61  1;49;97mip <ip_a
+00008dd0: 6464 7265 7373 3e0a 2020 2020 1b5b 313b  ddress>.    .[1;
+00008de0: 3439 3b39 326d 3e20 4558 414d 504c 453a  49;92m> EXAMPLE:
+00008df0: 201b 5b31 3b34 393b 3937 6d69 7020 382e   .[1;49;97mip 8.
+00008e00: 382e 382e 380a 2020 2020 1b5b 306d 720d  8.8.8.    .[0mr.
+00008e10: 0000 0061 1e01 0000 2020 1b5b 313b 3439  ...a....  .[1;49
+00008e20: 3b39 336d 5b2b 5d20 436f 6d6d 616e 6420  ;93m[+] Command 
+00008e30: 496e 666f 3a20 1b5b 313b 3439 3b39 336d  Info: .[1;49;93m
+00008e40: 6d61 630a 0a20 2020 201b 5b31 3b34 393b  mac..    .[1;49;
+00008e50: 3932 6d3e 2044 4553 4352 4950 5449 4f4e  92m> DESCRIPTION
+00008e60: 3a20 1b5b 313b 3439 3b39 376d 5768 656e  : .[1;49;97mWhen
+00008e70: 2079 6f75 2074 7970 6520 606d 6163 602c   you type `mac`,
+00008e80: 2069 7420 7769 6c6c 206c 6f6f 6b75 7020   it will lookup 
+00008e90: 7072 6f62 6162 6c65 2076 656e 646f 722f  probable vendor/
+00008ea0: 6d61 6e75 6661 6374 7572 6520 6f66 2067  manufacture of g
+00008eb0: 6976 656e 206d 6163 2061 6464 7265 7373  iven mac address
+00008ec0: 0a20 2020 201b 5b31 3b34 393b 3932 6d3e  .    .[1;49;92m>
+00008ed0: 2053 594e 5441 583a 201b 5b31 3b34 393b   SYNTAX: .[1;49;
+00008ee0: 3937 6d6d 6163 203c 6d61 635f 6164 6472  97mmac <mac_addr
+00008ef0: 6573 733e 0a20 2020 201b 5b31 3b34 393b  ess>.    .[1;49;
+00008f00: 3932 6d3e 2045 5841 4d50 4c45 3a20 1b5b  92m> EXAMPLE: .[
+00008f10: 313b 3439 3b39 376d 6d61 6320 6666 3a66  1;49;97mmac ff:f
+00008f20: 663a 6666 3a66 663a 6666 3a66 660a 2020  f:ff:ff:ff:ff.  
+00008f30: 2020 1b5b 306d e903 0000 007a 4720 2020    .[0m.....zG   
+00008f40: 205b 215d 2049 6e76 616c 6964 2073 7562   [!] Invalid sub
+00008f50: 2d63 6f6d 6d61 6e64 2120 5479 7065 2060  -command! Type `
+00008f60: 6865 6c70 6020 746f 2073 6565 2061 6c6c  help` to see all
+00008f70: 2061 7661 696c 6162 6c65 2063 6f6d 6d61   available comma
+00008f80: 6e64 732e 722c 0000 0072 2e00 0000 7a43  nds.r,...r....zC
+00008f90: 2020 2020 5b21 5d20 496e 7661 6c69 6420      [!] Invalid 
+00008fa0: 636f 6d6d 616e 6421 2054 7970 6520 6068  command! Type `h
+00008fb0: 656c 7060 2074 6f20 7365 6520 616c 6c20  elp` to see all 
+00008fc0: 6176 6169 6c61 626c 6520 636f 6d6d 616e  available comman
+00008fd0: 6473 2e7a 3820 2020 205b 405d 2054 6861  ds.z8    [@] Tha
+00008fe0: 6e6b 2079 6f75 2066 6f72 2075 7369 6e67  nk you for using
+00008ff0: 2060 5048 304d 4245 5260 206f 7369 6e74   `PH0MBER` osint
+00009000: 2066 7261 6d65 776f 726b 203a 297a 2720   framework :)z' 
+00009010: 2020 205b 2b5d 2047 656e 6572 6174 696e     [+] Generatin
+00009020: 6720 7261 6e64 6f6d 2064 6f72 6b20 7175  g random dork qu
+00009030: 6572 792e 2e2e 7223 0000 0072 2700 0000  ery...r#...r'...
+00009040: 7a06 2020 2020 3e20 2903 7224 0000 0072  z.    > ).r$...r
+00009050: 2500 0000 72c6 0000 007a 2720 2020 205b  %...r....z'    [
+00009060: 2b5d 2043 6865 636b 696e 6720 696e 7465  +] Checking inte
+00009070: 726e 6574 2063 6f6e 6e65 6374 696f 6e2e  rnet connection.
+00009080: 2e2e 7a17 6874 7470 733a 2f2f 7777 772e  ..z.https://www.
+00009090: 676f 6f67 6c65 2e63 6f6d 2f7a 2720 2020  google.com/z'   
+000090a0: 203e 2049 6e74 6572 6e65 7420 636f 6e6e   > Internet conn
+000090b0: 6563 7469 6f6e 2069 7320 6176 6169 6c61  ection is availa
+000090c0: 626c 6521 7a16 6874 7470 733a 2f2f 6874  ble!z.https://ht
+000090d0: 7470 6269 6e2e 6f72 672f 6970 da06 6f72  tpbin.org/ip..or
+000090e0: 6967 696e 7a10 6874 7470 733a 2f2f 6964  iginz.https://id
+000090f0: 656e 742e 6d65 7a15 6874 7470 733a 2f2f  ent.mez.https://
+00009100: 6170 692e 6970 6966 792e 6f72 6746 7a19  api.ipify.orgFz.
+00009110: 2020 2020 3e20 5075 626c 6963 2049 5020      > Public IP 
+00009120: 6164 6472 6573 733a 207a 2b20 2020 203e  address: z+    >
+00009130: 2049 6e74 6572 6e65 7420 636f 6e6e 6563   Internet connec
+00009140: 7469 6f6e 2069 7320 6e6f 7420 6176 6169  tion is not avai
+00009150: 6c61 626c 6521 7a21 2020 2020 3e20 4c6f  lable!z!    > Lo
+00009160: 6361 6c20 4950 2061 6464 7265 7373 3a20  cal IP address: 
+00009170: 3132 372e 302e 302e 3172 af00 0000 72c5  127.0.0.1r....r.
+00009180: 0000 007a 2c20 2020 205b 2b5d 2053 6176  ...z,    [+] Sav
+00009190: 696e 6720 6f75 7470 7574 206f 6620 7072  ing output of pr
+000091a0: 6576 696f 7573 2063 6f6d 6d61 6e64 2e2e  evious command..
+000091b0: 2e7a 4520 2020 203e 204e 6f20 6f75 7470  .zE    > No outp
+000091c0: 7574 2066 6f75 6e64 2120 5361 7665 7320  ut found! Saves 
+000091d0: 6f75 7470 7574 206f 6620 7072 6576 696f  output of previo
+000091e0: 7573 2073 6361 6e6e 6572 2063 6f6d 6d61  us scanner comma
+000091f0: 6e64 206f 6e6c 7921 7253 0000 007a 3b20  nd only!rS...z; 
+00009200: 2020 203e 204e 6f20 636f 6d6d 616e 6420     > No command 
+00009210: 666f 756e 6421 2054 7970 6520 6068 656c  found! Type `hel
+00009220: 7020 7368 656c 6c60 2074 6f20 7365 6520  p shell` to see 
+00009230: 6d6f 7265 2069 6e66 6f2e e906 0000 007a  more info......z
+00009240: 2520 2020 201b 5b37 3b34 393b 3933 6d5b  %    .[7;49;93m[
+00009250: 2b5d 2045 7865 6375 7469 6e67 2063 6f6d  +] Executing com
+00009260: 6d61 6e64 3a20 7a05 1b5b 306d 0a7a 203e  mand: z..[0m.z >
+00009270: 2043 6f6d 6d61 6e64 2065 7865 6375 7465   Command execute
+00009280: 6420 7375 6363 6573 7366 756c 6c79 2129  d successfully!)
+00009290: 03e9 0700 0000 7225 0000 0072 c600 0000  ......r%...r....
+000092a0: 7a05 0a20 2020 2029 0272 2800 0000 72ab  z..    ).r(...r.
+000092b0: 0000 007a 1b3e 2043 6f6d 6d61 6e64 2065  ...z.> Command e
+000092c0: 7865 6375 7469 6f6e 2066 6169 6c65 6421  xecution failed!
+000092d0: 2903 72e3 0000 0072 2500 0000 722d 0000  ).r....r%...r-..
+000092e0: 007a 3f20 2020 203e 204e 6f20 636f 6c6f  .z?    > No colo
+000092f0: 7220 636f 6465 2066 6f75 6e64 2120 5479  r code found! Ty
+00009300: 7065 2060 6865 6c70 2063 6861 6e67 6560  pe `help change`
+00009310: 2074 6f20 7365 6520 6d6f 7265 2069 6e66   to see more inf
+00009320: 6f2e 72e3 0000 00da 0130 7a2a 2020 2020  o.r......0z*    
+00009330: 3e20 436f 6c6f 7220 6368 616e 6765 6420  > Color changed 
+00009340: 7375 6363 6573 7366 756c 6c79 2074 6f20  successfully to 
+00009350: 424c 4143 4b21 da01 317a 2a20 2020 203e  BLACK!..1z*    >
+00009360: 2043 6f6c 6f72 2063 6861 6e67 6564 2073   Color changed s
+00009370: 7563 6365 7373 6675 6c6c 7920 746f 2057  uccessfully to W
+00009380: 4849 5445 217a 4020 2020 205b 215d 2049  HITE!z@    [!] I
+00009390: 6e76 616c 6964 2063 6f6c 6f72 2063 6f64  nvalid color cod
+000093a0: 6521 2054 7970 6520 6068 656c 7020 6368  e! Type `help ch
+000093b0: 616e 6765 6020 746f 2073 6565 206d 6f72  ange` to see mor
+000093c0: 6520 696e 666f 2e7a 4020 2020 203e 204e  e info.z@    > N
+000093d0: 6f20 7068 6f6e 6520 6e75 6d62 6572 2066  o phone number f
+000093e0: 6f75 6e64 2120 5479 7065 2060 6865 6c70  ound! Type `help
+000093f0: 206e 756d 6265 7260 2074 6f20 7365 6520   number` to see 
+00009400: 6d6f 7265 2069 6e66 6f7a 3120 2020 205b  more infoz1    [
+00009410: 2b5d 2050 6572 666f 726d 696e 6720 7265  +] Performing re
+00009420: 7665 7273 6520 7068 6f6e 6520 6e75 6d62  verse phone numb
+00009430: 6572 206c 6f6f 6b75 702e 2e2e 7a3a 2020  er lookup...z:  
+00009440: 2020 3e20 4e6f 2069 7020 6164 6472 6573    > No ip addres
+00009450: 7320 666f 756e 6421 2054 7970 6520 6068  s found! Type `h
+00009460: 656c 7020 6970 6020 746f 2073 6565 206d  elp ip` to see m
+00009470: 6f72 6520 696e 666f 7a2f 2020 2020 5b2b  ore infoz/    [+
+00009480: 5d20 5065 7266 6f72 6d69 6e67 2072 6576  ] Performing rev
+00009490: 6572 7365 2069 7020 6164 6472 6573 7320  erse ip address 
+000094a0: 6c6f 6f6b 7570 2e2e 2e7a 3c20 2020 203e  lookup...z<    >
+000094b0: 204e 6f20 6d61 6320 6164 6472 6573 7320   No mac address 
+000094c0: 666f 756e 6421 2054 7970 6520 6068 656c  found! Type `hel
+000094d0: 7020 6d61 6360 2074 6f20 7365 6520 6d6f  p mac` to see mo
+000094e0: 7265 2069 6e66 6f7a 3020 2020 205b 2b5d  re infoz0    [+]
+000094f0: 2050 6572 666f 726d 696e 6720 7265 7665   Performing reve
+00009500: 7273 6520 6d61 6320 6164 6472 6573 7320  rse mac address 
+00009510: 6c6f 6f6b 7570 2e2e 2e7a 3920 2020 203e  lookup...z9    >
+00009520: 204e 6f20 646f 6d61 696e 2066 6f75 6e64   No domain found
+00009530: 2120 5479 7065 2060 6865 6c70 2077 686f  ! Type `help who
+00009540: 6973 6020 746f 2073 6565 206d 6f72 6520  is` to see more 
+00009550: 696e 666f 7a2b 2020 2020 5b2b 5d20 5065  infoz+    [+] Pe
+00009560: 7266 6f72 6d69 6e67 2072 6576 6572 7365  rforming reverse
+00009570: 2064 6f6d 6169 6e20 6c6f 6f6b 7570 2e2e   domain lookup..
+00009580: 2e7a 3720 2020 203e 204e 6f20 646f 6d61  .z7    > No doma
+00009590: 696e 2066 6f75 6e64 2120 5479 7065 2060  in found! Type `
+000095a0: 6865 6c70 2064 6e73 6020 746f 2073 6565  help dns` to see
+000095b0: 206d 6f72 6520 696e 666f 7a20 2020 2020   more infoz     
+000095c0: 5b2b 5d20 5065 7266 6f72 6d69 6e67 2064  [+] Performing d
+000095d0: 6e73 206c 6f6f 6b75 702e 2e2e 292d da0b  ns lookup...)-..
+000095e0: 7369 6c65 6e74 5f6d 6f64 6572 3e00 0000  silent_moder>...
+000095f0: 7218 0000 0072 1900 0000 7242 0000 0072  r....r....rB...r
+00009600: a200 0000 da08 6765 746c 6f67 696e 7246  ......getloginrF
+00009610: 0000 0072 4700 0000 72b3 0000 00da 086e  ...rG...r......n
+00009620: 6f64 656e 616d 65da 0773 7973 6e61 6d65  odename..sysname
+00009630: da06 7073 7574 696c 5a0e 7669 7274 7561  ..psutilZ.virtua
+00009640: 6c5f 6d65 6d6f 7279 da07 7065 7263 656e  l_memory..percen
+00009650: 745a 0b63 7075 5f70 6572 6365 6e74 da0a  tZ.cpu_percent..
+00009660: 6469 736b 5f75 7361 6765 da04 6a6f 696e  disk_usage..join
+00009670: 723f 0000 00da 0766 696e 6461 6c6c da04  r?.....findall..
+00009680: 7575 6964 5a07 6765 746e 6f64 65da 076d  uuidZ.getnode..m
+00009690: 6163 6869 6e65 da08 7265 6164 6c69 6e65  achine..readline
+000096a0: da0e 7061 7273 655f 616e 645f 6269 6e64  ..parse_and_bind
+000096b0: 5a0d 7365 745f 636f 6d70 6c65 7465 7272  Z.set_completerr
+000096c0: d700 0000 7244 0000 0072 3d00 0000 7248  ....rD...r=...rH
+000096d0: 0000 00da 114b 6579 626f 6172 6449 6e74  .....KeyboardInt
+000096e0: 6572 7275 7074 72c4 0000 0072 1600 0000  erruptr....r....
+000096f0: 7217 0000 0072 7f00 0000 72a6 0000 0072  r....r....r....r
+00009700: cb00 0000 72cc 0000 0072 be00 0000 72b4  ....r....r....r.
+00009710: 0000 0072 4f00 0000 7284 0000 0072 8d00  ...rO...r....r..
+00009720: 0000 7299 0000 0072 9d00 0000 2926 7209  ..r....r....)&r.
+00009730: 0000 005a 0763 7274 5f65 7870 5a08 6578  ...Z.crt_expZ.ex
+00009740: 705f 696e 666f da04 7573 6572 da08 686f  p_info..user..ho
+00009750: 7374 6e61 6d65 72ba 0000 005a 0372 616d  stnamer....Z.ram
+00009760: 5a03 6370 755a 0464 6973 6b5a 0773 7973  Z.cpuZ.diskZ.sys
+00009770: 5f6d 6163 da04 6172 6368 da03 7665 725a  _mac..arch..verZ
+00009780: 0773 7973 696e 666f 720a 0000 005a 0474  .sysinfor....Z.t
+00009790: 6970 7372 b700 0000 5a09 636d 645f 636f  ipsr....Z.cmd_co
+000097a0: 6c6f 725a 0963 7274 5f63 6f6c 6f72 da03  lorZ.crt_color..
+000097b0: 636d 645a 0374 6970 5a09 6865 6c70 5f68  cmdZ.tipZ.help_h
+000097c0: 656c 705a 0965 7869 745f 6865 6c70 5a09  elpZ.exit_helpZ.
+000097d0: 646f 726b 5f68 656c 705a 0865 7870 5f68  dork_helpZ.exp_h
+000097e0: 656c 705a 0a63 6865 636b 5f68 656c 705a  elpZ.check_helpZ
+000097f0: 0a63 6c65 6172 5f68 656c 705a 0973 6176  .clear_helpZ.sav
+00009800: 655f 6865 6c70 5a0a 7368 656c 6c5f 6865  e_helpZ.shell_he
+00009810: 6c70 5a09 696e 666f 5f68 656c 705a 0b63  lpZ.info_helpZ.c
+00009820: 6861 6e67 655f 6865 6c70 5a0b 6e75 6d62  hange_helpZ.numb
+00009830: 6572 5f68 656c 705a 0a77 686f 6973 5f68  er_helpZ.whois_h
+00009840: 656c 705a 0864 6e73 5f68 656c 705a 0769  elpZ.dns_helpZ.i
+00009850: 705f 6865 6c70 5a08 6d61 635f 6865 6c70  p_helpZ.mac_help
+00009860: 5a09 7075 626c 6963 5f69 705a 0865 7865  Z.public_ipZ.exe
+00009870: 635f 636d 64da 066f 7574 7075 7472 1b00  c_cmd..outputr..
+00009880: 0000 721b 0000 0072 1c00 0000 da0e 636f  ..r....r......co
+00009890: 6e74 726f 6c5f 6365 6e74 6572 5f03 0000  ntrol_center_...
+000098a0: 732a 0200 0000 0526 0908 0708 0204 0f30  s*.....&.......0
+000098b0: 0134 0134 0138 0134 013c 0154 0134 021c  .4.4.8.4.<.T.4..
+000098c0: 0202 0402 fc04 0502 fb04 0602 fa04 0702  ................
+000098d0: f904 0802 f804 0a02 f604 0b02 f504 0c02  ................
+000098e0: f404 1302 ed08 1a04 1f08 0804 050a 010a  ................
+000098f0: 0308 0108 0528 020a 0108 0104 0108 010a  .....(..........
+00009900: 0114 0112 0112 010c 010a 0108 0104 050c  ................
+00009910: 0114 0108 0104 040c 010a 0108 0104 040c  ................
+00009920: 010a 0108 0104 040c 010a 0108 0104 040c  ................
+00009930: 010a 0108 0104 040c 010a 0108 0104 050c  ................
+00009940: 0112 0108 0104 050a 010a 0108 0104 040a  ................
+00009950: 010a 0108 0104 080a 010a 0108 0104 050a  ................
+00009960: 010a 0108 0104 050a 010a 0108 0104 050a  ................
+00009970: 010a 0108 0104 050a 010a 0108 0104 050a  ................
+00009980: 0208 0112 0208 0110 0108 0314 0122 0208  ............."..
+00009990: 010a 0108 0104 0112 011a 010a 0108 0104  ................
+000099a0: 010c 010a 0112 0102 010a 0110 0102 0116  ................
+000099b0: 0106 0102 0110 0106 0102 0110 0106 0116  ................
+000099c0: 0106 0116 010c 0106 0110 0110 010e 0108  ................
+000099d0: 010a 0108 0104 011e 010a 0112 010a 0110  ................
+000099e0: 010a 020a 010a 0208 0108 010a 0108 0104  ................
+000099f0: 0114 0112 0112 010c 0110 0108 020a 010a  ................
+00009a00: 0112 010a 0212 010a 0208 0110 0108 010a  ................
+00009a10: 0108 0104 010c 010a 0108 0104 0114 0112  ................
+00009a20: 0112 010c 010a 0108 0108 0112 010a 0108  ................
+00009a30: 0108 0112 0208 0112 0208 0110 0108 030a  ................
+00009a40: 0108 0114 0112 0104 0112 010c 0112 010a  ................
+00009a50: 010a 0208 0106 0208 0114 010a 0108 0114  ................
+00009a60: 0112 0104 0112 010c 0112 010a 010a 0208  ................
+00009a70: 0106 0208 0114 010a 0108 0114 0112 0104  ................
+00009a80: 0112 010c 0112 010a 010a 0208 0106 0208  ................
+00009a90: 0114 010a 0108 0114 0112 0104 0112 010c  ................
+00009aa0: 0112 010a 010a 0208 0106 0208 0112 010a  ................
+00009ab0: 0108 0112 0112 0104 0112 010c 0112 010a  ................
+00009ac0: 010a 0208 0106 0208 0112 0408 0110 0372  ...............r
+00009ad0: fa00 0000 6300 0000 0000 0000 0000 0000  ....c...........
+00009ae0: 0000 0000 000b 0000 0043 0000 0073 a000  .........C...s..
+00009af0: 0000 7a24 7400 6a01 6401 1900 6402 6b02  ..z$t.j.d...d.k.
+00009b00: 731e 7400 6a01 6401 1900 6403 6b02 7222  s.t.j.d...d.k.r"
+00009b10: 6404 6102 5700 6e12 0400 7403 7936 0100  d.a.W.n...t.y6..
+00009b20: 0100 0100 5900 6e02 3000 7402 7342 7404  ....Y.n.0.t.sBt.
+00009b30: 8300 0100 7a0a 7405 8300 0100 5700 6e4e  ....z.t.....W.nN
+00009b40: 0400 7406 799a 0100 0100 0100 7407 8300  ..t.y.......t...
+00009b50: 0100 7402 7390 7408 6405 6401 6406 7409  ..t.s.t.d.d.d.t.
+00009b60: a00a 6407 6408 6702 a101 6703 6404 6404  ..d.d.g...g.d.d.
+00009b70: 6404 6404 6409 8d06 0100 740b 8300 0100  d.d.d.....t.....
+00009b80: 6e06 7407 8300 0100 5900 6e02 3000 6400  n.t.....Y.n.0.d.
+00009b90: 5300 290a 4e72 2400 0000 7a02 2d73 7a08  S.).Nr$...z.-sz.
+00009ba0: 2d2d 7369 6c65 6e74 547a 265b 235d 2054  --silentTz&[#] T
+00009bb0: 6572 6d69 6e61 7469 6e67 2060 5048 304d  erminating `PH0M
+00009bc0: 4245 5260 2066 7261 6d65 776f 726b 2e2e  BER` framework..
+00009bd0: 2e72 2500 0000 722d 0000 0072 2600 0000  .r%...r-...r&...
+00009be0: 2905 7228 0000 0072 2900 0000 72a9 0000  ).r(...r)...r...
+00009bf0: 0072 a800 0000 72aa 0000 0029 0cda 0373  .r....r....)...s
+00009c00: 7973 da04 6172 6776 72e6 0000 00da 0a49  ys..argvr......I
+00009c10: 6e64 6578 4572 726f 7272 cd00 0000 72fa  ndexErrorr....r.
+00009c20: 0000 0072 f300 0000 7248 0000 0072 3e00  ...r....rH...r>.
+00009c30: 0000 7218 0000 0072 1900 0000 7208 0000  ..r....r....r...
+00009c40: 0072 1b00 0000 721b 0000 0072 1b00 0000  .r....r....r....
+00009c50: 721c 0000 00da 046d 6169 6e26 0500 0073  r......main&...s
+00009c60: 1c00 0000 0005 0201 1c01 0801 0c01 0603  ................
+00009c70: 0a03 0201 0a01 0c01 0601 0401 2401 0801  ............$...
+00009c80: 72fe 0000 0029 2372 1600 0000 72a2 0000  r....)#r....r...
+00009c90: 0072 fb00 0000 7218 0000 0072 b000 0000  .r....r....r....
+00009ca0: 72f1 0000 0072 3f00 0000 72ef 0000 0072  r....r?...r....r
+00009cb0: 9a00 0000 72ea 0000 0072 c200 0000 723c  ....r....r....r<
+00009cc0: 0000 005a 116d 6163 5f76 656e 646f 725f  ...Z.mac_vendor_
+00009cd0: 6c6f 6f6b 7570 7202 0000 0072 1200 0000  lookupr....r....
+00009ce0: 5a0c 646e 732e 7265 736f 6c76 6572 7207  Z.dns.resolverr.
+00009cf0: 0000 0072 d300 0000 da08 656c 656d 656e  ...r......elemen
+00009d00: 7473 723d 0000 0072 b400 0000 72e6 0000  tsr=...r....r...
+00009d10: 0072 1d00 0000 724f 0000 0072 8400 0000  .r....rO...r....
+00009d20: 728d 0000 0072 9900 0000 729d 0000 0072  r....r....r....r
+00009d30: 3e00 0000 72be 0000 0072 c400 0000 72cd  >...r....r....r.
+00009d40: 0000 0072 d700 0000 72fa 0000 0072 fe00  ...r....r....r..
+00009d50: 0000 721b 0000 0072 1b00 0000 721b 0000  ..r....r....r...
+00009d60: 0072 1c00 0000 da08 3c6d 6f64 756c 653e  .r......<module>
+00009d70: 2000 0000 734a 0000 0008 0108 0108 0108   ...sJ..........
+00009d80: 0108 0108 0108 0108 0108 0108 0108 0108  ................
+00009d90: 010c 0108 0108 040c 0104 0104 0104 0508  ................
+00009da0: 0a08 7f00 0e08 7f00 7f00 6608 2c08 4b08  ..........f.,.K.
+00009db0: 3824 2008 2b08 1c08 0a08 0a08 7f00 7f00  8$ .+...........
+00009dc0: 7f00 4a                                  ..J
```

