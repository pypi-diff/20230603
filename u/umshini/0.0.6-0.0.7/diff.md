# Comparing `tmp/umshini-0.0.6.tar.gz` & `tmp/umshini-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "umshini-0.0.6.tar", last modified: Tue Mar 14 17:13:06 2023, max compression
+gzip compressed data, was "umshini-0.0.7.tar", last modified: Sat Jun  3 01:06:54 2023, max compression
```

## Comparing `umshini-0.0.6.tar` & `umshini-0.0.7.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 hannah     (501) staff       (20)        0 2023-03-14 17:13:06.118056 umshini-0.0.6/
--rw-r--r--   0 hannah     (501) staff       (20)    34629 2023-03-14 14:07:32.000000 umshini-0.0.6/LICENSE
--rw-r--r--   0 hannah     (501) staff       (20)    40768 2023-03-14 17:13:06.117872 umshini-0.0.6/PKG-INFO
--rw-r--r--   0 hannah     (501) staff       (20)      258 2022-07-15 14:57:42.000000 umshini-0.0.6/README.md
-drwxr-xr-x   0 hannah     (501) staff       (20)        0 2023-03-14 17:13:06.108255 umshini-0.0.6/Umshini/
--rw-r--r--   0 hannah     (501) staff       (20)       34 2022-07-15 14:57:42.000000 umshini-0.0.6/Umshini/__init__.py
-drwxr-xr-x   0 hannah     (501) staff       (20)        0 2023-03-14 17:13:06.111908 umshini-0.0.6/Umshini/envs/
--rw-r--r--   0 hannah     (501) staff       (20)       55 2023-03-14 14:07:42.000000 umshini-0.0.6/Umshini/envs/__init__.py
--rw-r--r--   0 hannah     (501) staff       (20)     2284 2023-03-14 14:07:42.000000 umshini-0.0.6/Umshini/envs/envs_list.py
--rw-r--r--   0 hannah     (501) staff       (20)     2820 2023-03-14 14:07:42.000000 umshini-0.0.6/Umshini/example_client.py
--rw-r--r--   0 hannah     (501) staff       (20)     1560 2023-03-14 14:07:32.000000 umshini-0.0.6/Umshini/learner.py
--rw-r--r--   0 hannah     (501) staff       (20)    14723 2023-03-14 15:37:37.000000 umshini-0.0.6/Umshini/tournament_client.py
-drwxr-xr-x   0 hannah     (501) staff       (20)        0 2023-03-14 17:13:06.116163 umshini-0.0.6/Umshini/utils/
--rw-r--r--   0 hannah     (501) staff       (20)        0 2023-01-03 15:46:12.000000 umshini-0.0.6/Umshini/utils/__init__.py
--rw-r--r--   0 hannah     (501) staff       (20)      529 2023-01-03 15:46:12.000000 umshini-0.0.6/Umshini/utils/compress.py
--rw-r--r--   0 hannah     (501) staff       (20)     1326 2023-01-03 15:46:12.000000 umshini-0.0.6/Umshini/utils/socket_wrap.py
--rw-r--r--   0 hannah     (501) staff       (20)      373 2023-01-03 15:46:12.000000 umshini-0.0.6/Umshini/utils/test_compression.py
--rw-r--r--   0 hannah     (501) staff       (20)      687 2023-03-14 14:07:42.000000 umshini-0.0.6/pyproject.toml
--rw-r--r--   0 hannah     (501) staff       (20)       38 2023-03-14 17:13:06.118100 umshini-0.0.6/setup.cfg
--rw-r--r--   0 hannah     (501) staff       (20)     1543 2023-03-14 14:07:42.000000 umshini-0.0.6/setup.py
-drwxr-xr-x   0 hannah     (501) staff       (20)        0 2023-03-14 17:13:06.117531 umshini-0.0.6/umshini.egg-info/
--rw-r--r--   0 hannah     (501) staff       (20)    40768 2023-03-14 17:13:06.000000 umshini-0.0.6/umshini.egg-info/PKG-INFO
--rw-r--r--   0 hannah     (501) staff       (20)      455 2023-03-14 17:13:06.000000 umshini-0.0.6/umshini.egg-info/SOURCES.txt
--rw-r--r--   0 hannah     (501) staff       (20)        1 2023-03-14 17:13:06.000000 umshini-0.0.6/umshini.egg-info/dependency_links.txt
--rw-r--r--   0 hannah     (501) staff       (20)      208 2023-03-14 17:13:06.000000 umshini-0.0.6/umshini.egg-info/requires.txt
--rw-r--r--   0 hannah     (501) staff       (20)        8 2023-03-14 17:13:06.000000 umshini-0.0.6/umshini.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 01:06:54.123701 umshini-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    34629 2023-06-03 01:06:45.000000 umshini-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    40723 2023-06-03 01:06:54.123701 umshini-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-03 01:06:45.000000 umshini-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 01:06:54.119701 umshini-0.0.7/Umshini/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-03 01:06:45.000000 umshini-0.0.7/Umshini/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 01:06:54.119701 umshini-0.0.7/Umshini/envs/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-03 01:06:45.000000 umshini-0.0.7/Umshini/envs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-06-03 01:06:45.000000 umshini-0.0.7/Umshini/envs/envs_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-06-03 01:06:45.000000 umshini-0.0.7/Umshini/example_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-06-03 01:06:45.000000 umshini-0.0.7/Umshini/learner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14858 2023-06-03 01:06:45.000000 umshini-0.0.7/Umshini/tournament_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 01:06:54.119701 umshini-0.0.7/Umshini/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 01:06:45.000000 umshini-0.0.7/Umshini/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-06-03 01:06:45.000000 umshini-0.0.7/Umshini/utils/compress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-06-03 01:06:45.000000 umshini-0.0.7/Umshini/utils/socket_wrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-06-03 01:06:45.000000 umshini-0.0.7/Umshini/utils/test_compression.py
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-06-03 01:06:45.000000 umshini-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-03 01:06:54.123701 umshini-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-06-03 01:06:45.000000 umshini-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 01:06:54.123701 umshini-0.0.7/umshini.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    40723 2023-06-03 01:06:54.000000 umshini-0.0.7/umshini.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-03 01:06:54.000000 umshini-0.0.7/umshini.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 01:06:54.000000 umshini-0.0.7/umshini.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-03 01:06:54.000000 umshini-0.0.7/umshini.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-03 01:06:54.000000 umshini-0.0.7/umshini.egg-info/top_level.txt
```

### Comparing `umshini-0.0.6/LICENSE` & `umshini-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `umshini-0.0.6/PKG-INFO` & `umshini-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: umshini
-Version: 0.0.6
+Version: 0.0.7
 Summary: Umshini client for playing in MARL tournaments
 Home-page: https://github.com/umshini/umshini
 Author: umshini team
 Author-email: "Jordan K. Terry" <j.k.terry@swarmlabs.com>
 License: This code is copyright Jordan Terry, 2021, and is released under the GNU AGPLv3 license, included below:
         
                             GNU AFFERO GENERAL PUBLIC LICENSE
@@ -669,18 +669,16 @@
         For more information on this, and how to apply and follow the GNU AGPL, see
         <https://www.gnu.org/licenses/>.
         
 Project-URL: Homepage, https://github.com/umshini/umshini
 Keywords: Reinforcement Learning,game,RL,AI,gym
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Requires-Python: <3.10,>=3.6
+Requires-Python: >=3.6, <3.11
 Description-Content-Type: text/markdown
-Provides-Extra: atari
-Provides-Extra: classic
 License-File: LICENSE
 
 # Colosseum
 
 To run the Colosseum server for testing, refer to [the server repo](https://github.com/PettingZoo-Team/Colosseum-Server).
 
 To run one or multiple clients you can use the following command:
```

