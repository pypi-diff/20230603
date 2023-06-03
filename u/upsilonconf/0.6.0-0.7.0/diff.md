# Comparing `tmp/upsilonconf-0.6.0.tar.gz` & `tmp/upsilonconf-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "upsilonconf-0.6.0.tar", last modified: Mon Oct 31 16:54:37 2022, max compression
+gzip compressed data, was "upsilonconf-0.7.0.tar", last modified: Sat Jun  3 09:50:51 2023, max compression
```

## Comparing `upsilonconf-0.6.0.tar` & `upsilonconf-0.7.0.tar`

### file list

```diff
@@ -1,24 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 16:54:37.334399 upsilonconf-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1073 2022-10-31 16:54:26.000000 upsilonconf-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     5846 2022-10-31 16:54:37.334399 upsilonconf-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5158 2022-10-31 16:54:26.000000 upsilonconf-0.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-10-31 16:54:26.000000 upsilonconf-0.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      812 2022-10-31 16:54:37.338399 upsilonconf-0.6.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 16:54:37.334399 upsilonconf-0.6.0/upsilonconf/
--rw-r--r--   0 runner    (1001) docker     (121)      366 2022-10-31 16:54:26.000000 upsilonconf-0.6.0/upsilonconf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    17763 2022-10-31 16:54:26.000000 upsilonconf-0.6.0/upsilonconf/config.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 16:54:37.334399 upsilonconf-0.6.0/upsilonconf/io/
--rw-r--r--   0 runner    (1001) docker     (121)     4669 2022-10-31 16:54:26.000000 upsilonconf-0.6.0/upsilonconf/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2150 2022-10-31 16:54:26.000000 upsilonconf-0.6.0/upsilonconf/io/_optional_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (121)     6727 2022-10-31 16:54:26.000000 upsilonconf-0.6.0/upsilonconf/io/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     3896 2022-10-31 16:54:26.000000 upsilonconf-0.6.0/upsilonconf/io/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     3821 2022-10-31 16:54:26.000000 upsilonconf-0.6.0/upsilonconf/io/directory.py
--rw-r--r--   0 runner    (1001) docker     (121)     1345 2022-10-31 16:54:26.000000 upsilonconf-0.6.0/upsilonconf/io/json.py
--rw-r--r--   0 runner    (1001) docker     (121)      878 2022-10-31 16:54:26.000000 upsilonconf-0.6.0/upsilonconf/io/toml.py
--rw-r--r--   0 runner    (1001) docker     (121)     2148 2022-10-31 16:54:26.000000 upsilonconf-0.6.0/upsilonconf/io/yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 16:54:37.334399 upsilonconf-0.6.0/upsilonconf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5846 2022-10-31 16:54:37.000000 upsilonconf-0.6.0/upsilonconf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      472 2022-10-31 16:54:37.000000 upsilonconf-0.6.0/upsilonconf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-31 16:54:37.000000 upsilonconf-0.6.0/upsilonconf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       45 2022-10-31 16:54:37.000000 upsilonconf-0.6.0/upsilonconf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-10-31 16:54:37.000000 upsilonconf-0.6.0/upsilonconf.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 09:50:51.002443 upsilonconf-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-03 09:50:41.000000 upsilonconf-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5476 2023-06-03 09:50:51.002443 upsilonconf-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4703 2023-06-03 09:50:41.000000 upsilonconf-0.7.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-03 09:50:41.000000 upsilonconf-0.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-06-03 09:50:51.006443 upsilonconf-0.7.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 09:50:51.002443 upsilonconf-0.7.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    97268 2023-06-03 09:50:41.000000 upsilonconf-0.7.0/tests/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 09:50:51.002443 upsilonconf-0.7.0/upsilonconf/
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-03 09:50:41.000000 upsilonconf-0.7.0/upsilonconf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35473 2023-06-03 09:50:41.000000 upsilonconf-0.7.0/upsilonconf/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 09:50:51.002443 upsilonconf-0.7.0/upsilonconf/io/
+-rw-r--r--   0 runner    (1001) docker     (123)     4924 2023-06-03 09:50:41.000000 upsilonconf-0.7.0/upsilonconf/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-06-03 09:50:41.000000 upsilonconf-0.7.0/upsilonconf/io/_optional_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12273 2023-06-03 09:50:41.000000 upsilonconf-0.7.0/upsilonconf/io/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3920 2023-06-03 09:50:41.000000 upsilonconf-0.7.0/upsilonconf/io/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3976 2023-06-03 09:50:41.000000 upsilonconf-0.7.0/upsilonconf/io/directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-06-03 09:50:41.000000 upsilonconf-0.7.0/upsilonconf/io/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-06-03 09:50:41.000000 upsilonconf-0.7.0/upsilonconf/io/toml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-06-03 09:50:41.000000 upsilonconf-0.7.0/upsilonconf/io/yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 09:50:51.002443 upsilonconf-0.7.0/upsilonconf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5476 2023-06-03 09:50:50.000000 upsilonconf-0.7.0/upsilonconf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-06-03 09:50:50.000000 upsilonconf-0.7.0/upsilonconf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 09:50:50.000000 upsilonconf-0.7.0/upsilonconf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-03 09:50:50.000000 upsilonconf-0.7.0/upsilonconf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-03 09:50:50.000000 upsilonconf-0.7.0/upsilonconf.egg-info/top_level.txt
```

### Comparing `upsilonconf-0.6.0/LICENSE` & `upsilonconf-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `upsilonconf-0.6.0/PKG-INFO` & `upsilonconf-0.7.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,193 +1,215 @@
 Metadata-Version: 2.1
 Name: upsilonconf
-Version: 0.6.0
+Version: 0.7.0
 Summary: A simple configuration library
 Home-page: https://github.com/hoedt/upsilonconf
 Author: Pieter-Jan Hoedt
 Author-email: hoedt@ml.jku.at
+Project-URL: Documentation, https://hoedt.github.io/upsilonconf
 Project-URL: Bug Tracker, https://github.com/hoedt/upsilonconf/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Utilities
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Provides-Extra: YAML
 Provides-Extra: TOML
+Provides-Extra: DOCS
 License-File: LICENSE
 
 # UpsilonConf
 
 UpsilonConf is a simple configuration library written in Python.
-It might not be really obvious, but this library is inspired by the great [OmegaConf](https://github.com/omry/omegaconf) library.
-OmegaConf is also the backbone for the more advanced [Hydra](https://hydra.cc/) framework.
-Concretely, the idea of this library is to provide an alternative to OmegaConf without the overhead of the variable interpolation (especially the `antlr` dependency).
-It is also very similar to the (discontinued) [AttrDict](https://github.com/bcj/AttrDict) library.
-In the meantime, there is also the [ml_collections](https://github.com/google/ml_collections) library, which seems to build on similar ideas as this project.
 
-Nevertheless, I decided to release upsilonconf because there might be a few features that people might find interesting/useful:
+A few features that you might find interesting/useful:
  - dict-like configuration object with attribute access (cf. `attrdict`)
  - hierarchical indexing by means of tuples or *dot-strings* (cf. `omegaconf`)
- - overwriting protection to prevent unexplainable bugs
  - read from/write to various file formats
  - use hierarchical configs with options (cf. config groups in `hydra`)
  - retrieve and manipulate config using CLI (cf. `omegaconf`)
  - minimal dependencies (cf. `attrdict`)
+ - configs with overwriting protection to prevent unexplainable bugs
 
-The name is inspired by OmegaConf.
-I decided to go for the Greek letter [Upsilon](https://en.wikipedia.org/wiki/Upsilon) because it is the first letter of [ὑπέρ (hupér)](https://en.wiktionary.org/wiki/ὑπέρ).
-This again comes from the fact that this library should mainly help me with managing _hyper_-parameters in neural networks.
+[![pypi badge](https://img.shields.io/pypi/v/upsilonconf?label=PyPI)](https://pypi.org/project/upsilonconf)
+[![conda badge](https://img.shields.io/conda/v/hoedt/upsilonconf)](https://anaconda.org/hoedt/upsilonconf)
+[![docs badge](https://img.shields.io/github/actions/workflow/status/hoedt/upsilonconf/sphinx.yml?branch=main&label=docs&logo=github)](https://hoedt.github.io/upsilonconf)
+[![licencse badge](https://img.shields.io/github/license/hoedt/upsilonconf)](https://github.com/hoedt/upsilonconf/blob/main/LICENSE)
+
+---
 
 ### How to install
 
-Using `pip` to install from [PyPI](https://pypi.org/project/upsilonconf/):
+Using `pip` to install from PyPI:
 
 ```shell
 python -m pip install upsilonconf
 ```
 
-or, to install the (optional) dependencies (`pyyaml`) for YAML IO
+Optional dependencies (e.g. `pyyaml`) can be included using
 
 ```shell
 python -m pip install upsilonconf[YAML]
 ```
 
-Using `conda` to install from [Anaconda](https://anaconda.org/hoedt/upsilonconf):
+Using `conda` to install from Anaconda:
 
 ```shell
 conda install hoedt::upsilonconf
 ```
 
 Optional dependencies (e.g. `pyyaml`) have to be installed separately.
 
 ---
 
 ### How to Use
 
 ```python
