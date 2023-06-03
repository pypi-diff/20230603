# Comparing `tmp/firegs-0.7.tar.gz` & `tmp/firegs-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "firegs-0.7.tar", last modified: Sat Jun  3 17:33:35 2023, max compression
+gzip compressed data, was "firegs-0.8.tar", last modified: Sat Jun  3 17:43:55 2023, max compression
```

## Comparing `firegs-0.7.tar` & `firegs-0.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 ask        (501) staff       (20)        0 2023-06-03 17:33:35.653414 firegs-0.7/
--rw-r--r--   0 ask        (501) staff       (20)     1074 2023-06-03 14:51:55.000000 firegs-0.7/LICENSE
--rw-r--r--   0 ask        (501) staff       (20)     1330 2023-06-03 17:33:35.653265 firegs-0.7/PKG-INFO
--rw-r--r--   0 ask        (501) staff       (20)      932 2023-06-03 14:51:08.000000 firegs-0.7/README.md
-drwxr-xr-x   0 ask        (501) staff       (20)        0 2023-06-03 17:33:35.651936 firegs-0.7/firegs/
--rw-r--r--   0 ask        (501) staff       (20)        0 2023-06-03 14:45:22.000000 firegs-0.7/firegs/__init__.py
--rw-r--r--   0 ask        (501) staff       (20)     5921 2023-06-03 16:53:08.000000 firegs-0.7/firegs/script.py
--rw-r--r--   0 ask        (501) staff       (20)       19 2023-06-03 17:33:30.000000 firegs-0.7/firegs/version.py
-drwxr-xr-x   0 ask        (501) staff       (20)        0 2023-06-03 17:33:35.652848 firegs-0.7/firegs.egg-info/
--rw-r--r--   0 ask        (501) staff       (20)     1330 2023-06-03 17:33:35.000000 firegs-0.7/firegs.egg-info/PKG-INFO
--rw-r--r--   0 ask        (501) staff       (20)      262 2023-06-03 17:33:35.000000 firegs-0.7/firegs.egg-info/SOURCES.txt
--rw-r--r--   0 ask        (501) staff       (20)        1 2023-06-03 17:33:35.000000 firegs-0.7/firegs.egg-info/dependency_links.txt
--rw-r--r--   0 ask        (501) staff       (20)       46 2023-06-03 17:33:35.000000 firegs-0.7/firegs.egg-info/entry_points.txt
--rw-r--r--   0 ask        (501) staff       (20)       88 2023-06-03 17:33:35.000000 firegs-0.7/firegs.egg-info/requires.txt
--rw-r--r--   0 ask        (501) staff       (20)        7 2023-06-03 17:33:35.000000 firegs-0.7/firegs.egg-info/top_level.txt
--rw-r--r--   0 ask        (501) staff       (20)       38 2023-06-03 17:33:35.653468 firegs-0.7/setup.cfg
--rw-r--r--   0 ask        (501) staff       (20)      879 2023-06-03 16:53:08.000000 firegs-0.7/setup.py
+drwxr-xr-x   0 ask        (501) staff       (20)        0 2023-06-03 17:43:55.095185 firegs-0.8/
+-rw-r--r--   0 ask        (501) staff       (20)     1074 2023-06-03 14:51:55.000000 firegs-0.8/LICENSE
+-rw-r--r--   0 ask        (501) staff       (20)     1330 2023-06-03 17:43:55.095047 firegs-0.8/PKG-INFO
+-rw-r--r--   0 ask        (501) staff       (20)      932 2023-06-03 14:51:08.000000 firegs-0.8/README.md
+drwxr-xr-x   0 ask        (501) staff       (20)        0 2023-06-03 17:43:55.094120 firegs-0.8/firegs/
+-rw-r--r--   0 ask        (501) staff       (20)        0 2023-06-03 14:45:22.000000 firegs-0.8/firegs/__init__.py
+-rw-r--r--   0 ask        (501) staff       (20)     6455 2023-06-03 17:43:27.000000 firegs-0.8/firegs/script.py
+-rw-r--r--   0 ask        (501) staff       (20)       19 2023-06-03 17:43:46.000000 firegs-0.8/firegs/version.py
+drwxr-xr-x   0 ask        (501) staff       (20)        0 2023-06-03 17:43:55.094855 firegs-0.8/firegs.egg-info/
+-rw-r--r--   0 ask        (501) staff       (20)     1330 2023-06-03 17:43:55.000000 firegs-0.8/firegs.egg-info/PKG-INFO
+-rw-r--r--   0 ask        (501) staff       (20)      262 2023-06-03 17:43:55.000000 firegs-0.8/firegs.egg-info/SOURCES.txt
+-rw-r--r--   0 ask        (501) staff       (20)        1 2023-06-03 17:43:55.000000 firegs-0.8/firegs.egg-info/dependency_links.txt
+-rw-r--r--   0 ask        (501) staff       (20)       46 2023-06-03 17:43:55.000000 firegs-0.8/firegs.egg-info/entry_points.txt
+-rw-r--r--   0 ask        (501) staff       (20)       88 2023-06-03 17:43:55.000000 firegs-0.8/firegs.egg-info/requires.txt
+-rw-r--r--   0 ask        (501) staff       (20)        7 2023-06-03 17:43:55.000000 firegs-0.8/firegs.egg-info/top_level.txt
+-rw-r--r--   0 ask        (501) staff       (20)       38 2023-06-03 17:43:55.095224 firegs-0.8/setup.cfg
+-rw-r--r--   0 ask        (501) staff       (20)      879 2023-06-03 16:53:08.000000 firegs-0.8/setup.py
```

### Comparing `firegs-0.7/LICENSE` & `firegs-0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `firegs-0.7/PKG-INFO` & `firegs-0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: firegs
-Version: 0.7
+Version: 0.8
 Summary: A tool to add app to Firebase project from the command line
 Home-page: https://github.com/androiddevnotes/firegs
 Author: Android Dev Notes
 Author-email: awesomedevnotes@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
```

