# Comparing `tmp/mech_client-0.1.6.tar.gz` & `tmp/mech_client-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mech_client-0.1.6.tar", max compression
+gzip compressed data, was "mech_client-0.1.7.tar", max compression
```

## Comparing `mech_client-0.1.6.tar` & `mech_client-0.1.7.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0    11339 2023-05-27 20:23:22.952168 mech_client-0.1.6/LICENSE
--rw-r--r--   0        0        0     2037 2023-05-30 10:09:38.116752 mech_client-0.1.6/README.md
--rw-r--r--   0        0        0       22 2023-06-01 12:42:31.278538 mech_client-0.1.6/mech_client/__init__.py
--rw-r--r--   0        0        0     1147 2023-05-30 08:36:18.724247 mech_client-0.1.6/mech_client/cli.py
--rw-r--r--   0        0        0     7617 2023-06-01 12:41:57.849598 mech_client-0.1.6/mech_client/interact.py
--rw-r--r--   0        0        0     1779 2023-05-31 14:33:42.502514 mech_client-0.1.6/mech_client/prompt_to_ipfs.py
--rw-r--r--   0        0        0     1659 2023-05-31 14:33:42.503191 mech_client-0.1.6/mech_client/push_to_ipfs.py
--rw-r--r--   0        0        0      558 2023-06-01 12:42:33.054827 mech_client-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     2960 1970-01-01 00:00:00.000000 mech_client-0.1.6/setup.py
--rw-r--r--   0        0        0     2607 1970-01-01 00:00:00.000000 mech_client-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0    11339 2023-05-27 20:23:22.952168 mech_client-0.1.7/LICENSE
+-rw-r--r--   0        0        0     2037 2023-05-30 10:09:38.116752 mech_client-0.1.7/README.md
+-rw-r--r--   0        0        0       22 2023-06-03 09:13:28.534323 mech_client-0.1.7/mech_client/__init__.py
+-rw-r--r--   0        0        0     1514 2023-06-01 18:17:24.000853 mech_client-0.1.7/mech_client/cli.py
+-rw-r--r--   0        0        0     7617 2023-06-01 12:41:57.849598 mech_client-0.1.7/mech_client/interact.py
+-rw-r--r--   0        0        0     1779 2023-05-31 14:33:42.502514 mech_client-0.1.7/mech_client/prompt_to_ipfs.py
+-rw-r--r--   0        0        0     1659 2023-05-31 14:33:42.503191 mech_client-0.1.7/mech_client/push_to_ipfs.py
+-rw-r--r--   0        0        0     1993 2023-06-01 18:17:24.001121 mech_client-0.1.7/mech_client/to_png.py
+-rw-r--r--   0        0        0      581 2023-06-03 09:13:33.787570 mech_client-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     2960 1970-01-01 00:00:00.000000 mech_client-0.1.7/setup.py
+-rw-r--r--   0        0        0     2690 1970-01-01 00:00:00.000000 mech_client-0.1.7/PKG-INFO
```

### Comparing `mech_client-0.1.6/LICENSE` & `mech_client-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `mech_client-0.1.6/README.md` & `mech_client-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `mech_client-0.1.6/mech_client/cli.py` & `mech_client-0.1.7/mech_client/cli.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import click
 
 from mech_client import __version__
 from mech_client.interact import interact as interact_
 from mech_client.prompt_to_ipfs import main as prompt_to_ipfs_main
 from mech_client.push_to_ipfs import main as push_to_ipfs_main
+from mech_client.to_png import main as to_png_main
 
 
 @click.group(name="mechx")  # type: ignore
 @click.version_option(__version__, prog_name="mechx")
 def cli() -> None:
     """Command-line tool for interacting with mechs."""
 
@@ -31,14 +32,24 @@
 @click.command()
 @click.argument("file_path")
 def push_to_ipfs(file_path: str) -> None:
     """Upload a file to IPFS."""
     push_to_ipfs_main(file_path=file_path)
 
 
+@click.command()
+@click.argument("ipfs_hash")
+@click.argument("path")
+@click.argument("request_id")
+def to_png(ipfs_hash: str, path: str, request_id: str) -> None:
+    """Convert a stability AI API's diffusion model output into a PNG format."""
+    to_png_main(ipfs_hash, path, request_id)
+
+
 cli.add_command(interact)
 cli.add_command(prompt_to_ipfs)
 cli.add_command(push_to_ipfs)
+cli.add_command(to_png)
 
 
 if __name__ == "__main__":
     cli()
