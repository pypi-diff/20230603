# Comparing `tmp/aioarp-0.0.1.tar.gz` & `tmp/aioarp-0.0.2.tar.gz`

## Comparing `aioarp-0.0.1.tar` & `aioarp-0.0.2.tar`

### file list

```diff
@@ -1,76 +1,76 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 aioarp-0.0.1/requirements.txt
--rw-r--r--   0        0        0     1313 2020-02-02 00:00:00.000000 aioarp-0.0.1/unasync.py
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 aioarp-0.0.1/.ruff_cache/.gitignore
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 aioarp-0.0.1/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 aioarp-0.0.1/.ruff_cache/content/17946c0e3734f56
--rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 aioarp-0.0.1/.ruff_cache/content/18bd9323e775c06
--rw-r--r--   0        0        0     1211 2020-02-02 00:00:00.000000 aioarp-0.0.1/.ruff_cache/content/1cf748db3edf4393
--rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 aioarp-0.0.1/.ruff_cache/content/1d813f87eae436dc
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 aioarp-0.0.1/.ruff_cache/content/20360c87813708ee
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 aioarp-0.0.1/.ruff_cache/content/20e8c6fb6ec65fba
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 aioarp-0.0.1/.ruff_cache/content/22273ee756d2aeab
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 aioarp-0.0.1/.ruff_cache/content/22eb75e2705cd7cb
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 aioarp-0.0.1/.ruff_cache/content/27380b38303cddd4
--rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 aioarp-0.0.1/.ruff_cache/content/2894d2afe73e6dee
--rw-r--r--   0        0        0     2414 2020-02-02 00:00:00.000000 aioarp-0.0.1/.ruff_cache/content/28bfffee8af0f637
--rw-r--r--   0        0        0     1211 2020-02-02 00:00:00.000000 aioarp-0.0.1/.ruff_cache/content/29a3dfb41b2e153e
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 aioarp-0.0.1/.ruff_cache/content/2b17b1ab21ba1879
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 aioarp-0.0.1/.ruff_cache/content/3546886ec7b89ca2
--rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 aioarp-0.0.1/.ruff_cache/content/44618acc04af2a98
--rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 aioarp-0.0.1/.ruff_cache/content/464ea8dcb036f50b
--rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 aioarp-0.0.1/.ruff_cache/content/48dc01dafed313cb
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 aioarp-0.0.1/.ruff_cache/content/53922c565bc4cfdf
--rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 aioarp-0.0.1/.ruff_cache/content/608e0f7e2331dfd0
--rw-r--r--   0        0        0     5263 2020-02-02 00:00:00.000000 aioarp-0.0.1/.ruff_cache/content/64f9f289e0610564
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 aioarp-0.0.1/.ruff_cache/content/65bac7c6a4c4cb5e
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 aioarp-0.0.1/.ruff_cache/content/6857c9063a540073
--rw-r--r--   0        0        0     3069 2020-02-02 00:00:00.000000 aioarp-0.0.1/.ruff_cache/content/6ba798af16bd34e5
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 aioarp-0.0.1/.ruff_cache/content/75d5cb975af2bc07
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 aioarp-0.0.1/.ruff_cache/content/7753615b71d6a36e
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 aioarp-0.0.1/.ruff_cache/content/869f865c9f14daf7
--rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 aioarp-0.0.1/.ruff_cache/content/936f955f01285847
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 aioarp-0.0.1/.ruff_cache/content/967dc6947ad8c113
--rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 aioarp-0.0.1/.ruff_cache/content/a12cec0addd27620
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 aioarp-0.0.1/.ruff_cache/content/a64cd85354e281c5
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 aioarp-0.0.1/.ruff_cache/content/b3202a665cec273b
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 aioarp-0.0.1/.ruff_cache/content/bdd7c44b4f88bf5b
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 aioarp-0.0.1/.ruff_cache/content/c0d92e761aa72a56
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 aioarp-0.0.1/.ruff_cache/content/c24cf3b955d01f58
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 aioarp-0.0.1/.ruff_cache/content/c2e7f8eb8bfe8525
--rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 aioarp-0.0.1/.ruff_cache/content/c78c3248c370d9f2
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 aioarp-0.0.1/.ruff_cache/content/c7a507ee84d3e2ab
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 aioarp-0.0.1/.ruff_cache/content/dc53fc214ceea0dd
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 aioarp-0.0.1/.ruff_cache/content/de93c4dfa993ec19
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 aioarp-0.0.1/.ruff_cache/content/e11920c476dc4f59
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 aioarp-0.0.1/.ruff_cache/content/e12d636458d129da
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 aioarp-0.0.1/.ruff_cache/content/e305b1c5b826225
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 aioarp-0.0.1/.ruff_cache/content/e512a2b647437caa
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 aioarp-0.0.1/.ruff_cache/content/f3ac79af6cdde497
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 aioarp-0.0.1/.ruff_cache/content/f3d289f55f0ad6bd
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 aioarp-0.0.1/.ruff_cache/content/f45e36470415dca1
--rw-r--r--   0        0        0     3130 2020-02-02 00:00:00.000000 aioarp-0.0.1/.ruff_cache/content/f58c3d661899d706
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 aioarp-0.0.1/.ruff_cache/content/ffe7d79671eca8f
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 aioarp-0.0.1/aioarp/__about__.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 aioarp-0.0.1/aioarp/__init__.py
--rw-r--r--   0        0        0     4727 2020-02-02 00:00:00.000000 aioarp-0.0.1/aioarp/_arp.py
--rw-r--r--   0        0        0     1372 2020-02-02 00:00:00.000000 aioarp-0.0.1/aioarp/_client.py
--rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 aioarp-0.0.1/aioarp/_exceptions.py
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 aioarp-0.0.1/aioarp/_mock.py
--rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 aioarp-0.0.1/aioarp/_utils.py
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 aioarp-0.0.1/aioarp/defaults.py
--rw-r--r--   0        0        0     1912 2020-02-02 00:00:00.000000 aioarp-0.0.1/aioarp/_async/__init__.py
--rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 aioarp-0.0.1/aioarp/_sync/__init__.py
--rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 aioarp-0.0.1/aioarp/backends/_async.py
--rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 aioarp-0.0.1/aioarp/backends/_sync.py
--rwxr-xr-x   0        0        0       37 2020-02-02 00:00:00.000000 aioarp-0.0.1/scripts/check
--rwxr-xr-x   0        0        0       30 2020-02-02 00:00:00.000000 aioarp-0.0.1/scripts/lint
--rwxr-xr-x   0        0        0       52 2020-02-02 00:00:00.000000 aioarp-0.0.1/scripts/test
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 aioarp-0.0.1/tests/__init__.py
--rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 aioarp-0.0.1/tests/test_client.py
--rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 aioarp-0.0.1/tests/test_proto.py
--rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 aioarp-0.0.1/tests/test_utils.py
--rw-r--r--   0        0        0     2721 2020-02-02 00:00:00.000000 aioarp-0.0.1/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 aioarp-0.0.1/LICENSE.txt
--rw-r--r--   0        0        0     4421 2020-02-02 00:00:00.000000 aioarp-0.0.1/README.md
--rw-r--r--   0        0        0     1326 2020-02-02 00:00:00.000000 aioarp-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     5329 2020-02-02 00:00:00.000000 aioarp-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 aioarp-0.0.2/requirements.txt
+-rw-r--r--   0        0        0     1313 2020-02-02 00:00:00.000000 aioarp-0.0.2/unasync.py
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 aioarp-0.0.2/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 aioarp-0.0.2/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 aioarp-0.0.2/.ruff_cache/content/17946c0e3734f56
+-rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 aioarp-0.0.2/.ruff_cache/content/18bd9323e775c06
+-rw-r--r--   0        0        0     1211 2020-02-02 00:00:00.000000 aioarp-0.0.2/.ruff_cache/content/1cf748db3edf4393
+-rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 aioarp-0.0.2/.ruff_cache/content/1d813f87eae436dc
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 aioarp-0.0.2/.ruff_cache/content/20360c87813708ee
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 aioarp-0.0.2/.ruff_cache/content/20e8c6fb6ec65fba
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 aioarp-0.0.2/.ruff_cache/content/22273ee756d2aeab
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 aioarp-0.0.2/.ruff_cache/content/22eb75e2705cd7cb
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 aioarp-0.0.2/.ruff_cache/content/27380b38303cddd4
+-rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 aioarp-0.0.2/.ruff_cache/content/2894d2afe73e6dee
+-rw-r--r--   0        0        0     2414 2020-02-02 00:00:00.000000 aioarp-0.0.2/.ruff_cache/content/28bfffee8af0f637
+-rw-r--r--   0        0        0     1211 2020-02-02 00:00:00.000000 aioarp-0.0.2/.ruff_cache/content/29a3dfb41b2e153e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 aioarp-0.0.2/.ruff_cache/content/2b17b1ab21ba1879
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 aioarp-0.0.2/.ruff_cache/content/3546886ec7b89ca2
+-rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 aioarp-0.0.2/.ruff_cache/content/44618acc04af2a98
+-rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 aioarp-0.0.2/.ruff_cache/content/464ea8dcb036f50b
+-rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 aioarp-0.0.2/.ruff_cache/content/48dc01dafed313cb
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 aioarp-0.0.2/.ruff_cache/content/53922c565bc4cfdf
+-rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 aioarp-0.0.2/.ruff_cache/content/608e0f7e2331dfd0
+-rw-r--r--   0        0        0     5263 2020-02-02 00:00:00.000000 aioarp-0.0.2/.ruff_cache/content/64f9f289e0610564
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 aioarp-0.0.2/.ruff_cache/content/65bac7c6a4c4cb5e
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 aioarp-0.0.2/.ruff_cache/content/6857c9063a540073
+-rw-r--r--   0        0        0     3069 2020-02-02 00:00:00.000000 aioarp-0.0.2/.ruff_cache/content/6ba798af16bd34e5
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 aioarp-0.0.2/.ruff_cache/content/75d5cb975af2bc07
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 aioarp-0.0.2/.ruff_cache/content/7753615b71d6a36e
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 aioarp-0.0.2/.ruff_cache/content/869f865c9f14daf7
+-rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 aioarp-0.0.2/.ruff_cache/content/936f955f01285847
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 aioarp-0.0.2/.ruff_cache/content/967dc6947ad8c113
+-rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 aioarp-0.0.2/.ruff_cache/content/a12cec0addd27620
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 aioarp-0.0.2/.ruff_cache/content/a64cd85354e281c5
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 aioarp-0.0.2/.ruff_cache/content/b3202a665cec273b
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 aioarp-0.0.2/.ruff_cache/content/bdd7c44b4f88bf5b
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 aioarp-0.0.2/.ruff_cache/content/c0d92e761aa72a56
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 aioarp-0.0.2/.ruff_cache/content/c24cf3b955d01f58
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 aioarp-0.0.2/.ruff_cache/content/c2e7f8eb8bfe8525
+-rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 aioarp-0.0.2/.ruff_cache/content/c78c3248c370d9f2
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 aioarp-0.0.2/.ruff_cache/content/c7a507ee84d3e2ab
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 aioarp-0.0.2/.ruff_cache/content/dc53fc214ceea0dd
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 aioarp-0.0.2/.ruff_cache/content/de93c4dfa993ec19
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 aioarp-0.0.2/.ruff_cache/content/e11920c476dc4f59
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 aioarp-0.0.2/.ruff_cache/content/e12d636458d129da
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 aioarp-0.0.2/.ruff_cache/content/e305b1c5b826225
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 aioarp-0.0.2/.ruff_cache/content/e512a2b647437caa
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 aioarp-0.0.2/.ruff_cache/content/f3ac79af6cdde497
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 aioarp-0.0.2/.ruff_cache/content/f3d289f55f0ad6bd
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 aioarp-0.0.2/.ruff_cache/content/f45e36470415dca1
+-rw-r--r--   0        0        0     3130 2020-02-02 00:00:00.000000 aioarp-0.0.2/.ruff_cache/content/f58c3d661899d706
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 aioarp-0.0.2/.ruff_cache/content/ffe7d79671eca8f
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 aioarp-0.0.2/aioarp/__about__.py
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 aioarp-0.0.2/aioarp/__init__.py
+-rw-r--r--   0        0        0     4727 2020-02-02 00:00:00.000000 aioarp-0.0.2/aioarp/_arp.py
+-rw-r--r--   0        0        0     1372 2020-02-02 00:00:00.000000 aioarp-0.0.2/aioarp/_client.py
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 aioarp-0.0.2/aioarp/_exceptions.py
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 aioarp-0.0.2/aioarp/_mock.py
+-rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 aioarp-0.0.2/aioarp/_utils.py
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 aioarp-0.0.2/aioarp/defaults.py
+-rw-r--r--   0        0        0     1912 2020-02-02 00:00:00.000000 aioarp-0.0.2/aioarp/_async/__init__.py
+-rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 aioarp-0.0.2/aioarp/_sync/__init__.py
+-rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 aioarp-0.0.2/aioarp/backends/_async.py
+-rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 aioarp-0.0.2/aioarp/backends/_sync.py
+-rwxr-xr-x   0        0        0       37 2020-02-02 00:00:00.000000 aioarp-0.0.2/scripts/check
+-rwxr-xr-x   0        0        0       30 2020-02-02 00:00:00.000000 aioarp-0.0.2/scripts/lint
+-rwxr-xr-x   0        0        0       52 2020-02-02 00:00:00.000000 aioarp-0.0.2/scripts/test
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 aioarp-0.0.2/tests/__init__.py
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 aioarp-0.0.2/tests/test_client.py
+-rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 aioarp-0.0.2/tests/test_proto.py
+-rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 aioarp-0.0.2/tests/test_utils.py
+-rw-r--r--   0        0        0     2721 2020-02-02 00:00:00.000000 aioarp-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 aioarp-0.0.2/LICENSE.txt
+-rw-r--r--   0        0        0     4421 2020-02-02 00:00:00.000000 aioarp-0.0.2/README.md
+-rw-r--r--   0        0        0     1332 2020-02-02 00:00:00.000000 aioarp-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     5335 2020-02-02 00:00:00.000000 aioarp-0.0.2/PKG-INFO
```