### Comparing `umshini-0.0.6/Umshini/example_client.py` & `umshini-0.0.7/Umshini/example_client.py`

 * *Files identical despite different names*

### Comparing `umshini-0.0.6/Umshini/learner.py` & `umshini-0.0.7/Umshini/learner.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,27 +5,30 @@
 
 def create_and_run(botname, user_key):
     agent = ColosseumTournamentAgent(maximum_rounds=100)
     agent.connect(botname, user_key)
     agent.run()
 
 
-def connect(environment, botname, user_key, user_policy, debug=False):
+def connect(environment, botname, user_key, user_policy, debug=False, testing=False):
     """
     User end function to add their RL policy
 
     Passed function accepts parameters:
         policy(observation, reward, done, info)
 
     Passed function returns action
     """
-    agent = ColosseumTournamentAgent(policy=user_policy, games=[environment], maximum_rounds=100, host="34.70.234.149",
-                                     port="8803", debug=debug)
-    #agent = ColosseumTournamentAgent(policy=user_policy, games=[environment],
-    #                                 maximum_rounds=100, debug=debug)
+    if testing:
+        agent = ColosseumTournamentAgent(policy=user_policy, games=[environment], maximum_rounds=100, host="127.0.0.1",
+                                         port="8803", debug=debug)
+    else:
+        agent = ColosseumTournamentAgent(policy=user_policy, games=[environment], maximum_rounds=100, host="34.70.234.149",
+                                        port="8803", debug=debug)
+
     agent.connect(botname, user_key)
     agent.run()
 
 
 def test(environment, user_policy):
     test_env = TestEnv(environment)
     term = trunc = False