-import upsilonconf
+>>> import upsilonconf
+>>> from upsilonconf import PlainConfiguration as Configuration
 ```
 
-###### creation
+###### Creation
+
+load config from file
 
 ```python
-conf1 = upsilonconf.load("config.yaml")  # from config file
-conf2 = upsilonconf.Configuration(key1="value1", key2=2)  # direct
-dictionary = {"sub": conf2}  # sub-configs allowed!
-conf3 = upsilonconf.Configuration(**dictionary)  # from dict
-free_dict = {"a key": "with whitespace"}
-confX = upsilonconf.Configuration.from_dict(free_dict, key_mods={" ": "_"})
-conf = conf1 | conf2 | conf3  # from other configurations
+>>> conf = upsilonconf.load("my_config.yml")
 ```
 
-###### indexing
+or directly create config object
 
 ```python
-# getters
-conf["key1"] == conf.key1
-conf.key2 == conf["sub", "key2"]
-conf["sub", "key1"] == conf["sub.key1"]
-conf["sub.key2"] == conf.sub.key2
+>>> conf = Configuration(key1="value1", sub={"key1": 1, "key2": 2})
+```
 
-# setters
-conf["new_key"] = "new_value"
-conf.other_key = "other_value"
-conf.sub2 = {"a": .1, "b": 2}
-conf["sub2", "c"] = 3.
-conf["sub2.d"] = -4
+###### Indexing
 
-# and deleters...
-del conf["sub2.c"]
+Access values the way you like
+
+```python
+>>> assert conf["key1"] == conf.key1
+>>> assert conf.sub.key2 == conf["sub", "key2"]
+>>> assert conf["sub", "key1"] == conf["sub.key1"]
+>>> assert conf["sub.key2"] == conf.sub.key2
 ```
 
-###### overwrite protection
+###### Cool Tricks
+
+unpack configurations to function arguments
 
 ```python
-try:
-    conf["key1"] = "overwrite1"
-except ValueError:
-    print("overwriting")
-    conf.overwrite("key1", "overwrite1")
+>>> def test(key1, key2):
+...    return key1 + key2
+>>> test(**conf.sub)
+3
+```
 
-try:
-    conf.key1 = "overwrite2"
-except AttributeError:
-    print("overwriting")
-    conf.overwrite("key1", "overwrite2")
+convert config to flat `dict`
 
-try:
-    conf.update(key1="overwrite3")
-except ValueError:
-    print("overwriting")
-    conf.overwrite_all(key1="overwrite3")
+```python
+>>> conf.to_dict(flat=True)
+{'key1': 'value1', 'sub.key1': 1, 'sub.key2': 2}
 ```
 
+merge configurations with `|`
+
+```python
+>>> merged = conf | {"sub.key2": 3, "sub.key3": 2}
+>>> merged.sub.key2
+3
+>>> merged.sub.key3
+2
+```
+
+More details can be found in the [documentation](https://hoedt.github.io/upsilonconf)
+
 ###### flexible I/O
 
+support for different file formats
+
 ```python
-# different file formats (with optional requirements)
-conf = upsilonconf.load("config.yaml")  # with patched float parsing
-upsilonconf.save(conf, "config.json")  # with indentation by default
+>>> conf = upsilonconf.load("config.yaml")  # with patched float parsing
+>>> upsilonconf.save(conf, "config.json")  # with indentation by default
 ```
 
+transform non-identifier keys in files on-the-fly
+
 ```python
-# fix invalid keys in files on-the-fly
-conf = upsilonconf.load("config.yaml", key_mods={" ": "_"})
-upsilonconf.save(conf, "config.json", key_mods={"_": " "})
+>>> conf = upsilonconf.load("config.yaml", key_mods={" ": "_"})
+>>> upsilonconf.save(conf, "config.json", key_mods={"_": " "})
 ```
 
+organise hierarchical configs in directories
+
 ```python
-# organise hierarchical configs in directories
-upsilonconf.save({"key": "option1"}, "config_dir/config.json")
-upsilonconf.save({"foo": 1, "bar": 2}, "config_dir/key/option1.json")
-upsilonconf.save({"foo": 2, "baz": 3}, "config_dir/key/option2.json")
+>>> upsilonconf.save({"key": "option1"}, "config_dir/config.json")
+>>> upsilonconf.save({"foo": 1, "bar": 2}, "config_dir/key/option1.json")
+>>> upsilonconf.save({"foo": 2, "baz": 3}, "config_dir/key/option2.json")
 ```
 
+load arbitrary parts of hierarchy
+
 ```python
-# load arbitrary parts of hierarchy
-conf = upsilonconf.load("config_dir/key")
-conf == upsilonconf.Configuration(
-    option1={"foo": 1, "bar": 2}, 
-    option2={"foo": 2, "baz": 3}
-)
+>>> conf = upsilonconf.load("config_dir/key")
+>>> conf == Configuration(
+...     option1={"foo": 1, "bar": 2},
+...     option2={"foo": 2, "baz": 3}
+... )
 ```
 
+hierarchies enable option feature
+
 ```python