### Comparing `firegs-0.7/README.md` & `firegs-0.8/README.md`

 * *Files identical despite different names*

### Comparing `firegs-0.7/firegs/script.py` & `firegs-0.8/firegs/script.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+# firegs/script.py
+
 import os
 import requests
 import json
 import configparser
 from google.oauth2 import service_account
 from google.auth.transport.requests import AuthorizedSession
 import argparse
@@ -36,131 +38,138 @@
         service_account_file = input("Please enter the path to your Service Account file: ")
         if not os.path.isfile(service_account_file):
             print("Invalid file path. Exiting.")
             exit(1)
     return service_account_file
 
 
-# Check if the configuration file exists
-if os.path.exists(config_file):
-    # If it exists, read it
-    config.read(config_file)
-
-    # Get the service account file path
-    SERVICE_ACCOUNT_FILE = config.get('DEFAULT', 'service_account_file')
-
-    # Get the project id if it exists
-    if config.has_option('DEFAULT', 'project_id'):
-        PROJECT_ID = config.get('DEFAULT', 'project_id')
-
-else:
-    # If it does not exist, prompt the user to enter the path
-    SERVICE_ACCOUNT_FILE = input('Please enter the path to your service account file: ')
+def main():
+
+    # Check if the configuration file exists
+    if os.path.exists(config_file):
+        # If it exists, read it
+        config.read(config_file)
+
+        # Get the service account file path
+        global SERVICE_ACCOUNT_FILE
+        SERVICE_ACCOUNT_FILE = config.get('DEFAULT', 'service_account_file')
+
+        # Get the project id if it exists
+        global PROJECT_ID
+        if config.has_option('DEFAULT', 'project_id'):
+            PROJECT_ID = config.get('DEFAULT', 'project_id')
+
+    else:
+        # If it does not exist, prompt the user to enter the path
+        SERVICE_ACCOUNT_FILE = input('Please enter the path to your service account file: ')
+
+        # Save the path to the configuration file for future use
+        config['DEFAULT'] = {'service_account_file': SERVICE_ACCOUNT_FILE}
+        with open(config_file, 'w') as f:
+            config.write(f)
+
+    # Parse command line arguments
+    parser = argparse.ArgumentParser(description='Manage Firebase Android Apps')
+    parser.add_argument('-p', '--project', help='Project ID for the Firebase project')
+    parser.add_argument('-c', '--create', help='Create an app with the provided Application ID or package name')
+    parser.add_argument('-d', '--display', help='Display name for the app')
+    parser.add_argument('-l', '--list', help='List all apps in the project', action='store_true')
+    parser.add_argument('-v', '--version', action='version', version=f'firegs {__version__}',
+                        help='Display the version of the program')
+    args = parser.parse_args()
+
+    if len(sys.argv) == 1:
+        print("Hello, welcome to firegs!")
+        exit()
+
+    if args.project:
+        PROJECT_ID = args.project
 
