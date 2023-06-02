# Comparing `tmp/liveports-0.1.3.tar.gz` & `tmp/liveports-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "liveports-0.1.3.tar", last modified: Fri Jun  2 22:07:49 2023, max compression
+gzip compressed data, was "liveports-0.1.4.tar", last modified: Fri Jun  2 22:49:48 2023, max compression
```

## Comparing `liveports-0.1.3.tar` & `liveports-0.1.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-02 22:07:49.350569 liveports-0.1.3/
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      212 2023-06-02 22:07:49.350569 liveports-0.1.3/PKG-INFO
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-02 22:07:49.350569 liveports-0.1.3/liveports/
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)        0 2023-06-02 16:32:43.000000 liveports-0.1.3/liveports/__init__.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     3327 2023-06-02 16:38:40.000000 liveports-0.1.3/liveports/blaster_utils.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     5942 2023-06-02 22:01:34.000000 liveports-0.1.3/liveports/client.py
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-02 22:07:49.350569 liveports-0.1.3/liveports.egg-info/
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      212 2023-06-02 22:07:49.000000 liveports-0.1.3/liveports.egg-info/PKG-INFO
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      277 2023-06-02 22:07:49.000000 liveports-0.1.3/liveports.egg-info/SOURCES.txt
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)        1 2023-06-02 22:07:49.000000 liveports-0.1.3/liveports.egg-info/dependency_links.txt
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       53 2023-06-02 22:07:49.000000 liveports-0.1.3/liveports.egg-info/entry_points.txt
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       17 2023-06-02 22:07:49.000000 liveports-0.1.3/liveports.egg-info/requires.txt
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       10 2023-06-02 22:07:49.000000 liveports-0.1.3/liveports.egg-info/top_level.txt
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       38 2023-06-02 22:07:49.350569 liveports-0.1.3/setup.cfg
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      400 2023-06-02 22:03:35.000000 liveports-0.1.3/setup.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-02 22:49:48.582609 liveports-0.1.4/
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      212 2023-06-02 22:49:48.582609 liveports-0.1.4/PKG-INFO
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-02 22:49:48.582609 liveports-0.1.4/liveports/
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)        0 2023-06-02 16:32:43.000000 liveports-0.1.4/liveports/__init__.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     3327 2023-06-02 16:38:40.000000 liveports-0.1.4/liveports/blaster_utils.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     6266 2023-06-02 22:49:22.000000 liveports-0.1.4/liveports/client.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-02 22:49:48.582609 liveports-0.1.4/liveports.egg-info/
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      212 2023-06-02 22:49:48.000000 liveports-0.1.4/liveports.egg-info/PKG-INFO
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      277 2023-06-02 22:49:48.000000 liveports-0.1.4/liveports.egg-info/SOURCES.txt
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)        1 2023-06-02 22:49:48.000000 liveports-0.1.4/liveports.egg-info/dependency_links.txt
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       53 2023-06-02 22:49:48.000000 liveports-0.1.4/liveports.egg-info/entry_points.txt
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       17 2023-06-02 22:49:48.000000 liveports-0.1.4/liveports.egg-info/requires.txt
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       10 2023-06-02 22:49:48.000000 liveports-0.1.4/liveports.egg-info/top_level.txt
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       38 2023-06-02 22:49:48.582609 liveports-0.1.4/setup.cfg
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      400 2023-06-02 22:46:51.000000 liveports-0.1.4/setup.py
```

### Comparing `liveports-0.1.3/liveports/blaster_utils.py` & `liveports-0.1.4/liveports/blaster_utils.py`

 * *Files identical despite different names*

### Comparing `liveports-0.1.3/liveports/client.py` & `liveports-0.1.4/liveports/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,17 +21,18 @@
 ssl_context.verify_mode = ssl.CERT_NONE
 
 socketserver.TCPServer.allow_reuse_address = True
 
 # Process command line arguments
 
 # If request logging enabled, we will use a proxy server to log request/response