-# hierarchies enable option feature
-conf = upsilonconf.load("config_dir")
-conf == upsilonconf.Configuration(key={"foo": 1, "bar": 2})
+>>> conf = upsilonconf.load("config_dir")
+>>> conf == Configuration(key={"foo": 1, "bar": 2})
 ```
 
+store hierarchy to directory with a default file format
+
 ```python
-# store hierarchy to default file in specified directory
-upsilonconf.save(conf, "backup")
+>>> upsilonconf.save(conf, "backup")
 ```
 
 ###### CLI helper
 
+read command-line arguments
+
 ```python
-# read command-line arguments (from sys.argv)
-conf = upsilonconf.from_cli()
+>>> conf = upsilonconf.from_cli()
+```
 
-# parse arbitrary arguments to construct config
-conf = upsilonconf.from_cli(["key=1", "sub.test=2"])
-conf == upsilonconf.Configuration(key=1, sub={"test": 2})
+parse arbitrary arguments to construct config
+
+```python
+>>> conf = upsilonconf.from_cli(["key=1", "sub.test=2"])
+>>> assert conf == Configuration(key=1, sub={"test": 2})
 ```
 
+use file as base config
+
 ```python
-# use file as base config
-conf = upsilonconf.from_cli(["--config", "config.yaml", "key=1", "sub.test=2"])
-result = upsilonconf.load("config.yaml")
-result.overwrite_all(key=1, sub={"test": 2})
-conf == result
+>>> conf = upsilonconf.from_cli(["--config", "config.yaml", "key=1", "sub.test=2"])
+>>> result = upsilonconf.load("config.yaml")
+>>> result.overwrite_all(key=1, sub={"test": 2})
+>>> assert conf == result
 ```
 
+enhance existing argparser
+
 ```python
-# enhance existing argparser
-from argparse import ArgumentParser
-parser = ArgumentParser()
-# add other arguments...
-conf, args = upsilonconf.from_cli(parser=parser)
+>>> from argparse import ArgumentParser
+>>> parser = ArgumentParser()
+>>> # add other arguments...
+>>> conf, args = upsilonconf.from_cli(parser=parser)
 ```
+
+### Feedback
+
+This library is very much a work in progress.
+I welcome any feedback, especially in shaping the interface.
+Of course, also bug reports and feature requests are very useful feedback.
+Just create an [issue](https://github.com/hoedt/upsilonconf/issues) on github.
+
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `upsilonconf-0.6.0/README.md` & `upsilonconf-0.7.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,173 +1,193 @@
 # UpsilonConf
 
 UpsilonConf is a simple configuration library written in Python.