-    # Save the path to the configuration file for future use
-    config['DEFAULT'] = {'service_account_file': SERVICE_ACCOUNT_FILE}
+    PROJECT_ID = validate_project_id(PROJECT_ID)
+    SERVICE_ACCOUNT_FILE = validate_service_account_file(SERVICE_ACCOUNT_FILE)
+
+    # Save the project id to the configuration file for future use
+    config['DEFAULT']['project_id'] = PROJECT_ID
     with open(config_file, 'w') as f:
         config.write(f)
 
-# Parse command line arguments
-parser = argparse.ArgumentParser(description='Manage Firebase Android Apps')
-parser.add_argument('-p', '--project', help='Project ID for the Firebase project')
-parser.add_argument('-c', '--create', help='Create an app with the provided Application ID or package name')
-parser.add_argument('-d', '--display', help='Display name for the app')
-parser.add_argument('-l', '--list', help='List all apps in the project', action='store_true')
-parser.add_argument('-v', '--version', action='version', version=f'firegs {__version__}',
-                    help='Display the version of the program')
-args = parser.parse_args()
-
-if len(sys.argv) == 1:
-    print("Hello, welcome to firegs!")
-    exit()
-
-if args.project:
-    PROJECT_ID = args.project
-
-PROJECT_ID = validate_project_id(PROJECT_ID)
-SERVICE_ACCOUNT_FILE = validate_service_account_file(SERVICE_ACCOUNT_FILE)
-
-# Save the project id to the configuration file for future use
-config['DEFAULT']['project_id'] = PROJECT_ID
-with open(config_file, 'w') as f:
-    config.write(f)
-
-# API endpoint for creating apps
-CREATE_APP_URL = f"https://firebase.googleapis.com/v1beta1/projects/{PROJECT_ID}/androidApps"
-
-# API endpoint for listing apps
-LIST_APPS_URL = f"https://firebase.googleapis.com/v1beta1/projects/{PROJECT_ID}/androidApps"
-
-# Firebase project URL
-FIREBASE_PROJECT_URL = f"https://console.firebase.google.com/project/{PROJECT_ID}/settings/general"
-
-# Load credentials from the service account file
-credentials = service_account.Credentials.from_service_account_file(
-    SERVICE_ACCOUNT_FILE,
-    scopes=['https://www.googleapis.com/auth/cloud-platform'],
-)
-
-# Create an authorized session
-authed_session = AuthorizedSession(credentials)
-
-# Create a new Android app
-if args.create:
-    app_id = args.create
-    display_name = args.display if args.display else app_id  # Use the app ID as the display name if no display name is provided
-    payload = {
-        'packageName': app_id,
-        'displayName': display_name,
-    }
-
-    print(f'Creating a new Android app with ID/package name: {app_id} in project: {PROJECT_ID}')
-
-    try:
-        response = authed_session.post(CREATE_APP_URL, json=payload)
-        response.raise_for_status()
-        print(f'Successfully created the Android app with ID/package name: {app_id} and Display name: {display_name}')
-
-        # Open Firebase project page in browser
-        webbrowser.open(FIREBASE_PROJECT_URL)
-    except requests.exceptions.HTTPError as e:
-        if e.response.status_code == 409:
-            print(f'The Android app with ID/package name: {app_id} already exists in the Firebase project.')
-        else:
-            print(f'Error creating the Android app: {e}')
-            exit(1)
-elif args.list:
-    # Initialize an empty list to store all apps
-    all_apps = []
-
-    # Initialize nextPageToken to None for the first API call
-    next_page_token = None
-
-    while True:
-        # Create the API URL with the nextPageToken parameter if it is not None
-        list_apps_url = LIST_APPS_URL
-        if next_page_token is not None:
-            list_apps_url += f'?pageToken={next_page_token}'
+    # API endpoint for creating apps
+    CREATE_APP_URL = f"https://firebase.googleapis.com/v1beta1/projects/{PROJECT_ID}/androidApps"
+
+    # API endpoint for listing apps
+    LIST_APPS_URL = f"https://firebase.googleapis.com/v1beta1/projects/{PROJECT_ID}/androidApps"
+
+    # Firebase project URL
+    FIREBASE_PROJECT_URL = f"https://console.firebase.google.com/project/{PROJECT_ID}/settings/general"
+
+    # Load credentials from the service account file
+    credentials = service_account.Credentials.from_service_account_file(
+        SERVICE_ACCOUNT_FILE,
+        scopes=['https://www.googleapis.com/auth/cloud-platform'],
+    )
+
+    # Create an authorized session
+    authed_session = AuthorizedSession(credentials)
+
+    # Create a new Android app
+    if args.create:
+        app_id = args.create
+        display_name = args.display if args.display else app_id  # Use the app ID as the display name if no display name is provided
+        payload = {
+            'packageName': app_id,
+            'displayName': display_name,
+        }
+
+        print(f'Creating a new Android app with ID/package name: {app_id} in project: {PROJECT_ID}')
 