### Comparing `aioarp-0.0.1/unasync.py` & `aioarp-0.0.2/unasync.py`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.1/.ruff_cache/content/18bd9323e775c06` & `aioarp-0.0.2/.ruff_cache/content/18bd9323e775c06`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.1/.ruff_cache/content/1cf748db3edf4393` & `aioarp-0.0.2/.ruff_cache/content/1cf748db3edf4393`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.1/.ruff_cache/content/1d813f87eae436dc` & `aioarp-0.0.2/.ruff_cache/content/1d813f87eae436dc`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.1/.ruff_cache/content/22273ee756d2aeab` & `aioarp-0.0.2/.ruff_cache/content/22273ee756d2aeab`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.1/.ruff_cache/content/2894d2afe73e6dee` & `aioarp-0.0.2/.ruff_cache/content/2894d2afe73e6dee`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.1/.ruff_cache/content/28bfffee8af0f637` & `aioarp-0.0.2/.ruff_cache/content/28bfffee8af0f637`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.1/.ruff_cache/content/29a3dfb41b2e153e` & `aioarp-0.0.2/.ruff_cache/content/29a3dfb41b2e153e`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.1/.ruff_cache/content/44618acc04af2a98` & `aioarp-0.0.2/.ruff_cache/content/44618acc04af2a98`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.1/.ruff_cache/content/464ea8dcb036f50b` & `aioarp-0.0.2/.ruff_cache/content/464ea8dcb036f50b`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.1/.ruff_cache/content/48dc01dafed313cb` & `aioarp-0.0.2/.ruff_cache/content/48dc01dafed313cb`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.1/.ruff_cache/content/608e0f7e2331dfd0` & `aioarp-0.0.2/.ruff_cache/content/608e0f7e2331dfd0`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.1/.ruff_cache/content/64f9f289e0610564` & `aioarp-0.0.2/.ruff_cache/content/64f9f289e0610564`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.1/.ruff_cache/content/6ba798af16bd34e5` & `aioarp-0.0.2/.ruff_cache/content/6ba798af16bd34e5`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.1/.ruff_cache/content/936f955f01285847` & `aioarp-0.0.2/.ruff_cache/content/936f955f01285847`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.1/.ruff_cache/content/a12cec0addd27620` & `aioarp-0.0.2/.ruff_cache/content/a12cec0addd27620`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.1/.ruff_cache/content/bdd7c44b4f88bf5b` & `aioarp-0.0.2/.ruff_cache/content/bdd7c44b4f88bf5b`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.1/.ruff_cache/content/c78c3248c370d9f2` & `aioarp-0.0.2/.ruff_cache/content/c78c3248c370d9f2`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.1/.ruff_cache/content/e12d636458d129da` & `aioarp-0.0.2/.ruff_cache/content/e12d636458d129da`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.1/.ruff_cache/content/f45e36470415dca1` & `aioarp-0.0.2/.ruff_cache/content/f45e36470415dca1`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.1/.ruff_cache/content/f58c3d661899d706` & `aioarp-0.0.2/.ruff_cache/content/f58c3d661899d706`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.1/aioarp/_arp.py` & `aioarp-0.0.2/aioarp/_arp.py`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.1/aioarp/_client.py` & `aioarp-0.0.2/aioarp/_client.py`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.1/aioarp/_utils.py` & `aioarp-0.0.2/aioarp/_utils.py`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.1/aioarp/_async/__init__.py` & `aioarp-0.0.2/aioarp/_async/__init__.py`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.1/aioarp/_sync/__init__.py` & `aioarp-0.0.2/aioarp/_sync/__init__.py`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.1/aioarp/backends/_async.py` & `aioarp-0.0.2/aioarp/backends/_async.py`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.1/aioarp/backends/_sync.py` & `aioarp-0.0.2/aioarp/backends/_sync.py`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.1/tests/test_client.py` & `aioarp-0.0.2/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.1/tests/test_proto.py` & `aioarp-0.0.2/tests/test_proto.py`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.1/.gitignore` & `aioarp-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.1/LICENSE.txt` & `aioarp-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.1/README.md` & `aioarp-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.1/pyproject.toml` & `aioarp-0.0.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -25,17 +25,17 @@
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
   "anyio"
 ]
 
 [project.urls]
-Documentation = "https://github.com/unknown/aioarp#readme"
-Issues = "https://github.com/unknown/aioarp/issues"
-Source = "https://github.com/unknown/aioarp"
+Documentation = "https://github.com/karosis88/aioarp#readme"
+Issues = "https://github.com/karosis88/aioarp/issues"
+Source = "https://github.com/karosis88/aioarp"
 
 [tool.hatch.version]
 path = "aioarp/__about__.py"
 
 [tool.ruff]
 select = ["E", "F", "I", "B", "PIE"]
 ignore = ["B904", "B028", "F403"]
```

### Comparing `aioarp-0.0.1/PKG-INFO` & `aioarp-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: aioarp
-Version: 0.0.1
-Project-URL: Documentation, https://github.com/unknown/aioarp#readme
-Project-URL: Issues, https://github.com/unknown/aioarp/issues
-Project-URL: Source, https://github.com/unknown/aioarp
+Version: 0.0.2
+Project-URL: Documentation, https://github.com/karosis88/aioarp#readme
+Project-URL: Issues, https://github.com/karosis88/aioarp/issues
+Project-URL: Source, https://github.com/karosis88/aioarp
 Author-email: Karen Petrosyan <kar.petrosyanpy@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