```

### Comparing `umshini-0.0.6/Umshini/tournament_client.py` & `umshini-0.0.7/Umshini/tournament_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,17 +13,18 @@
 
 # Send JSON through socket
 def send_json(sock, data):
     return sock.sendall(json.dumps(data).encode("utf-8"))
 
 
 # Receive JSON from socket
-def recv_json(sock, timeout=60 * 15):
+def recv_json(sock, timeout=30):
     sock.settimeout(timeout)
     data = sock.recv(2 ** 30)  # Arbitrarily large buffer
+    sock.settimeout(30)
     return data
 
 
 class NetworkEnv(gym.Env):
     def __init__(self, env_id, seed, game_ip, game_port, username, token, verbose=0):
         self.verbose = verbose
         if self.verbose > 0:
@@ -120,14 +121,17 @@
         self.spinner.start()
         # Get initial observation
         if self.verbose > 1:
             print("receiving initial obs")
         observation_data = recv_json(self.game_connection)
         if self.verbose > 1:
             print("received initial obs")
+            print(observation_data)
+            if not observation_data:
+                print("No data received")
         if observation_data["type"] != "observation":
             # Game is done
             return self.obs
 
         # Unpack observation
         obs = decompress(observation_data["data"][self.agent])
         self.obs = obs
@@ -152,16 +156,16 @@
         self.was_trunc = False
         self.obss = None
 
     def reset(self):
         self.num_steps = 0
         self.was_term = False
         self.was_trunc = False