-        # Call the API
         try:
-            response = authed_session.get(list_apps_url)
+            response = authed_session.post(CREATE_APP_URL, json=payload)
             response.raise_for_status()
-            apps = response.json()
-        except requests.exceptions.HTTPError as e:
-            print(f'Error listing the Android apps: {e}')
-            exit(1)
+            print(f'Successfully created the Android app with ID/package name: {app_id} and Display name: {display_name}')
 
-        # Add the apps from the current page to the all_apps list
-        all_apps.extend(apps['apps'])
+            # Open Firebase project page in browser
+            webbrowser.open(FIREBASE_PROJECT_URL)
+        except requests.exceptions.HTTPError as e:
+            if e.response.status_code == 409:
+                print(f'The Android app with ID/package name: {app_id} already exists in the Firebase project.')
+            else:
+                print(f'Error creating the Android app: {e}')
+                exit(1)
+    elif args.list:
+        # Initialize an empty list to store all apps
+        all_apps = []
+
+        # Initialize nextPageToken to None for the first API call
+        next_page_token = None
+
+        while True:
+            # Create the API URL with the nextPageToken parameter if it is not None
+            list_apps_url = LIST_APPS_URL
+            if next_page_token is not None:
+                list_apps_url += f'?pageToken={next_page_token}'
+
+            # Call the API
+            try:
+                response = authed_session.get(list_apps_url)
+                response.raise_for_status()
+                apps = response.json()
+            except requests.exceptions.HTTPError as e:
+                print(f'Error listing the Android apps: {e}')
+                exit(1)
+
+            # Add the apps from the current page to the all_apps list
+            all_apps.extend(apps['apps'])
+
+            # If a nextPageToken is present in the response, set it for the next API call
+            if 'nextPageToken' in apps:
+                next_page_token = apps['nextPageToken']
+            else:
+                # If no nextPageToken is present, we have fetched all apps, so we break the loop
+                break
+
+        # Now all_apps contains all Android apps in the project
+        for app in all_apps:
+            display_name = app.get('displayName', 'No display name')
+            print(f'  - {display_name} ({app["packageName"]})')
 
-        # If a nextPageToken is present in the response, set it for the next API call
-        if 'nextPageToken' in apps:
-            next_page_token = apps['nextPageToken']
-        else:
-            # If no nextPageToken is present, we have fetched all apps, so we break the loop
-            break
-
-    # Now all_apps contains all Android apps in the project
-    for app in all_apps:
-        display_name = app.get('displayName', 'No display name')
-        print(f'  - {display_name} ({app["packageName"]})')
+if __name__ == "__main__":
+    main()
```

### Comparing `firegs-0.7/firegs.egg-info/PKG-INFO` & `firegs-0.8/firegs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: firegs
-Version: 0.7
+Version: 0.8
 Summary: A tool to add app to Firebase project from the command line
 Home-page: https://github.com/androiddevnotes/firegs
 Author: Android Dev Notes
 Author-email: awesomedevnotes@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
```

### Comparing `firegs-0.7/setup.py` & `firegs-0.8/setup.py`

 * *Files identical despite different names*