```

### Comparing `mech_client-0.1.6/mech_client/interact.py` & `mech_client-0.1.7/mech_client/interact.py`

 * *Files identical despite different names*

### Comparing `mech_client-0.1.6/mech_client/prompt_to_ipfs.py` & `mech_client-0.1.7/mech_client/prompt_to_ipfs.py`

 * *Files identical despite different names*

### Comparing `mech_client-0.1.6/mech_client/push_to_ipfs.py` & `mech_client-0.1.7/mech_client/push_to_ipfs.py`

 * *Files identical despite different names*

### Comparing `mech_client-0.1.6/pyproject.toml` & `mech_client-0.1.7/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 [tool.poetry]
 name = "mech-client"
-version = "0.1.6"
+version = "0.1.7"
 description = "Basic client to interact with a mech"
 authors = ["David Minarsch <david.minarsch@googlemail.com>"]
 readme = "README.md"
 packages = [{include = "mech_client"}]
+license = "Apache-2.0"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 open-aea = {version = "1.34.0", extras = ["cli"]}
 open-aea-ledger-ethereum = "1.34.0"
 open-aea-cli-ipfs = "1.34.0"
 websocket-client = ">=0.32.0,<1"
```

### Comparing `mech_client-0.1.6/setup.py` & `mech_client-0.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
  'websocket-client>=0.32.0,<1']
 
 entry_points = \
 {'console_scripts': ['mechx = mech_client.cli:cli']}
 
 setup_kwargs = {
     'name': 'mech-client',
-    'version': '0.1.6',
+    'version': '0.1.7',
     'description': 'Basic client to interact with a mech',
     'long_description': '# mech-client\nBasic client to interact with a mech\n\n> **Warning**<br />\n> **This is a hacky alpha version of the client - don\'t rely on it as production software.**\n\n## Installation\n\n```bash\npip install mech-client\n```\n\nThen, set a websocket endpoint for Gnosis RPC like so:\n\n```bash\nexport WEBSOCKET_ENDPOINT=<YOUR ENDPOINT>\n```\n\n## CLI:\n\n```bash\nUsage: mechx [OPTIONS] COMMAND [ARGS]...\n\n  Command-line tool for interacting with mechs.\n\nOptions:\n  --version  Show the version and exit.\n  --help     Show this message and exit.\n\nCommands:\n  interact        Interact with a mech specifying a prompt and tool.\n  prompt-to-ipfs  Upload a prompt and tool to IPFS as metadata.\n  push-to-ipfs    Upload a file to IPFS.\n ```\n\n## Usage:\n\nFirst, create a private key in file `ethereum_private_key.txt` with this command:\n\n```bash\naea generate-key ethereum\n```\n\nEnsure the private key carries funds on Gnosis Chain.\n\nSecond, run the following command to instruct the mech with `<prompt>` and `<tool>`:\n\n```bash\nmechx interact <prompt> <tool>\n```\n\nExample output:\n```bash\nmechx interact "write a short poem" "openai-text-davinci-003"\nPrompt uploaded: https://gateway.autonolas.tech/ipfs/f01701220ad9e2d5698fbd6c3a4ce61f329590e68a23181772669e543e69decdae316423b\nTransaction sent: https://gnosisscan.io/tx/0xb3a17ef90da6cc7a86e008a3a91bd367d573b406eae53405a4aa981001a5eaf3\nRequest on-chain with id: 15263135923206312300456917202469137903009897852865973093832667165921851537677\nData arrived: https://gateway.autonolas.tech/ipfs/f017012205053a4ae3ef0cf4ed7eff0c2d74dbaf3479fbdeb292472560e7bfaa4cfecfcdc\nData: {\'requestId\': 15263135923206312300456917202469137903009897852865973093832667165921851537677, \'result\': "\\n\\nA sun-filled sky,\\nA soft breeze blowing by,\\nWhere the trees sway in the wind,\\nA peaceful moment I can\'t rewind."}\n```\n\n## Release guide:\n\nFinish edits, bump versions in `pyproject.toml` and `mech_client/__init__.py`, then `poetry lock`, then `rm -rf dist`, then `poetry publish --build --username=<username> --password=<password>`.',
     'author': 'David Minarsch',
     'author_email': 'david.minarsch@googlemail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `mech_client-0.1.6/PKG-INFO` & `mech_client-0.1.7/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: mech-client
-Version: 0.1.6
+Version: 0.1.7
 Summary: Basic client to interact with a mech
+License: Apache-2.0
 Author: David Minarsch
 Author-email: david.minarsch@googlemail.com
 Requires-Python: >=3.10,<4.0
+Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: open-aea-cli-ipfs (==1.34.0)
 Requires-Dist: open-aea-ledger-ethereum (==1.34.0)
 Requires-Dist: open-aea[cli] (==1.34.0)
 Requires-Dist: websocket-client (>=0.32.0,<1)
```