-        obss = self.env.reset()
-        return obss[self.agent]
+        obss, info = self.env.reset()
+        return obss, info
 
     def step(self, action):
         assert not self.was_term and not self.was_trunc, "stepped after term or trunc, should terminate loop"
 
         # Set random actions for all other agents in parallel game or None in turn-based game
         actions = {
             agent: (None if self.turn_based else self.env.action_space(agent).sample()) for agent in self.env.agents
@@ -270,15 +274,15 @@
         self.current_match = 0
         self._test_environments()
 
     # Test agent in every game
     def _test_environments(self):
         for game in self.available_games:
             test_env = TestEnv(game)
-            obs = test_env.reset()
+            obs, info = test_env.reset()
             for _ in range(100):
                 if (obs is not None
                     and isinstance(obs, dict)
                     and obs and "action_mask" in obs):
                     action = np.random.choice(obs["action_mask"].nonzero()[0])
                 else:
                     action = test_env.action_space.sample()
@@ -292,15 +296,15 @@
         if self.tournament_completed:
             return None
 
         # Receive game server info from matchmaker
         spinner = Halo(text='Waiting for players', text_color='cyan', color='green', spinner='dots')
         spinner.start()
         try:
-            ready_data = recv_json(self.main_connection, timeout=60 * 15)
+            ready_data = recv_json(self.main_connection, timeout=60)
         except TimeoutError as err:
             print("Not enough players to start tournament.", flush=True)
             raise err
         spinner.succeed()
 
         if self.debug:
             print(ready_data)
```

### Comparing `umshini-0.0.6/Umshini/utils/compress.py` & `umshini-0.0.7/Umshini/utils/compress.py`

 * *Files identical despite different names*

### Comparing `umshini-0.0.6/Umshini/utils/socket_wrap.py` & `umshini-0.0.7/Umshini/utils/socket_wrap.py`

 * *Files identical despite different names*

### Comparing `umshini-0.0.6/pyproject.toml` & `umshini-0.0.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel", "numpy>=1.19.0", "Cython>=0.29.21"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "umshini"
-version = "0.0.6"
+version = "0.0.7"
 readme = "README.md"
 description = "Umshini client for playing in MARL tournaments"
 authors = [{ name = "Jordan K. Terry", email = "j.k.terry@swarmlabs.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
```

### Comparing `umshini-0.0.6/setup.py` & `umshini-0.0.7/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,49 +1,41 @@
 from setuptools import find_packages, setup
 
-VERSION = '0.0.6'
+VERSION = '0.0.7'
 DESCRIPTION = 'Umshini Client API'
 with open("README.md", 'r') as f:
     long_description = f.read()
 
 setup(
     name='umshini',
     version=VERSION,
     author='umshini team',
     author_email="j.k.terry@swarmlabs.com",
     description=DESCRIPTION,
     url='https://github.com/umshini/umshini',
     #long_description=long_description,
     #long_description_content_type="text/markdown",
     #keywords=["Reinforcement Learning", "game", "RL", "AI", "gym"],
-    #python_requires=">=3.6, <3.10",
+    python_requires=">=3.6, <3.11",
     #data_files=[("", ["LICENSE.txt"])],
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
+        ''
         'Cython',
         'colorama',
-        'pettingzoo==1.22.3',
-        'supersuit==3.7.1',
-        'gymnasium',
-        'numpy',
-        'halo',
-    ],
-    setup_requires=[
-        'Cython',
-        'colorama',
-        'supersuit==3.7.1',
-        'pettingzoo==1.22.3',
+        'pettingzoo==1.23.0',
+        'pettingzoo[classic]==1.23.0',
+        'rlcard',
+        'supersuit==3.8.0',
         'gymnasium',
         'numpy',
         'halo',
     ],
     extras_require={
-        "atari": ['pettingzoo[atari]==1.22.3', 'autorom[accept-rom-license]', 'multi-agent-ale-py'],
-        "classic": ['pettingzoo[classic]==1.22.3', 'pygame', 'rlcard'],
     },
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
```

### Comparing `umshini-0.0.6/umshini.egg-info/PKG-INFO` & `umshini-0.0.7/umshini.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: umshini
-Version: 0.0.6
+Version: 0.0.7
 Summary: Umshini client for playing in MARL tournaments
 Home-page: https://github.com/umshini/umshini
 Author: umshini team
 Author-email: "Jordan K. Terry" <j.k.terry@swarmlabs.com>
 License: This code is copyright Jordan Terry, 2021, and is released under the GNU AGPLv3 license, included below:
         
                             GNU AFFERO GENERAL PUBLIC LICENSE
@@ -669,18 +669,16 @@
         For more information on this, and how to apply and follow the GNU AGPL, see
         <https://www.gnu.org/licenses/>.
         
 Project-URL: Homepage, https://github.com/umshini/umshini
 Keywords: Reinforcement Learning,game,RL,AI,gym
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Requires-Python: <3.10,>=3.6
+Requires-Python: >=3.6, <3.11
 Description-Content-Type: text/markdown
-Provides-Extra: atari
-Provides-Extra: classic
 License-File: LICENSE
 
 # Colosseum
 
 To run the Colosseum server for testing, refer to [the server repo](https://github.com/PettingZoo-Team/Colosseum-Server).
 
 To run one or multiple clients you can use the following command:
```