-It might not be really obvious, but this library is inspired by the great [OmegaConf](https://github.com/omry/omegaconf) library.
-OmegaConf is also the backbone for the more advanced [Hydra](https://hydra.cc/) framework.
-Concretely, the idea of this library is to provide an alternative to OmegaConf without the overhead of the variable interpolation (especially the `antlr` dependency).
-It is also very similar to the (discontinued) [AttrDict](https://github.com/bcj/AttrDict) library.
-In the meantime, there is also the [ml_collections](https://github.com/google/ml_collections) library, which seems to build on similar ideas as this project.
 
-Nevertheless, I decided to release upsilonconf because there might be a few features that people might find interesting/useful:
+A few features that you might find interesting/useful:
  - dict-like configuration object with attribute access (cf. `attrdict`)
  - hierarchical indexing by means of tuples or *dot-strings* (cf. `omegaconf`)
- - overwriting protection to prevent unexplainable bugs
  - read from/write to various file formats
  - use hierarchical configs with options (cf. config groups in `hydra`)
  - retrieve and manipulate config using CLI (cf. `omegaconf`)
  - minimal dependencies (cf. `attrdict`)
+ - configs with overwriting protection to prevent unexplainable bugs
 
-The name is inspired by OmegaConf.
-I decided to go for the Greek letter [Upsilon](https://en.wikipedia.org/wiki/Upsilon) because it is the first letter of [ὑπέρ (hupér)](https://en.wiktionary.org/wiki/ὑπέρ).
-This again comes from the fact that this library should mainly help me with managing _hyper_-parameters in neural networks.
+[![pypi badge](https://img.shields.io/pypi/v/upsilonconf?label=PyPI)](https://pypi.org/project/upsilonconf)
+[![conda badge](https://img.shields.io/conda/v/hoedt/upsilonconf)](https://anaconda.org/hoedt/upsilonconf)
+[![docs badge](https://img.shields.io/github/actions/workflow/status/hoedt/upsilonconf/sphinx.yml?branch=main&label=docs&logo=github)](https://hoedt.github.io/upsilonconf)
+[![licencse badge](https://img.shields.io/github/license/hoedt/upsilonconf)](https://github.com/hoedt/upsilonconf/blob/main/LICENSE)
+
+---
 
 ### How to install
 
-Using `pip` to install from [PyPI](https://pypi.org/project/upsilonconf/):
+Using `pip` to install from PyPI:
 
 ```shell
 python -m pip install upsilonconf
 ```
 
-or, to install the (optional) dependencies (`pyyaml`) for YAML IO
+Optional dependencies (e.g. `pyyaml`) can be included using
 
 ```shell
 python -m pip install upsilonconf[YAML]
 ```
 
-Using `conda` to install from [Anaconda](https://anaconda.org/hoedt/upsilonconf):
+Using `conda` to install from Anaconda:
 
 ```shell
 conda install hoedt::upsilonconf
 ```
 
 Optional dependencies (e.g. `pyyaml`) have to be installed separately.
 
 ---
 
 ### How to Use
 
 ```python
-import upsilonconf
+>>> import upsilonconf
+>>> from upsilonconf import PlainConfiguration as Configuration
 ```
 
-###### creation
+###### Creation
+
+load config from file
 
 ```python
-conf1 = upsilonconf.load("config.yaml")  # from config file
-conf2 = upsilonconf.Configuration(key1="value1", key2=2)  # direct
-dictionary = {"sub": conf2}  # sub-configs allowed!
-conf3 = upsilonconf.Configuration(**dictionary)  # from dict
-free_dict = {"a key": "with whitespace"}
-confX = upsilonconf.Configuration.from_dict(free_dict, key_mods={" ": "_"})
-conf = conf1 | conf2 | conf3  # from other configurations
+>>> conf = upsilonconf.load("my_config.yml")
 ```
 
-###### indexing
+or directly create config object
 
 ```python
-# getters
-conf["key1"] == conf.key1
-conf.key2 == conf["sub", "key2"]
-conf["sub", "key1"] == conf["sub.key1"]
-conf["sub.key2"] == conf.sub.key2
+>>> conf = Configuration(key1="value1", sub={"key1": 1, "key2": 2})
+```
 
-# setters
-conf["new_key"] = "new_value"
-conf.other_key = "other_value"
-conf.sub2 = {"a": .1, "b": 2}
-conf["sub2", "c"] = 3.
-conf["sub2.d"] = -4
+###### Indexing
 
-# and deleters...
-del conf["sub2.c"]
+Access values the way you like
+
+```python
+>>> assert conf["key1"] == conf.key1
+>>> assert conf.sub.key2 == conf["sub", "key2"]
+>>> assert conf["sub", "key1"] == conf["sub.key1"]
+>>> assert conf["sub.key2"] == conf.sub.key2
 ```
 
-###### overwrite protection
+###### Cool Tricks
+
+unpack configurations to function arguments
 
 ```python
-try:
-    conf["key1"] = "overwrite1"
-except ValueError:
-    print("overwriting")
-    conf.overwrite("key1", "overwrite1")
+>>> def test(key1, key2):
+...    return key1 + key2
+>>> test(**conf.sub)
+3
+```
 
-try:
-    conf.key1 = "overwrite2"
-except AttributeError:
-    print("overwriting")
-    conf.overwrite("key1", "overwrite2")
+convert config to flat `dict`
 
-try:
-    conf.update(key1="overwrite3")
-except ValueError:
-    print("overwriting")
-    conf.overwrite_all(key1="overwrite3")
+```python
+>>> conf.to_dict(flat=True)
+{'key1': 'value1', 'sub.key1': 1, 'sub.key2': 2}
 ```
 
+merge configurations with `|`
+
+```python
+>>> merged = conf | {"sub.key2": 3, "sub.key3": 2}
+>>> merged.sub.key2
+3
+>>> merged.sub.key3
+2
+```
+
+More details can be found in the [documentation](https://hoedt.github.io/upsilonconf)
+
 ###### flexible I/O
 
+support for different file formats
+
 ```python
-# different file formats (with optional requirements)
-conf = upsilonconf.load("config.yaml")  # with patched float parsing
-upsilonconf.save(conf, "config.json")  # with indentation by default
+>>> conf = upsilonconf.load("config.yaml")  # with patched float parsing
+>>> upsilonconf.save(conf, "config.json")  # with indentation by default
 ```
 
+transform non-identifier keys in files on-the-fly
+
 ```python
-# fix invalid keys in files on-the-fly
-conf = upsilonconf.load("config.yaml", key_mods={" ": "_"})
-upsilonconf.save(conf, "config.json", key_mods={"_": " "})
+>>> conf = upsilonconf.load("config.yaml", key_mods={" ": "_"})
+>>> upsilonconf.save(conf, "config.json", key_mods={"_": " "})
 ```
 
+organise hierarchical configs in directories
+
 ```python
-# organise hierarchical configs in directories
-upsilonconf.save({"key": "option1"}, "config_dir/config.json")
-upsilonconf.save({"foo": 1, "bar": 2}, "config_dir/key/option1.json")
-upsilonconf.save({"foo": 2, "baz": 3}, "config_dir/key/option2.json")
+>>> upsilonconf.save({"key": "option1"}, "config_dir/config.json")
+>>> upsilonconf.save({"foo": 1, "bar": 2}, "config_dir/key/option1.json")
+>>> upsilonconf.save({"foo": 2, "baz": 3}, "config_dir/key/option2.json")
 ```
 
+load arbitrary parts of hierarchy
+
 ```python
-# load arbitrary parts of hierarchy
-conf = upsilonconf.load("config_dir/key")
-conf == upsilonconf.Configuration(
-    option1={"foo": 1, "bar": 2}, 
-    option2={"foo": 2, "baz": 3}
-)
+>>> conf = upsilonconf.load("config_dir/key")
+>>> conf == Configuration(
+...     option1={"foo": 1, "bar": 2},
+...     option2={"foo": 2, "baz": 3}
+... )
 ```
 
+hierarchies enable option feature
+
 ```python
-# hierarchies enable option feature
-conf = upsilonconf.load("config_dir")
-conf == upsilonconf.Configuration(key={"foo": 1, "bar": 2})
+>>> conf = upsilonconf.load("config_dir")
+>>> conf == Configuration(key={"foo": 1, "bar": 2})
 ```
 
+store hierarchy to directory with a default file format
+
 ```python
-# store hierarchy to default file in specified directory
-upsilonconf.save(conf, "backup")
+>>> upsilonconf.save(conf, "backup")
 ```
 
 ###### CLI helper
 
+read command-line arguments
+
 ```python
-# read command-line arguments (from sys.argv)
-conf = upsilonconf.from_cli()
+>>> conf = upsilonconf.from_cli()
+```
 
-# parse arbitrary arguments to construct config
-conf = upsilonconf.from_cli(["key=1", "sub.test=2"])
-conf == upsilonconf.Configuration(key=1, sub={"test": 2})
+parse arbitrary arguments to construct config
+
+```python
+>>> conf = upsilonconf.from_cli(["key=1", "sub.test=2"])
+>>> assert conf == Configuration(key=1, sub={"test": 2})
 ```
 
+use file as base config
+
 ```python
-# use file as base config
-conf = upsilonconf.from_cli(["--config", "config.yaml", "key=1", "sub.test=2"])
-result = upsilonconf.load("config.yaml")
-result.overwrite_all(key=1, sub={"test": 2})
-conf == result
+>>> conf = upsilonconf.from_cli(["--config", "config.yaml", "key=1", "sub.test=2"])
+>>> result = upsilonconf.load("config.yaml")
+>>> result.overwrite_all(key=1, sub={"test": 2})
+>>> assert conf == result
 ```
 
+enhance existing argparser
+
 ```python
-# enhance existing argparser
-from argparse import ArgumentParser
-parser = ArgumentParser()
-# add other arguments...
-conf, args = upsilonconf.from_cli(parser=parser)
+>>> from argparse import ArgumentParser
+>>> parser = ArgumentParser()
+>>> # add other arguments...
+>>> conf, args = upsilonconf.from_cli(parser=parser)
 ```
+
+### Feedback
+
+This library is very much a work in progress.
+I welcome any feedback, especially in shaping the interface.
+Of course, also bug reports and feature requests are very useful feedback.
+Just create an [issue](https://github.com/hoedt/upsilonconf/issues) on github.
+
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `upsilonconf-0.6.0/setup.cfg` & `upsilonconf-0.7.0/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 description = A simple configuration library
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Pieter-Jan Hoedt
 author_email = hoedt@ml.jku.at
 url = https://github.com/hoedt/upsilonconf
 project_urls = 
+	Documentation = https://hoedt.github.io/upsilonconf
 	Bug Tracker = https://github.com/hoedt/upsilonconf/issues
 classifiers = 
 	Development Status :: 3 - Alpha
 	Intended Audience :: Developers
 	Intended Audience :: Science/Research
 	Topic :: Utilities
 	Programming Language :: Python :: 3
@@ -25,12 +26,14 @@
 	upsilonconf.io
 
 [options.extras_require]
 YAML = 
 	pyyaml>=5.4.1
 TOML = 
 	tomlkit>=0.8.0
+DOCS = 
+	numpydoc>=1.5.0
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `upsilonconf-0.6.0/upsilonconf/io/__init__.py` & `upsilonconf-0.7.0/upsilonconf/io/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,35 +1,39 @@
 from pathlib import Path
-from typing import Mapping, Union
+from typing import Mapping, Union, Optional
 
-from ..config import Configuration
+from ..config import ConfigurationBase
 from ._optional_dependencies import OptionalDependencyError
-from .base import ConfigIO, FlexibleIO
+from .base import ConfigIO, ExtensionIO, FlexibleIO
 from .json import JSONIO
 from .yaml import YAMLIO
+from .toml import TOMLIO
 from .directory import DirectoryIO
 
 
 __all__ = [
     "OptionalDependencyError",
     "ConfigIO",
-    "FlexibleIO",
+    "ExtensionIO",
     "JSONIO",
     "YAMLIO",
+    "TOMLIO",
     "DirectoryIO",
     "load_config",
     "save_config",
     "from_cli",
 ]
 
 _default_io = None
 
 
-def get_default_io(default_ext: str = None) -> ConfigIO:
+def get_default_io(default_ext: Optional[str] = None) -> ConfigIO:
     """
+    Get the default I/O setup.
+
     Parameters
     ----------
     default_ext : str, optional
         The extension to use as the default for reading/writing config files.
         If not specified, the default is chosen for you.
 
     Returns
@@ -37,89 +41,89 @@
     default_io : ConfigIO
         The default IO for reading and writing configuration files.
 
     Raises
     ------
     ValueError
         If there is no (known) IO for the value passed for `default_ext`.
-
-    See Also
-    --------
-    FlexibleIO : IO to map extensions to other IOs.
     """
     global _default_io
     if _default_io is not None:
         return _default_io
 
-    json_io = JSONIO()
-    yaml_io = YAMLIO()
-    _default_io = FlexibleIO(
-        {
-            ".json": json_io,  # default format
-            ".yaml": yaml_io,
-            ".yml": yaml_io,
-        },
-        default_ext=default_ext,
-    )
-    _default_io.update("", DirectoryIO(_default_io))
+    _default_io = ExtensionIO(JSONIO(), YAMLIO(), TOMLIO(), default_ext=default_ext)
+    _default_io[""] = DirectoryIO(_default_io)
     return _default_io
 
 
 def load_config(
     path: Union[Path, str],
-    key_mods: Mapping[str, str] = None,
-    config_io: ConfigIO = None,
-) -> Configuration:
+    key_mods: Optional[Mapping[str, str]] = None,
+    config_io: Optional[ConfigIO] = None,
+) -> ConfigurationBase:
     """
-    Read configuration from disk.
+    Load configuration from a file.
 
     Parameters
     ----------
     path : Path or str
-        Path to a readable location on disk.
+        Path to a readable text file on disk.
     key_mods : dict, optional
         A dictionary mapping key substrings to replacement patterns.
         This allows to modify keys with invalid characters for config keys.
     config_io : ConfigIO, optional
         The IO to use for reading the file.
-        By default, the IO will be inferred from the file extension.
+        If not specified, the default IO will be used.
 
     Returns
     -------
-    config : Configuration
+    config : ConfigurationBase
         A configuration object with the key-value pairs as provided in the file.
+
+    See Also
+    --------
+    io.get_default_io : retrieve the default IO.
+    io.ConfigIO.load_config : implementation of functionality.
     """
     if config_io is None:
         config_io = get_default_io()
 
     return config_io.load_config(path, key_mods)
 
 
 def save_config(
-    config: Configuration,
+    config: ConfigurationBase,
     path: Union[Path, str],
-    key_mods: Mapping[str, str] = None,
-    config_io: ConfigIO = None,
+    key_mods: Optional[Mapping[str, str]] = None,
+    config_io: Optional[ConfigIO] = None,
 ) -> None:
     """
-    Write a configuration to disk.
+    Write a configuration data to disk.
 
     Parameters
     ----------
+    config : ConfigurationBase
+        The configuration object to save.
     path : Path or str
-        Path to a writeable location on disk.
+        Path to a writeable text file on disk.
     key_mods : dict, optional
         A dictionary mapping key substrings to replacement patterns.
         This allows to modify keys with invalid characters for config keys.
     config_io : ConfigIO, optional
         The IO to use for writing the file.
-        By default, the IO will be inferred from the file extension.
+        If not specified, the default IO will be used.
+
+    See Also
+    --------
+    io.get_default_io : retrieve the default IO.
+    io.ConfigIO.save_config : implementation of functionality.
     """
     if config_io is None:
         config_io = get_default_io()
+
     config_io.save_config(config, path, key_mods)
 
 
 def from_cli(args=None, parser=None, config_io=None):
     """
     Construct a configuration from a Command Line Interface.
 
@@ -140,15 +144,15 @@
         Moreover, the parser should not already use the names *config* or *overrides*.
         If not specified, an empty parser will be created.
     config_io : ConfigIO
         The IO to use for reading config files that are passed as argument.
 
     Returns
     -------
-    config : Configuration
+    config : ConfigurationBase
         The configuration as specified by the command line arguments.
     ns : Namespace, optional
         The namespace with additional arguments from the command line arguments.
         This is only returned if `parser` is not ``None``
     """
     from .cli import ConfigParser
```

### Comparing `upsilonconf-0.6.0/upsilonconf/io/_optional_dependencies.py` & `upsilonconf-0.7.0/upsilonconf/io/_optional_dependencies.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-from typing import Callable
+from typing import Optional, Callable
 
 
 class OptionalDependencyError(ImportError):
     """Raised when an attempt is made to import an optional dependency."""
 
     pass
 
 
 def optional_dependency_to(
-    feature: str = None, package: str = None
+    feature: Optional[str] = None, package: Optional[str] = None
 ) -> Callable[[Callable], Callable]:
     """
     Decorator factory for functions that provide optional features.
 
     The decorators produced by this decorator factory aim
     to capture any import errors that might occur
     as a result of optional dependencies not being installed.
```

### Comparing `upsilonconf-0.6.0/upsilonconf/io/cli.py` & `upsilonconf-0.7.0/upsilonconf/io/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,40 @@
 from argparse import ArgumentParser
 from pathlib import Path
-from typing import Tuple, Any, Sequence
+from typing import Tuple, Any, Sequence, Optional
 
 from .base import ConfigIO
-from ..config import Configuration
+from ..config import CarefulConfiguration
 
 
 class ConfigParser:
     """
     Wrapper around ArgumentParser with a configuration group.
 
     This wrapper adds a *configuration* group to an argument parser.
     With this group, positional arguments are parsed as key-value pairs.
     Additionally, a ``--config`` option is added if an IO has been specified.
     The ``--config`` option takes a filename as argument
     from which a base configuration can be loaded.
+
+    .. versionadded:: 0.5.0
+
+    Parameters
+    ----------
+    config_io : ConfigIO
+        Specifies how configuration files are read.
+    parser : ArgumentParser, optional
+        The CLI parser to use as a base for retrieving configuration options.
+        The parser can not (already) expect a variable number of positional args.
+        Moreover, the parser should not already use the names *config* or *overrides*.
+        If not specified, an empty parser will be created.
+    return_ns : bool, optional
+        If ``True``, `parse_config` will also return the namespace.
+        If ``False``, it will only return the configuration.
+        By default, `return_ns` is set to ``True`` if `parser` is not ``None``.
     """
 
     @staticmethod
     def _assignment_expr(s: str) -> Tuple[str, Any]:
         """Parse assignment expression argument."""
         import json
 
@@ -28,43 +44,28 @@
         except json.JSONDecodeError:
             pass
 
         return key, val
 
     def __init__(
         self,
-        parser: ArgumentParser = None,
-        config_io: ConfigIO = None,
-        return_ns: bool = None,
+        parser: Optional[ArgumentParser] = None,
+        config_io: Optional[ConfigIO] = None,
+        return_ns: Optional[bool] = None,
     ):
-        """
-        Parameters
-        ----------
-        config_io : ConfigIO
-            Specifies how configuration files are read.
-        parser : ArgumentParser, optional
-            The CLI parser to use as a base for retrieving configuration options.
-            The parser can not (already) expect a variable number of positional args.
-            Moreover, the parser should not already use the names *config* or *overrides*.
-            If not specified, an empty parser will be created.
-        return_ns : bool, optional
-            If ``True``, `parse_config` will also return the namespace.
-            If ``False``, it will only return the configuration.
-            By default, `return_ns` is set to ``True`` if `parser` is not ``None``.
-        """
         if return_ns is None:
             return_ns = parser is not None
 
         self._parser = ArgumentParser() if parser is None else parser
         self._config_io = config_io
         self.return_ns = return_ns
 
         self._modify_parser()
 
-    def _modify_parser(self):
+    def _modify_parser(self) -> None:
         """Add the configuration group to the parser."""
         group = self._parser.add_argument_group("configuration")
         group.add_argument(
             "overrides",
             nargs="*",
             type=self._assignment_expr,
             help="configuration options to override in the config file",
@@ -81,39 +82,39 @@
             )
 
     @property
     def parser(self) -> ArgumentParser:
         """Wrapped `ArgumentParser` instance."""
         return self._parser
 
-    def parse_config(self, args: Sequence[str] = None):
+    def parse_config(self, args: Optional[Sequence[str]] = None):
         """
         Parse a configuration from command line arguments.
 
         Parameters
         ----------
         args : sequence of str, optional
             The list of arguments to parse.
             By default, arguments are taken from ``sys.argv``.
 
         Returns
         -------
-        config : Configuration
+        config : ConfigurationBase
             The configuration as specified by the command line arguments.
         ns : Namespace, optional
             The namespace with non-configuration arguments.
             This is only returned if `return_ns` is ``True``.
         """
         ns = self._parser.parse_args(args)
         config = (
-            Configuration()
+            CarefulConfiguration()
             if self._config_io is None or ns.config is None
             else self._config_io.load_config(ns.config)
         )
-        config.overwrite_all(ns.overrides)
+        config |= dict(ns.overrides)
         if not self.return_ns:
             return config
 
         del ns.overrides
         if self._config_io is not None:
             del ns.config
```

### Comparing `upsilonconf-0.6.0/upsilonconf/io/directory.py` & `upsilonconf-0.7.0/upsilonconf/io/directory.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,10 @@
+from typing import Optional
+
 from .base import ConfigIO
-from ..config import Configuration
 
 
 class DirectoryIO(ConfigIO):
     """
     IO for reading/writing configs from a directory.
 
     A config directory can hold any combination of the following three elements:
@@ -12,14 +13,24 @@
         These sub-configs are directly added to the base config.
         The filename of this sub-config will be a new(!) key in the base config.
      3. Config files/directories with config options for the base config.
         These sub-configs provide one or more sub-config options
         for an existing(!) key in the base config.
         Therefore, the filename must match one of the keys in the base config.
 
+    .. versionadded:: 0.5.0
+
+    Parameters
+    ----------
+    config_io : ConfigIO
+        The io to use to read/write files in each directory.
+    main_file : str, optional
+        The filename that specifies the main config file when reading
+        or the filename for the file that is created when writing.
+
     Examples
     --------
     Consider a directory with structure::
 
         examples/hparam/
           config.yaml
           bar.yaml
@@ -37,30 +48,21 @@
 
         # baz.yaml
         a: 0.1
         b: 0.2
 
     When reading this directory, we end up with the following configuration:
 
-    >>> upsilonconf.load_config("examples/hparam")
-    ... Configuration(foo=1, baz=Configuration(a=0.1, b=0.2), bar='hparam')
+    >>> upsilonconf.load_config("examples/hparam")  # doctest: +SKIP
+    PlainConfiguration(foo=1, baz=PlainConfiguration(a=0.1, b=0.2), bar='hparam')
     """
 
     DEFAULT_NAME = "config"
 
-    def __init__(self, config_io: ConfigIO, main_file: str = None):
-        """
-        Parameters
-        ----------
-        config_io : ConfigIO
-            The io to use to read/write files in each directory.
-        main_file : str, optional
-            The filename that specifies the main config file when reading
-            or the filename for the file that is created when writing.
-        """
+    def __init__(self, config_io: ConfigIO, main_file: Optional[str] = None):
         if main_file is None:
             main_file = self.DEFAULT_NAME
 
         parts = main_file.rsplit(".", maxsplit=1)
         name, ext = parts[0], (None if len(parts) < 2 else f".{parts[1]}")
         if ext is not None and ext not in config_io.extensions:
             raise ValueError("unsupported extension for given IO")
@@ -75,25 +77,26 @@
 
     @property
     def file_name(self) -> str:
         ext = self.config_io.default_ext if self._file_ext is None else self._file_ext
         return self._file_name + ext
 
     def read_from(self, stream):
-        raise TypeError("directory IO does not support streams")
+        cls_name = self.__class__.__name__
+        raise TypeError(f"{cls_name} does not support reading from stream")
 
-    def read(self, path):
+    def read(self, path, encoding="utf-8"):
         try:
             base_path = next(path.glob(f"{self._file_name}.*"))
-            base_conf = self.config_io.read(base_path)
+            base_conf = self.config_io.read(base_path, encoding)
             if self._file_ext is None:
                 self._file_ext = base_path.suffix
         except StopIteration:
             base_path = None
-            base_conf = Configuration()
+            base_conf = {}
 
         for sub in path.iterdir():
             if sub == base_path:
                 continue
 
             key, sub_conf = sub.stem, self.config_io.read(sub)
             if key in base_conf:
@@ -106,14 +109,15 @@
                         f"does not match any of the options in '{sub.name}'"
                     )
 
             base_conf[key] = sub_conf
 
         return base_conf
 
-    def write(self, conf, path):
+    def write(self, conf, path, encoding="utf-8"):
         file_path = path / self.file_name
         path.mkdir(exist_ok=True)
-        self.config_io.write(conf, file_path)
+        self.config_io.write(conf, file_path, encoding)
 
     def write_to(self, stream, config):
-        raise TypeError("directory IO does not support streams")
+        cls_name = self.__class__.__name__
+        raise TypeError(f"{cls_name} does not support writing to stream")
```

### Comparing `upsilonconf-0.6.0/upsilonconf/io/json.py` & `upsilonconf-0.7.0/upsilonconf/io/json.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 from .base import ConfigIO
 
 
 class JSONIO(ConfigIO):
-    """IO for reading/writing JSON files."""
+    """
+    IO for reading/writing JSON files.
+
+    .. versionadded:: 0.5.0
+
+    Parameters
+    ----------
+    indent : int, optional
+        The number of spaces to use for indentation in the output file.
+    sort_keys : bool, optional
+        Whether keys should be sorted before writing to the output file.
+    """
 
     def __init__(self, indent: int = 2, sort_keys: bool = False):
-        """
-        Parameters
-        ----------
-        indent : int, optional
-            The number of spaces to use for indentation in the output file.
-        sort_keys : bool, optional
-            Whether keys should be sorted before writing to the output file.
-        """
         self._encoder = None
         self._encode_kwargs = {
             "indent": indent,
             "sort_keys": sort_keys,
         }
 
     @property
```

### Comparing `upsilonconf-0.6.0/upsilonconf/io/toml.py` & `upsilonconf-0.7.0/upsilonconf/io/toml.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,15 +2,19 @@
 from collections.abc import Mapping
 
 from upsilonconf.io._optional_dependencies import optional_dependency_to
 from .base import ConfigIO
 
 
 class TOMLIO(ConfigIO):
-    """IO for reading/writing TOML files."""
+    """
+    IO for reading/writing TOML files.
+
+    .. versionadded:: 0.6.0
+    """
 
     @property
     def extensions(self):
         return [".toml"]
 
     @optional_dependency_to("read TOML files for python <3.11")
     def read_from(self, stream):
```

### Comparing `upsilonconf-0.6.0/upsilonconf/io/yaml.py` & `upsilonconf-0.7.0/upsilonconf/io/yaml.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 from collections.abc import Mapping
 
 from ._optional_dependencies import optional_dependency_to
 from .base import ConfigIO
 
 
 class YAMLIO(ConfigIO):
-    """IO for reading/writing YAML files."""
+    """
+    IO for reading/writing YAML files.
+
+    .. versionadded:: 0.5.0
+
+    Parameters
+    ----------
+    indent : int, optional
+        The number of spaces to use for indentation in the output file.
+    sort_keys : bool, optional
+        Whether keys should be sorted before writing to the output file.
+    """
 
     def __init__(self, indent: int = 2, sort_keys: bool = False):
-        """
-        Parameters
-        ----------
-        indent : int, optional
-            The number of spaces to use for indentation in the output file.
-        sort_keys : bool, optional
-            Whether keys should be sorted before writing to the output file.
-        """
         self.kwargs = {"indent": indent, "sort_keys": sort_keys}
         self._loader = None
         self._dumper = None
 
     @property
     def _yaml_loader(self):
         """Lazily loaded (and patched) YAML loader."""
```

### Comparing `upsilonconf-0.6.0/upsilonconf.egg-info/PKG-INFO` & `upsilonconf-0.7.0/upsilonconf.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,193 +1,215 @@
 Metadata-Version: 2.1
 Name: upsilonconf
-Version: 0.6.0
+Version: 0.7.0
 Summary: A simple configuration library
 Home-page: https://github.com/hoedt/upsilonconf
 Author: Pieter-Jan Hoedt
 Author-email: hoedt@ml.jku.at
+Project-URL: Documentation, https://hoedt.github.io/upsilonconf
 Project-URL: Bug Tracker, https://github.com/hoedt/upsilonconf/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Utilities
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Provides-Extra: YAML
 Provides-Extra: TOML
+Provides-Extra: DOCS
 License-File: LICENSE
 
 # UpsilonConf
 
 UpsilonConf is a simple configuration library written in Python.
-It might not be really obvious, but this library is inspired by the great [OmegaConf](https://github.com/omry/omegaconf) library.
-OmegaConf is also the backbone for the more advanced [Hydra](https://hydra.cc/) framework.
-Concretely, the idea of this library is to provide an alternative to OmegaConf without the overhead of the variable interpolation (especially the `antlr` dependency).
-It is also very similar to the (discontinued) [AttrDict](https://github.com/bcj/AttrDict) library.
-In the meantime, there is also the [ml_collections](https://github.com/google/ml_collections) library, which seems to build on similar ideas as this project.
 
-Nevertheless, I decided to release upsilonconf because there might be a few features that people might find interesting/useful:
+A few features that you might find interesting/useful:
  - dict-like configuration object with attribute access (cf. `attrdict`)
  - hierarchical indexing by means of tuples or *dot-strings* (cf. `omegaconf`)
- - overwriting protection to prevent unexplainable bugs
  - read from/write to various file formats
  - use hierarchical configs with options (cf. config groups in `hydra`)
  - retrieve and manipulate config using CLI (cf. `omegaconf`)
  - minimal dependencies (cf. `attrdict`)
+ - configs with overwriting protection to prevent unexplainable bugs
 
-The name is inspired by OmegaConf.
-I decided to go for the Greek letter [Upsilon](https://en.wikipedia.org/wiki/Upsilon) because it is the first letter of [ὑπέρ (hupér)](https://en.wiktionary.org/wiki/ὑπέρ).
-This again comes from the fact that this library should mainly help me with managing _hyper_-parameters in neural networks.
+[![pypi badge](https://img.shields.io/pypi/v/upsilonconf?label=PyPI)](https://pypi.org/project/upsilonconf)
+[![conda badge](https://img.shields.io/conda/v/hoedt/upsilonconf)](https://anaconda.org/hoedt/upsilonconf)
+[![docs badge](https://img.shields.io/github/actions/workflow/status/hoedt/upsilonconf/sphinx.yml?branch=main&label=docs&logo=github)](https://hoedt.github.io/upsilonconf)
+[![licencse badge](https://img.shields.io/github/license/hoedt/upsilonconf)](https://github.com/hoedt/upsilonconf/blob/main/LICENSE)
+
+---
 
 ### How to install
 
-Using `pip` to install from [PyPI](https://pypi.org/project/upsilonconf/):
+Using `pip` to install from PyPI:
 
 ```shell
 python -m pip install upsilonconf
 ```
 
-or, to install the (optional) dependencies (`pyyaml`) for YAML IO
+Optional dependencies (e.g. `pyyaml`) can be included using
 
 ```shell
 python -m pip install upsilonconf[YAML]
 ```
 
-Using `conda` to install from [Anaconda](https://anaconda.org/hoedt/upsilonconf):
+Using `conda` to install from Anaconda:
 
 ```shell
 conda install hoedt::upsilonconf
 ```
 
 Optional dependencies (e.g. `pyyaml`) have to be installed separately.
 
 ---
 
 ### How to Use
 
 ```python
-import upsilonconf
+>>> import upsilonconf
+>>> from upsilonconf import PlainConfiguration as Configuration
 ```
 
-###### creation
+###### Creation
+
+load config from file
 
 ```python
-conf1 = upsilonconf.load("config.yaml")  # from config file
-conf2 = upsilonconf.Configuration(key1="value1", key2=2)  # direct
-dictionary = {"sub": conf2}  # sub-configs allowed!
-conf3 = upsilonconf.Configuration(**dictionary)  # from dict
-free_dict = {"a key": "with whitespace"}
-confX = upsilonconf.Configuration.from_dict(free_dict, key_mods={" ": "_"})
-conf = conf1 | conf2 | conf3  # from other configurations
+>>> conf = upsilonconf.load("my_config.yml")
 ```
 
-###### indexing
+or directly create config object
 
 ```python
-# getters
-conf["key1"] == conf.key1
-conf.key2 == conf["sub", "key2"]
-conf["sub", "key1"] == conf["sub.key1"]
-conf["sub.key2"] == conf.sub.key2
+>>> conf = Configuration(key1="value1", sub={"key1": 1, "key2": 2})
+```
 
-# setters
-conf["new_key"] = "new_value"
-conf.other_key = "other_value"
-conf.sub2 = {"a": .1, "b": 2}
-conf["sub2", "c"] = 3.
-conf["sub2.d"] = -4
+###### Indexing
 
-# and deleters...
-del conf["sub2.c"]
+Access values the way you like
+
+```python
+>>> assert conf["key1"] == conf.key1
+>>> assert conf.sub.key2 == conf["sub", "key2"]
+>>> assert conf["sub", "key1"] == conf["sub.key1"]
+>>> assert conf["sub.key2"] == conf.sub.key2
 ```
 
-###### overwrite protection
+###### Cool Tricks
+
+unpack configurations to function arguments
 
 ```python
-try:
-    conf["key1"] = "overwrite1"
-except ValueError:
-    print("overwriting")
-    conf.overwrite("key1", "overwrite1")
+>>> def test(key1, key2):
+...    return key1 + key2
+>>> test(**conf.sub)
+3
+```
 
-try:
-    conf.key1 = "overwrite2"
-except AttributeError:
-    print("overwriting")
-    conf.overwrite("key1", "overwrite2")
+convert config to flat `dict`
 
-try:
-    conf.update(key1="overwrite3")
-except ValueError:
-    print("overwriting")
-    conf.overwrite_all(key1="overwrite3")
+```python
+>>> conf.to_dict(flat=True)
+{'key1': 'value1', 'sub.key1': 1, 'sub.key2': 2}
 ```
 
+merge configurations with `|`
+
+```python
+>>> merged = conf | {"sub.key2": 3, "sub.key3": 2}
+>>> merged.sub.key2
+3
+>>> merged.sub.key3
+2
+```
+
+More details can be found in the [documentation](https://hoedt.github.io/upsilonconf)
+
 ###### flexible I/O
 
+support for different file formats
+
 ```python
-# different file formats (with optional requirements)
-conf = upsilonconf.load("config.yaml")  # with patched float parsing
-upsilonconf.save(conf, "config.json")  # with indentation by default
+>>> conf = upsilonconf.load("config.yaml")  # with patched float parsing
+>>> upsilonconf.save(conf, "config.json")  # with indentation by default
 ```
 
+transform non-identifier keys in files on-the-fly
+
 ```python
-# fix invalid keys in files on-the-fly
-conf = upsilonconf.load("config.yaml", key_mods={" ": "_"})
-upsilonconf.save(conf, "config.json", key_mods={"_": " "})
+>>> conf = upsilonconf.load("config.yaml", key_mods={" ": "_"})
+>>> upsilonconf.save(conf, "config.json", key_mods={"_": " "})
 ```
 
+organise hierarchical configs in directories
+
 ```python
-# organise hierarchical configs in directories
-upsilonconf.save({"key": "option1"}, "config_dir/config.json")
-upsilonconf.save({"foo": 1, "bar": 2}, "config_dir/key/option1.json")
-upsilonconf.save({"foo": 2, "baz": 3}, "config_dir/key/option2.json")
+>>> upsilonconf.save({"key": "option1"}, "config_dir/config.json")
+>>> upsilonconf.save({"foo": 1, "bar": 2}, "config_dir/key/option1.json")
+>>> upsilonconf.save({"foo": 2, "baz": 3}, "config_dir/key/option2.json")
 ```
 
+load arbitrary parts of hierarchy
+
 ```python
-# load arbitrary parts of hierarchy
-conf = upsilonconf.load("config_dir/key")
-conf == upsilonconf.Configuration(
-    option1={"foo": 1, "bar": 2}, 
-    option2={"foo": 2, "baz": 3}
-)
+>>> conf = upsilonconf.load("config_dir/key")
+>>> conf == Configuration(
+...     option1={"foo": 1, "bar": 2},
+...     option2={"foo": 2, "baz": 3}
+... )
 ```
 
+hierarchies enable option feature
+
 ```python
-# hierarchies enable option feature
-conf = upsilonconf.load("config_dir")
-conf == upsilonconf.Configuration(key={"foo": 1, "bar": 2})
+>>> conf = upsilonconf.load("config_dir")
+>>> conf == Configuration(key={"foo": 1, "bar": 2})
 ```
 
+store hierarchy to directory with a default file format
+
 ```python
-# store hierarchy to default file in specified directory
-upsilonconf.save(conf, "backup")
+>>> upsilonconf.save(conf, "backup")
 ```
 
 ###### CLI helper
 
+read command-line arguments
+
 ```python
-# read command-line arguments (from sys.argv)
-conf = upsilonconf.from_cli()
+>>> conf = upsilonconf.from_cli()
+```
 
-# parse arbitrary arguments to construct config
-conf = upsilonconf.from_cli(["key=1", "sub.test=2"])
-conf == upsilonconf.Configuration(key=1, sub={"test": 2})
+parse arbitrary arguments to construct config
+
+```python
+>>> conf = upsilonconf.from_cli(["key=1", "sub.test=2"])
+>>> assert conf == Configuration(key=1, sub={"test": 2})
 ```
 
+use file as base config
+
 ```python
-# use file as base config
-conf = upsilonconf.from_cli(["--config", "config.yaml", "key=1", "sub.test=2"])
-result = upsilonconf.load("config.yaml")
-result.overwrite_all(key=1, sub={"test": 2})
-conf == result
+>>> conf = upsilonconf.from_cli(["--config", "config.yaml", "key=1", "sub.test=2"])
+>>> result = upsilonconf.load("config.yaml")
+>>> result.overwrite_all(key=1, sub={"test": 2})
+>>> assert conf == result
 ```
 
+enhance existing argparser
+
 ```python
-# enhance existing argparser
-from argparse import ArgumentParser
-parser = ArgumentParser()
-# add other arguments...
-conf, args = upsilonconf.from_cli(parser=parser)
+>>> from argparse import ArgumentParser
+>>> parser = ArgumentParser()
+>>> # add other arguments...
+>>> conf, args = upsilonconf.from_cli(parser=parser)
 ```
+
+### Feedback
+
+This library is very much a work in progress.
+I welcome any feedback, especially in shaping the interface.
+Of course, also bug reports and feature requests are very useful feedback.
+Just create an [issue](https://github.com/hoedt/upsilonconf/issues) on github.
+
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