+NO_PROXY = bool(CommandLineArgs.get("noproxy", False))
 LOG_VIEWER_PORT = int(CommandLineArgs.get("logViewerPort", 4061))
 LOCAL_PROXY_PORT = int(CommandLineArgs.get("proxyPort", 4060))
-
+DEBUG_LOG_LEVEL = int(CommandLineArgs.get("logLevel", 0))
 # target
 TARGET_PORT = int(CommandLineArgs.get("port") or CommandLineArgs["args"][-1])
 TARGET_PROTOCOL = ((len(CommandLineArgs["args"]) > 1 and CommandLineArgs["args"][1]) or "http").lower()
 if(TARGET_PROTOCOL not in ["http", "https"]):
 	print("Invalid protocol: must be one of http/https", TARGET_PROTOCOL)
 	sys.exit(1)
 
@@ -70,16 +71,17 @@
 			log_viewer_server.handle_request()
 		cls.log_viewer_server = None
 
 	@staticmethod
 	def ssh_reverse_proxy(server_hostname, server_port, password):
 		open("echo_pass", "w").write(f"#!/bin/bash\necho \"{password}\"\n")
 		run_shell("chmod +x echo_pass", shell=True)
+		proxy_port = TARGET_PORT if NO_PROXY else LOCAL_PROXY_PORT
 		run_shell(
-			f"ssh -o ServerAliveInterval=60 -NR {server_port}:localhost:{LOCAL_PROXY_PORT} proxyuser@{server_hostname}",
+			f"ssh -o ServerAliveInterval=60 -NR {server_port}:localhost:{proxy_port} proxyuser@{server_hostname}",
 			shell=True,
 			env={"SSH_ASKPASS": os.path.abspath("echo_pass"), "DISPLAY": "xxx"},
 			state=Client.ssh_proc,
 			preexec_fn=os.setsid
 		)
 		Client.is_running = False
 
@@ -164,14 +166,15 @@
 			fcntl.flock(cache_file.fileno(), fcntl.LOCK_EX)
 
 			prev_resp = cache.get(SOURCE) or {}
 			server_hostname = prev_resp.get("server_hostname") or "ports.live"
 			resp = requests.post(
 				"https://" + server_hostname + "/api/register",
 				json={
+					"protocol": TARGET_PROTOCOL if NO_PROXY else "http",
 					"source": SOURCE,
 					"api_key": CommandLineArgs.get("api_key", prev_resp.get("api_key"))
 				}
 			).json()
 			# update the previously cached data and cache it
 			prev_resp.update(resp)
 			cache[SOURCE] = resp
@@ -183,31 +186,33 @@
 				sys.exit(1)
 
 			print(f'Your public hostname is: https://{resp["public_hostname"]}')
 
 			server_threads = []
 
 			# START LOGVIEWER SERVER
-			log_viewer_server = threading.Thread(target=Client.start_log_viewer)
-			log_viewer_server.start()
-			server_threads.append(log_viewer_server)
-
-			# START PROXYSERVER
-			proxy_server = threading.Thread(target=Client.start_proxy_server)
-			proxy_server.start()
-			server_threads.append(proxy_server)
+			if(not NO_PROXY):
+				log_viewer_server = threading.Thread(target=Client.start_log_viewer)
+				log_viewer_server.start()
+				server_threads.append(log_viewer_server)
+
+				# START PROXYSERVER
+				proxy_server = threading.Thread(target=Client.start_proxy_server)
+				proxy_server.start()
+				server_threads.append(proxy_server)
 
 			# START SSH REVERSE PROXY
 			Client.ssh_reverse_proxy(resp["server_hostname"], resp["server_port"], resp["password"])
 
 			# WAIT FOR ALL THREADS STOPPED
 			for _thread in server_threads:
 				_thread.join()
 
 		except Exception as ex:
+			DEBUG_LOG_LEVEL > 1 and print("Encountered an exception ", str(ex))
 			sys.exit(1)
 		finally:
 			fcntl.flock(cache_file.fileno(), fcntl.LOCK_UN)
 			cache_file.close()
 
 
 if __name__ == '__main__':
```

