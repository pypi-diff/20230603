# Comparing `tmp/intercom_test-2.3.0.tar.gz` & `tmp/intercom_test-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/intercom_test-2.3.0.tar", last modified: Fri Oct 22 22:14:22 2021, max compression
+gzip compressed data, was "intercom_test-2.3.1.tar", last modified: Sat Jun  3 06:18:23 2023, max compression
```

## Comparing `intercom_test-2.3.0.tar` & `intercom_test-2.3.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxr-x   0 richardt  (1000) richardt  (1000)        0 2021-10-22 22:14:22.000000 intercom_test-2.3.0/
--rw-rw-r--   0 richardt  (1000) richardt  (1000)       38 2021-10-22 22:14:22.000000 intercom_test-2.3.0/setup.cfg
-drwxrwxr-x   0 richardt  (1000) richardt  (1000)        0 2021-10-22 22:14:22.000000 intercom_test-2.3.0/lib/
-drwxrwxr-x   0 richardt  (1000) richardt  (1000)        0 2021-10-22 22:14:22.000000 intercom_test-2.3.0/lib/intercom_test.egg-info/
--rw-r--r--   0 richardt  (1000) richardt  (1000)      918 2021-10-22 22:14:21.000000 intercom_test-2.3.0/lib/intercom_test.egg-info/SOURCES.txt
--rw-r--r--   0 richardt  (1000) richardt  (1000)        1 2021-10-22 22:14:21.000000 intercom_test-2.3.0/lib/intercom_test.egg-info/dependency_links.txt
--rw-r--r--   0 richardt  (1000) richardt  (1000)       14 2021-10-22 22:14:21.000000 intercom_test-2.3.0/lib/intercom_test.egg-info/top_level.txt
--rw-r--r--   0 richardt  (1000) richardt  (1000)       65 2021-10-22 22:14:21.000000 intercom_test-2.3.0/lib/intercom_test.egg-info/entry_points.txt
--rw-r--r--   0 richardt  (1000) richardt  (1000)      130 2021-10-22 22:14:21.000000 intercom_test-2.3.0/lib/intercom_test.egg-info/requires.txt
--rw-r--r--   0 richardt  (1000) richardt  (1000)    11195 2021-10-22 22:14:21.000000 intercom_test-2.3.0/lib/intercom_test.egg-info/PKG-INFO
-drwxrwxr-x   0 richardt  (1000) richardt  (1000)        0 2021-10-22 22:14:22.000000 intercom_test-2.3.0/lib/intercom_test/
-drwxrwxr-x   0 richardt  (1000) richardt  (1000)        0 2021-10-22 22:14:22.000000 intercom_test-2.3.0/lib/intercom_test/json_asn1/
--rw-r--r--   0 richardt  (1000) richardt  (1000)        0 2021-01-05 03:43:10.000000 intercom_test-2.3.0/lib/intercom_test/json_asn1/__init__.py
--rw-r--r--   0 richardt  (1000) richardt  (1000)     2129 2021-01-05 03:43:10.000000 intercom_test-2.3.0/lib/intercom_test/json_asn1/convert.py
--rw-r--r--   0 richardt  (1000) richardt  (1000)     2039 2021-01-05 03:43:10.000000 intercom_test-2.3.0/lib/intercom_test/json_asn1/types.py
--rw-r--r--   0 richardt  (1000) richardt  (1000)     3391 2021-01-15 22:08:18.000000 intercom_test-2.3.0/lib/intercom_test/yaml_tools.py
--rw-r--r--   0 richardt  (1000) richardt  (1000)     5047 2021-01-12 16:25:51.000000 intercom_test-2.3.0/lib/intercom_test/http_stub_server.py
--rw-rw-r--   0 richardt  (1000) richardt  (1000)    23625 2021-10-22 22:09:53.000000 intercom_test-2.3.0/lib/intercom_test/framework.py
--rw-r--r--   0 richardt  (1000) richardt  (1000)      927 2021-01-05 03:43:10.000000 intercom_test-2.3.0/lib/intercom_test/exceptions.py
--rw-r--r--   0 richardt  (1000) richardt  (1000)     1399 2021-01-13 06:41:33.000000 intercom_test-2.3.0/lib/intercom_test/__init__.py
--rw-r--r--   0 richardt  (1000) richardt  (1000)    11119 2021-01-15 18:04:33.000000 intercom_test-2.3.0/lib/intercom_test/foreign.py
--rw-r--r--   0 richardt  (1000) richardt  (1000)     8466 2021-01-15 18:04:33.000000 intercom_test-2.3.0/lib/intercom_test/utils.py
--rw-r--r--   0 richardt  (1000) richardt  (1000)    26388 2021-01-15 18:04:33.000000 intercom_test-2.3.0/lib/intercom_test/http_best_matches.py
--rw-rw-r--   0 richardt  (1000) richardt  (1000)     1770 2021-10-22 22:09:53.000000 intercom_test-2.3.0/lib/intercom_test/version.py
-drwxrwxr-x   0 richardt  (1000) richardt  (1000)        0 2021-10-22 22:14:22.000000 intercom_test-2.3.0/lib/intercom_test/augmentation/
--rw-rw-r--   0 richardt  (1000) richardt  (1000)     4062 2021-10-22 22:09:53.000000 intercom_test-2.3.0/lib/intercom_test/augmentation/origin_mapping_stream.py
--rw-r--r--   0 richardt  (1000) richardt  (1000)        0 2021-01-05 03:43:10.000000 intercom_test-2.3.0/lib/intercom_test/augmentation/__init__.py
--rw-rw-r--   0 richardt  (1000) richardt  (1000)    13771 2021-10-22 22:09:53.000000 intercom_test-2.3.0/lib/intercom_test/augmentation/update_file.py
--rw-rw-r--   0 richardt  (1000) richardt  (1000)    12008 2021-10-22 22:09:53.000000 intercom_test-2.3.0/lib/intercom_test/augmentation/compact_file.py
--rw-r--r--   0 richardt  (1000) richardt  (1000)     5568 2021-01-13 06:41:33.000000 intercom_test-2.3.0/lib/intercom_test/cases.py
--rw-rw-r--   0 richardt  (1000) richardt  (1000)    31594 2021-10-22 22:09:53.000000 intercom_test-2.3.0/lib/intercom_test/aws_http.py
--rw-r--r--   0 richardt  (1000) richardt  (1000)     9778 2021-01-13 06:53:57.000000 intercom_test-2.3.0/README.md
--rw-r--r--   0 richardt  (1000) richardt  (1000)     2087 2021-01-15 18:04:33.000000 intercom_test-2.3.0/setup.py
--rw-rw-r--   0 richardt  (1000) richardt  (1000)    11195 2021-10-22 22:14:22.000000 intercom_test-2.3.0/PKG-INFO
+drwxrwxr-x   0 rweeks    (1000) rweeks    (1000)        0 2023-06-03 06:18:23.306208 intercom_test-2.3.1/
+-rw-rw-r--   0 rweeks    (1000) rweeks    (1000)    11358 2021-10-22 04:01:23.000000 intercom_test-2.3.1/LICENSE
+-rw-rw-r--   0 rweeks    (1000) rweeks    (1000)    10518 2023-06-03 06:18:23.306208 intercom_test-2.3.1/PKG-INFO
+-rw-rw-r--   0 rweeks    (1000) rweeks    (1000)     9778 2021-10-22 04:01:23.000000 intercom_test-2.3.1/README.md
+drwxrwxr-x   0 rweeks    (1000) rweeks    (1000)        0 2023-06-03 06:18:23.302209 intercom_test-2.3.1/lib/
+drwxrwxr-x   0 rweeks    (1000) rweeks    (1000)        0 2023-06-03 06:18:23.302209 intercom_test-2.3.1/lib/intercom_test/
+-rw-rw-r--   0 rweeks    (1000) rweeks    (1000)     1399 2021-10-22 04:01:23.000000 intercom_test-2.3.1/lib/intercom_test/__init__.py
+drwxrwxr-x   0 rweeks    (1000) rweeks    (1000)        0 2023-06-03 06:18:23.306208 intercom_test-2.3.1/lib/intercom_test/augmentation/
+-rw-rw-r--   0 rweeks    (1000) rweeks    (1000)        0 2021-10-22 04:01:23.000000 intercom_test-2.3.1/lib/intercom_test/augmentation/__init__.py
+-rw-rw-r--   0 rweeks    (1000) rweeks    (1000)    12008 2021-10-22 22:08:23.000000 intercom_test-2.3.1/lib/intercom_test/augmentation/compact_file.py
+-rw-rw-r--   0 rweeks    (1000) rweeks    (1000)     4062 2021-10-22 22:08:23.000000 intercom_test-2.3.1/lib/intercom_test/augmentation/origin_mapping_stream.py
+-rw-rw-r--   0 rweeks    (1000) rweeks    (1000)    13771 2021-10-22 22:08:23.000000 intercom_test-2.3.1/lib/intercom_test/augmentation/update_file.py
+-rw-rw-r--   0 rweeks    (1000) rweeks    (1000)    31594 2021-10-22 22:08:23.000000 intercom_test-2.3.1/lib/intercom_test/aws_http.py
+-rw-rw-r--   0 rweeks    (1000) rweeks    (1000)     5568 2021-10-22 04:01:23.000000 intercom_test-2.3.1/lib/intercom_test/cases.py
+-rw-rw-r--   0 rweeks    (1000) rweeks    (1000)      927 2021-10-22 04:01:23.000000 intercom_test-2.3.1/lib/intercom_test/exceptions.py
+-rw-rw-r--   0 rweeks    (1000) rweeks    (1000)    11381 2023-06-03 06:03:43.000000 intercom_test-2.3.1/lib/intercom_test/foreign.py
+-rw-rw-r--   0 rweeks    (1000) rweeks    (1000)    23625 2021-10-22 22:08:23.000000 intercom_test-2.3.1/lib/intercom_test/framework.py
+-rw-rw-r--   0 rweeks    (1000) rweeks    (1000)    26388 2021-10-22 04:01:23.000000 intercom_test-2.3.1/lib/intercom_test/http_best_matches.py
+drwxrwxr-x   0 rweeks    (1000) rweeks    (1000)        0 2023-06-03 06:18:23.306208 intercom_test-2.3.1/lib/intercom_test/json_asn1/
+-rw-rw-r--   0 rweeks    (1000) rweeks    (1000)        0 2021-10-22 04:01:23.000000 intercom_test-2.3.1/lib/intercom_test/json_asn1/__init__.py
+-rw-rw-r--   0 rweeks    (1000) rweeks    (1000)     2129 2021-10-22 04:01:23.000000 intercom_test-2.3.1/lib/intercom_test/json_asn1/convert.py
+-rw-rw-r--   0 rweeks    (1000) rweeks    (1000)     2039 2021-10-22 04:01:23.000000 intercom_test-2.3.1/lib/intercom_test/json_asn1/types.py
+-rw-rw-r--   0 rweeks    (1000) rweeks    (1000)     8466 2021-10-22 04:01:23.000000 intercom_test-2.3.1/lib/intercom_test/utils.py
+-rw-rw-r--   0 rweeks    (1000) rweeks    (1000)     1807 2023-06-03 06:17:34.000000 intercom_test-2.3.1/lib/intercom_test/version.py
+-rw-rw-r--   0 rweeks    (1000) rweeks    (1000)     3391 2021-10-22 04:01:23.000000 intercom_test-2.3.1/lib/intercom_test/yaml_tools.py
+drwxrwxr-x   0 rweeks    (1000) rweeks    (1000)        0 2023-06-03 06:18:23.306208 intercom_test-2.3.1/lib/intercom_test.egg-info/
+-rw-rw-r--   0 rweeks    (1000) rweeks    (1000)    10518 2023-06-03 06:18:23.000000 intercom_test-2.3.1/lib/intercom_test.egg-info/PKG-INFO
+-rw-rw-r--   0 rweeks    (1000) rweeks    (1000)      888 2023-06-03 06:18:23.000000 intercom_test-2.3.1/lib/intercom_test.egg-info/SOURCES.txt
+-rw-rw-r--   0 rweeks    (1000) rweeks    (1000)        1 2023-06-03 06:18:23.000000 intercom_test-2.3.1/lib/intercom_test.egg-info/dependency_links.txt
+-rw-rw-r--   0 rweeks    (1000) rweeks    (1000)       65 2023-06-03 06:18:23.000000 intercom_test-2.3.1/lib/intercom_test.egg-info/entry_points.txt
+-rw-rw-r--   0 rweeks    (1000) rweeks    (1000)      130 2023-06-03 06:18:23.000000 intercom_test-2.3.1/lib/intercom_test.egg-info/requires.txt
+-rw-rw-r--   0 rweeks    (1000) rweeks    (1000)       14 2023-06-03 06:18:23.000000 intercom_test-2.3.1/lib/intercom_test.egg-info/top_level.txt
+-rw-rw-r--   0 rweeks    (1000) rweeks    (1000)       38 2023-06-03 06:18:23.306208 intercom_test-2.3.1/setup.cfg
+-rw-rw-r--   0 rweeks    (1000) rweeks    (1000)     2087 2023-06-03 06:03:43.000000 intercom_test-2.3.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `intercom_test-2.3.0/lib/intercom_test.egg-info/SOURCES.txt` & `intercom_test-2.3.1/lib/intercom_test.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,17 @@
+LICENSE
 README.md
 setup.py
 lib/intercom_test/__init__.py
 lib/intercom_test/aws_http.py
 lib/intercom_test/cases.py
 lib/intercom_test/exceptions.py
 lib/intercom_test/foreign.py
 lib/intercom_test/framework.py
 lib/intercom_test/http_best_matches.py
-lib/intercom_test/http_stub_server.py
 lib/intercom_test/utils.py
 lib/intercom_test/version.py
 lib/intercom_test/yaml_tools.py
 lib/intercom_test.egg-info/PKG-INFO
 lib/intercom_test.egg-info/SOURCES.txt
 lib/intercom_test.egg-info/dependency_links.txt
 lib/intercom_test.egg-info/entry_points.txt
```

### Comparing `intercom_test-2.3.0/lib/intercom_test.egg-info/PKG-INFO` & `intercom_test-2.3.1/lib/intercom_test.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,105 +1,108 @@
 Metadata-Version: 2.1
 Name: intercom-test
-Version: 2.3.0
+Version: 2.3.1
 Summary: Inter-component testing support code for "Interface By Example"
 Home-page: https://github.com/PayTrace/intercom_test
 Author: Richard T. Weeks
 Author-email: rtweeks21@gmail.com
 License: Apache License 2.0
-Description: 
-        # The intercom_test Package
-        
-        This package provides Python tools to facilitate _Interface by Example_ programming.
-        
-        Test case data is stored in YAML to provide the widest possible access by tools and programming languages while still being friendly to the humans who often need to manually manipulate it.
-        
-        Package documentation is available at [Read the Docs][docs].
-        
-        ## Interface by Example
-        
-        Integration testing has developed a reputation as a gigantic money- and time-suck occurring near the end of a project.  Software components are built _to specification_ in isolation from one another then, near the end of the project, stood up in an actual environment to finally talk to one another.  Inevitably, the two components disagreed on the proper interpretation of some aspect of specifications (think of NASA's lost Mars orbiter), leading to miscommunication or misdesign.  Though the very end of the project is not the best time to discover a need for significant changes, as there is limited opportunity to trade out lower-priority work for the changes required for successful integration, this is exactly when such issues will be discovered.
-        
-        Beyond the downsides of traditional integration testing enumerated above, the Agile philosophy espouses a general feeling that "Specifications documents are wrong."  This is not saying they are wrong in the sense that writing them is wrong, but that the documents themselves are _providing wrong information_ by:
-        
-        * Giving incomplete and/or ambiguous specifications
-        * Contradicting the actual implementation and usage
-        * Falling out of date with the implementation
-        * Being more rigid than necessary, promoting byzantine implementations
-        * Only being testable by writing test code, which may be buggy
-        
-        In essence, this is another way of saying "If it isn't tested, it isn't true."
-        
-        A more Agile approach is to document exact input/output pairs conforming to the desired interface.  Consumers of the interface can use these examples to configure mock responses during unit testing, while providers/implementers of the interface can test against the specified cases.  If both consumers and providers are testing against the same cases, a much greater degree of confidence can be developed that both sides are "speaking the same language."
-        
-        While *intercom_test* is a good tool for testing and communication, it is not a replacement for good communication between the teams developing the service provider and consumer.  Just because the consumer team adds a test case to the interface file does not create a guarantee that the provider could _ever_ make the test pass.  But the consumer development team could use *intercom_test* files to _propose_ a change to the team implementing the provider...in language much less ambiguous than is found in most interface specification documents.
-        
-        
-        ## Test Case Format
-        
-        Each test case is viewed as a `dict` of values to be consumed by the application's testing system, either as a feasible request/response pair for stubbing in a consumer or as a request/response pair with additional data for generating an integration test case for a provider.
-        
-        This library provides an iterable of test cases or test case runner callables.  As detailed below, these test cases can come from multiple data files and may be a merge of information in more than one file.  Within the data files, test case data is represented in YAML.
-        
-        ## Challenges Solved
-        
-        * Correlating augmenting data for the service provider
-        * Maintaining augmenting data for the service provider
-        * Merging new test cases
-        
-        
-        ### Correlating Augmenting Data for the Service Provider
-        
-        The basic idea of storing machine-readable request/response pairs in a shared "repository" between service consumers and providers is straightforward.  The first difficulty arises because service consumers need only the request/response pair for testing where service providers typically need to establish some particular state and/or mocks of other external services for the test cases to pass.  This information will typically be tightly coupled to the provider's implementation (e.g. it's database tables) and really should not be shared as part of the interface example.  This raises the problem of correlating the _augmenting data_ for the service provider with the test case data shared by both components.
-        
-        The first reasonable solution might be to insist that each test case provide an unique identifier which could be used to look up the augmenting data in a dictionary- or hashtable-like structure.  This is feasible but still puts an additional burden on the format of the data in the shared test cases: it must now incorporate this unique identifier in some way.  This unique identifier is also not typically helpful to the interface consumer and thus constitutes noise on that side of the interface.  The unique identifier also, and subtly as shown below, allows bad behavior by provider-test writers.
-        
-        An alternative is to derive a hash value for each test case from the key fields of the request.  Since the consumer needs each response to have a different request to effectively make all test case responses available, this also helps to identify cases in the test set where different responses are indicated for the same request.  Using this correlation method, it will be difficult for all the provider-side tests to pass as the provider-side can only have a single augmenting data set correlated with the _request_; when using unique identifiers, the provider side can test multiple cases with different augmentation data for the same request, subtly breaking the consumers' ability to use tests.  Because interface consumers benefit by being able to actually invoke each response, this is the better (if more complicated) solution and the one taken by *intercom_test*.
-        
-        Typically, the interface case data will be stored in a directory that is shared between consumers and providers (e.g. a Git submodule, a Subversion external) where the augmentation data would live in the same repository as the test code for the provider.  This reduces exposure of implementation details, loosening the coupling between providers and consumers.  It also reduces churn in the interface case files, especially where changes to the persistent storage of the provider occur.
-        
-        
-        ### Maintaining Augmenting Data for the Service Provider
-        
-        While the hash value derived for identifying the test case described in the previous section works well for _implementation_ of this library, it is much more difficult for a human to use that hash value to correlate the augmenting data with the test case.  Essentially, making a new entry in the compact data format file manually is not feasible.  *intercom_test* incorporates functionality to update such high-performance files from a more human-friendly format, which identifies the test case simply by copying the whole case from the shared interface file and adding new keys to the `dict`.  If the test case runner is wrapped by the provided decorator function (possibly through generation of *case runners*), the compact format data files will be automatically updated from these programmer-friendly _update files_ when all of the interface tests pass.
-        
-        Beyond automatically wrapping the test function in the compact data updating decorator, the *case runners* that *intercom_test* can generate have an additional advantage: they automatically log the case data they are about to test.  If the testing framework captures and displays logging events for failed tests, it becomes simple to paste the test case data into an update file, alter it as necessary to get the test passing, and have the compact data file automatically updated with the new, correct test data.
-        
-        
-        ## Merging New Test Cases
-        
-        The simplest organization of the shared test case data (i.e. the request/response pair) would be to put them in a single file using a file format supporting a data sequence: e.g. JSON, XML, or YAML.  This becomes problematic when two branches of development both try to add new items at the end of the file, which inevitably causes a merge conflict.  While this conflict is predictable and fairly easily managed with good tools, it would be preferable to avoid the conflict in the normal course of development.
-        
-        This essentially means distributing the test cases through multiple files.  *intercom_test* provides facilities for organizing test cases in multiple files and combining them in a predictable, mergeable way as and when desired.
-        
-        
-        ## Command Line Interface (`[cli]` Extra)
-        
-        When this package is installed with the `[cli]` extra, it makes a command line tool called `icy-test` available to access the core functionality of `intercom_test`, facilitating use of this functionality in languages other than Python.  Help on use of the tool can be obtained by running `icy-test --help`.
-        
-        
-        ## Contributing
-        
-        1. Fork it ( https://github.com/PayTrace/intercom_test )
-        2. Create your feature branch (`git checkout -b my-new-feature`)
-        3. Commit your changes (`git commit -am 'Add some feature'`)
-        4. Push to the branch (`git push origin my-new-feature`)
-        5. Create new Pull Request (on [GitHub](https://github.com))
-        
-        PayTrace uses *intercom_test* for coordinating testing of protocols between our components, and we consider this library to be in _alpha status_ at this time. It is under active development and maintenance! For further details on contributing, see [CONTRIBUTING.md](./CONTRIBUTING.md).
-        
-        ## TL; DR
-        
-        This package allows a cheaper version of integration tests to run as part of unit testing.  It reads and maintains the data files necessary for this style of testing.  Service providers and consumers maintain parity by testing with the same test cases.
-        
-        [docs]: https://intercom-test.readthedocs.io/en/latest/
-        
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Other Audience
 Classifier: Topic :: Software Development :: Testing
 Description-Content-Type: text/markdown
 Provides-Extra: cli
+License-File: LICENSE
+
+
+# The intercom_test Package
+
+This package provides Python tools to facilitate _Interface by Example_ programming.
+
+Test case data is stored in YAML to provide the widest possible access by tools and programming languages while still being friendly to the humans who often need to manually manipulate it.
+
+Package documentation is available at [Read the Docs][docs].
+
+## Interface by Example
+
+Integration testing has developed a reputation as a gigantic money- and time-suck occurring near the end of a project.  Software components are built _to specification_ in isolation from one another then, near the end of the project, stood up in an actual environment to finally talk to one another.  Inevitably, the two components disagreed on the proper interpretation of some aspect of specifications (think of NASA's lost Mars orbiter), leading to miscommunication or misdesign.  Though the very end of the project is not the best time to discover a need for significant changes, as there is limited opportunity to trade out lower-priority work for the changes required for successful integration, this is exactly when such issues will be discovered.
+
+Beyond the downsides of traditional integration testing enumerated above, the Agile philosophy espouses a general feeling that "Specifications documents are wrong."  This is not saying they are wrong in the sense that writing them is wrong, but that the documents themselves are _providing wrong information_ by:
+
+* Giving incomplete and/or ambiguous specifications
+* Contradicting the actual implementation and usage
+* Falling out of date with the implementation
+* Being more rigid than necessary, promoting byzantine implementations
+* Only being testable by writing test code, which may be buggy
+
+In essence, this is another way of saying "If it isn't tested, it isn't true."
+
+A more Agile approach is to document exact input/output pairs conforming to the desired interface.  Consumers of the interface can use these examples to configure mock responses during unit testing, while providers/implementers of the interface can test against the specified cases.  If both consumers and providers are testing against the same cases, a much greater degree of confidence can be developed that both sides are "speaking the same language."
+
+While *intercom_test* is a good tool for testing and communication, it is not a replacement for good communication between the teams developing the service provider and consumer.  Just because the consumer team adds a test case to the interface file does not create a guarantee that the provider could _ever_ make the test pass.  But the consumer development team could use *intercom_test* files to _propose_ a change to the team implementing the provider...in language much less ambiguous than is found in most interface specification documents.
+
+
+## Test Case Format
+
+Each test case is viewed as a `dict` of values to be consumed by the application's testing system, either as a feasible request/response pair for stubbing in a consumer or as a request/response pair with additional data for generating an integration test case for a provider.
+
+This library provides an iterable of test cases or test case runner callables.  As detailed below, these test cases can come from multiple data files and may be a merge of information in more than one file.  Within the data files, test case data is represented in YAML.
+
+## Challenges Solved
+
+* Correlating augmenting data for the service provider
+* Maintaining augmenting data for the service provider
+* Merging new test cases
+
+
+### Correlating Augmenting Data for the Service Provider
+
+The basic idea of storing machine-readable request/response pairs in a shared "repository" between service consumers and providers is straightforward.  The first difficulty arises because service consumers need only the request/response pair for testing where service providers typically need to establish some particular state and/or mocks of other external services for the test cases to pass.  This information will typically be tightly coupled to the provider's implementation (e.g. it's database tables) and really should not be shared as part of the interface example.  This raises the problem of correlating the _augmenting data_ for the service provider with the test case data shared by both components.
+
+The first reasonable solution might be to insist that each test case provide an unique identifier which could be used to look up the augmenting data in a dictionary- or hashtable-like structure.  This is feasible but still puts an additional burden on the format of the data in the shared test cases: it must now incorporate this unique identifier in some way.  This unique identifier is also not typically helpful to the interface consumer and thus constitutes noise on that side of the interface.  The unique identifier also, and subtly as shown below, allows bad behavior by provider-test writers.
+
+An alternative is to derive a hash value for each test case from the key fields of the request.  Since the consumer needs each response to have a different request to effectively make all test case responses available, this also helps to identify cases in the test set where different responses are indicated for the same request.  Using this correlation method, it will be difficult for all the provider-side tests to pass as the provider-side can only have a single augmenting data set correlated with the _request_; when using unique identifiers, the provider side can test multiple cases with different augmentation data for the same request, subtly breaking the consumers' ability to use tests.  Because interface consumers benefit by being able to actually invoke each response, this is the better (if more complicated) solution and the one taken by *intercom_test*.
+
+Typically, the interface case data will be stored in a directory that is shared between consumers and providers (e.g. a Git submodule, a Subversion external) where the augmentation data would live in the same repository as the test code for the provider.  This reduces exposure of implementation details, loosening the coupling between providers and consumers.  It also reduces churn in the interface case files, especially where changes to the persistent storage of the provider occur.
+
+
+### Maintaining Augmenting Data for the Service Provider
+
+While the hash value derived for identifying the test case described in the previous section works well for _implementation_ of this library, it is much more difficult for a human to use that hash value to correlate the augmenting data with the test case.  Essentially, making a new entry in the compact data format file manually is not feasible.  *intercom_test* incorporates functionality to update such high-performance files from a more human-friendly format, which identifies the test case simply by copying the whole case from the shared interface file and adding new keys to the `dict`.  If the test case runner is wrapped by the provided decorator function (possibly through generation of *case runners*), the compact format data files will be automatically updated from these programmer-friendly _update files_ when all of the interface tests pass.
+
+Beyond automatically wrapping the test function in the compact data updating decorator, the *case runners* that *intercom_test* can generate have an additional advantage: they automatically log the case data they are about to test.  If the testing framework captures and displays logging events for failed tests, it becomes simple to paste the test case data into an update file, alter it as necessary to get the test passing, and have the compact data file automatically updated with the new, correct test data.
+
+
+## Merging New Test Cases
+
+The simplest organization of the shared test case data (i.e. the request/response pair) would be to put them in a single file using a file format supporting a data sequence: e.g. JSON, XML, or YAML.  This becomes problematic when two branches of development both try to add new items at the end of the file, which inevitably causes a merge conflict.  While this conflict is predictable and fairly easily managed with good tools, it would be preferable to avoid the conflict in the normal course of development.
+
+This essentially means distributing the test cases through multiple files.  *intercom_test* provides facilities for organizing test cases in multiple files and combining them in a predictable, mergeable way as and when desired.
+
+
+## Command Line Interface (`[cli]` Extra)
+
+When this package is installed with the `[cli]` extra, it makes a command line tool called `icy-test` available to access the core functionality of `intercom_test`, facilitating use of this functionality in languages other than Python.  Help on use of the tool can be obtained by running `icy-test --help`.
+
+
+## Contributing
+
+1. Fork it ( https://github.com/PayTrace/intercom_test )
+2. Create your feature branch (`git checkout -b my-new-feature`)
+3. Commit your changes (`git commit -am 'Add some feature'`)
+4. Push to the branch (`git push origin my-new-feature`)
+5. Create new Pull Request (on [GitHub](https://github.com))
+
+PayTrace uses *intercom_test* for coordinating testing of protocols between our components, and we consider this library to be in _alpha status_ at this time. It is under active development and maintenance! For further details on contributing, see [CONTRIBUTING.md](./CONTRIBUTING.md).
+
+## TL; DR
+
+This package allows a cheaper version of integration tests to run as part of unit testing.  It reads and maintains the data files necessary for this style of testing.  Service providers and consumers maintain parity by testing with the same test cases.
+
+[docs]: https://intercom-test.readthedocs.io/en/latest/
+
+
```

### Comparing `intercom_test-2.3.0/lib/intercom_test/json_asn1/convert.py` & `intercom_test-2.3.1/lib/intercom_test/json_asn1/convert.py`

 * *Files identical despite different names*

### Comparing `intercom_test-2.3.0/lib/intercom_test/json_asn1/types.py` & `intercom_test-2.3.1/lib/intercom_test/json_asn1/types.py`

 * *Files identical despite different names*

### Comparing `intercom_test-2.3.0/lib/intercom_test/yaml_tools.py` & `intercom_test-2.3.1/lib/intercom_test/yaml_tools.py`

 * *Files identical despite different names*

### Comparing `intercom_test-2.3.0/lib/intercom_test/framework.py` & `intercom_test-2.3.1/lib/intercom_test/framework.py`

 * *Files identical despite different names*

### Comparing `intercom_test-2.3.0/lib/intercom_test/exceptions.py` & `intercom_test-2.3.1/lib/intercom_test/exceptions.py`

 * *Files identical despite different names*

### Comparing `intercom_test-2.3.0/lib/intercom_test/__init__.py` & `intercom_test-2.3.1/lib/intercom_test/__init__.py`

 * *Files identical despite different names*

### Comparing `intercom_test-2.3.0/lib/intercom_test/foreign.py` & `intercom_test-2.3.1/lib/intercom_test/foreign.py`

 * *Files 4% similar despite different names*

```diff
@@ -115,14 +115,16 @@
     
     CASE_AUGMENTATION_KEYS = frozenset(('augmentation data', 'request keys'))
     
     case_augmenter = None
     request_keys = ()
     
     def __init__(self, filepath):
+        if filepath is None:
+            raise RuntimeError("Path to config file must be specified")
         super(Config, self).__init__()
         with open(filepath) as cfgfile:
             cfg_data = yaml.safe_load(cfgfile)
         
         ref_dir = os.path.dirname(filepath)
         
         self.interface_dir = os.path.join(ref_dir, cfg_data['interfaces'])
@@ -196,14 +198,17 @@
     """usage: {program} init [options]
     
     Interactively create a configuration file
     
     Options:
         -c CONFFILE, --config CONFFILE      path to configuration file
     """
+    if options.get('--config') is None:
+        print("REQUIRED: Use -c/--config to specify config file to write")
+        raise SystemExit(2)
     if not Config.build_with_cui(options['--config']):
         print("*** Canceled by user ***")
         raise SystemExit(1)
 
 @subcommand()
 def enumerate(options):
     """usage: {program} enumerate [options]
@@ -315,15 +320,15 @@
         add_request_keys=config.request_keys,
     )
     
     for line in sys.stdin:
         database.json_exchange(line, sys.stdout)
 
 def csmain():
-    main(sys.argv[0], _package_version)
+    main(os.path.basename(sys.argv[0]), _package_version)
 
 if __name__ == '__main__':
     my_name = os.path.splitext(os.path.basename(__file__))[0]
     
     # NOTE: Cannot use "python -m{}.{}" as the format string because docopt
     # interprets the "-m..." as flags to the program.
     main("{}.{}".format(_package, my_name), _package_version)
```

### Comparing `intercom_test-2.3.0/lib/intercom_test/utils.py` & `intercom_test-2.3.1/lib/intercom_test/utils.py`

 * *Files identical despite different names*

### Comparing `intercom_test-2.3.0/lib/intercom_test/http_best_matches.py` & `intercom_test-2.3.1/lib/intercom_test/http_best_matches.py`

 * *Files identical despite different names*

### Comparing `intercom_test-2.3.0/lib/intercom_test/version.py` & `intercom_test-2.3.1/lib/intercom_test/version.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-_nominal_version = "2.3.0"
+_nominal_version = "2.3.1"
 
 import os.path
 import subprocess
 import sys
 
 class VersionInfo:
     version_unknown = False
@@ -43,14 +43,14 @@
     
     def get_version_unknown(self, ):
         return self._git_cmd_for_vtag("rev-parse --verify --quiet", stdout=subprocess.DEVNULL)
     
     def _git_cmd_for_vtag(self, cmd_str, *, subp='call', **kwargs):
         try:
             return getattr(subprocess, subp)(
-                ["git"] + cmd_str.split() + [self.version_tag],
+                ["git", "-C", os.path.dirname(self.git_dir)] + cmd_str.split() + [self.version_tag],
                 **kwargs
             )
         except FileNotFoundError:
             return None
 
 __version__ = VersionInfo(_nominal_version).actual_version
```

### Comparing `intercom_test-2.3.0/lib/intercom_test/augmentation/origin_mapping_stream.py` & `intercom_test-2.3.1/lib/intercom_test/augmentation/origin_mapping_stream.py`

 * *Files identical despite different names*

### Comparing `intercom_test-2.3.0/lib/intercom_test/augmentation/update_file.py` & `intercom_test-2.3.1/lib/intercom_test/augmentation/update_file.py`

 * *Files identical despite different names*

### Comparing `intercom_test-2.3.0/lib/intercom_test/augmentation/compact_file.py` & `intercom_test-2.3.1/lib/intercom_test/augmentation/compact_file.py`

 * *Files identical despite different names*

### Comparing `intercom_test-2.3.0/lib/intercom_test/cases.py` & `intercom_test-2.3.1/lib/intercom_test/cases.py`

 * *Files identical despite different names*

### Comparing `intercom_test-2.3.0/lib/intercom_test/aws_http.py` & `intercom_test-2.3.1/lib/intercom_test/aws_http.py`

 * *Files identical despite different names*

### Comparing `intercom_test-2.3.0/README.md` & `intercom_test-2.3.1/README.md`

 * *Files identical despite different names*

### Comparing `intercom_test-2.3.0/setup.py` & `intercom_test-2.3.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     install_requires=[
         'PyYAML >=3.11, <6',
         'pyasn1 >=0.4.2, <1',
         'packaging >=20.8, <21',
         'python-Levenshtein >=0.12, <1',
     ],
     extras_require={
-        'cli': ['docopt-subcommands>=3.0, <4', 'pick>=0.6.4, <1'],
+        'cli': ['docopt-subcommands>=3.0, <4', 'pick>=1.6.0, <2'],
     },
     entry_points={
         'console_scripts': [
             'icy-test = intercom_test.foreign:csmain [cli]',
         ],
     },
     classifiers=[
```

### Comparing `intercom_test-2.3.0/PKG-INFO` & `intercom_test-2.3.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,105 +1,108 @@
 Metadata-Version: 2.1
 Name: intercom_test
-Version: 2.3.0
+Version: 2.3.1
 Summary: Inter-component testing support code for "Interface By Example"
 Home-page: https://github.com/PayTrace/intercom_test
 Author: Richard T. Weeks
 Author-email: rtweeks21@gmail.com
 License: Apache License 2.0
-Description: 
-        # The intercom_test Package
-        
-        This package provides Python tools to facilitate _Interface by Example_ programming.
-        
-        Test case data is stored in YAML to provide the widest possible access by tools and programming languages while still being friendly to the humans who often need to manually manipulate it.
-        
-        Package documentation is available at [Read the Docs][docs].
-        
-        ## Interface by Example
-        
-        Integration testing has developed a reputation as a gigantic money- and time-suck occurring near the end of a project.  Software components are built _to specification_ in isolation from one another then, near the end of the project, stood up in an actual environment to finally talk to one another.  Inevitably, the two components disagreed on the proper interpretation of some aspect of specifications (think of NASA's lost Mars orbiter), leading to miscommunication or misdesign.  Though the very end of the project is not the best time to discover a need for significant changes, as there is limited opportunity to trade out lower-priority work for the changes required for successful integration, this is exactly when such issues will be discovered.
-        
-        Beyond the downsides of traditional integration testing enumerated above, the Agile philosophy espouses a general feeling that "Specifications documents are wrong."  This is not saying they are wrong in the sense that writing them is wrong, but that the documents themselves are _providing wrong information_ by:
-        
-        * Giving incomplete and/or ambiguous specifications
-        * Contradicting the actual implementation and usage
-        * Falling out of date with the implementation
-        * Being more rigid than necessary, promoting byzantine implementations
-        * Only being testable by writing test code, which may be buggy
-        
-        In essence, this is another way of saying "If it isn't tested, it isn't true."
-        
-        A more Agile approach is to document exact input/output pairs conforming to the desired interface.  Consumers of the interface can use these examples to configure mock responses during unit testing, while providers/implementers of the interface can test against the specified cases.  If both consumers and providers are testing against the same cases, a much greater degree of confidence can be developed that both sides are "speaking the same language."
-        
-        While *intercom_test* is a good tool for testing and communication, it is not a replacement for good communication between the teams developing the service provider and consumer.  Just because the consumer team adds a test case to the interface file does not create a guarantee that the provider could _ever_ make the test pass.  But the consumer development team could use *intercom_test* files to _propose_ a change to the team implementing the provider...in language much less ambiguous than is found in most interface specification documents.
-        
-        
-        ## Test Case Format
-        
-        Each test case is viewed as a `dict` of values to be consumed by the application's testing system, either as a feasible request/response pair for stubbing in a consumer or as a request/response pair with additional data for generating an integration test case for a provider.
-        
-        This library provides an iterable of test cases or test case runner callables.  As detailed below, these test cases can come from multiple data files and may be a merge of information in more than one file.  Within the data files, test case data is represented in YAML.
-        
-        ## Challenges Solved
-        
-        * Correlating augmenting data for the service provider
-        * Maintaining augmenting data for the service provider
-        * Merging new test cases
-        
-        
-        ### Correlating Augmenting Data for the Service Provider
-        
-        The basic idea of storing machine-readable request/response pairs in a shared "repository" between service consumers and providers is straightforward.  The first difficulty arises because service consumers need only the request/response pair for testing where service providers typically need to establish some particular state and/or mocks of other external services for the test cases to pass.  This information will typically be tightly coupled to the provider's implementation (e.g. it's database tables) and really should not be shared as part of the interface example.  This raises the problem of correlating the _augmenting data_ for the service provider with the test case data shared by both components.
-        
-        The first reasonable solution might be to insist that each test case provide an unique identifier which could be used to look up the augmenting data in a dictionary- or hashtable-like structure.  This is feasible but still puts an additional burden on the format of the data in the shared test cases: it must now incorporate this unique identifier in some way.  This unique identifier is also not typically helpful to the interface consumer and thus constitutes noise on that side of the interface.  The unique identifier also, and subtly as shown below, allows bad behavior by provider-test writers.
-        
-        An alternative is to derive a hash value for each test case from the key fields of the request.  Since the consumer needs each response to have a different request to effectively make all test case responses available, this also helps to identify cases in the test set where different responses are indicated for the same request.  Using this correlation method, it will be difficult for all the provider-side tests to pass as the provider-side can only have a single augmenting data set correlated with the _request_; when using unique identifiers, the provider side can test multiple cases with different augmentation data for the same request, subtly breaking the consumers' ability to use tests.  Because interface consumers benefit by being able to actually invoke each response, this is the better (if more complicated) solution and the one taken by *intercom_test*.
-        
-        Typically, the interface case data will be stored in a directory that is shared between consumers and providers (e.g. a Git submodule, a Subversion external) where the augmentation data would live in the same repository as the test code for the provider.  This reduces exposure of implementation details, loosening the coupling between providers and consumers.  It also reduces churn in the interface case files, especially where changes to the persistent storage of the provider occur.
-        
-        
-        ### Maintaining Augmenting Data for the Service Provider
-        
-        While the hash value derived for identifying the test case described in the previous section works well for _implementation_ of this library, it is much more difficult for a human to use that hash value to correlate the augmenting data with the test case.  Essentially, making a new entry in the compact data format file manually is not feasible.  *intercom_test* incorporates functionality to update such high-performance files from a more human-friendly format, which identifies the test case simply by copying the whole case from the shared interface file and adding new keys to the `dict`.  If the test case runner is wrapped by the provided decorator function (possibly through generation of *case runners*), the compact format data files will be automatically updated from these programmer-friendly _update files_ when all of the interface tests pass.
-        
-        Beyond automatically wrapping the test function in the compact data updating decorator, the *case runners* that *intercom_test* can generate have an additional advantage: they automatically log the case data they are about to test.  If the testing framework captures and displays logging events for failed tests, it becomes simple to paste the test case data into an update file, alter it as necessary to get the test passing, and have the compact data file automatically updated with the new, correct test data.
-        
-        
-        ## Merging New Test Cases
-        
-        The simplest organization of the shared test case data (i.e. the request/response pair) would be to put them in a single file using a file format supporting a data sequence: e.g. JSON, XML, or YAML.  This becomes problematic when two branches of development both try to add new items at the end of the file, which inevitably causes a merge conflict.  While this conflict is predictable and fairly easily managed with good tools, it would be preferable to avoid the conflict in the normal course of development.
-        
-        This essentially means distributing the test cases through multiple files.  *intercom_test* provides facilities for organizing test cases in multiple files and combining them in a predictable, mergeable way as and when desired.
-        
-        
-        ## Command Line Interface (`[cli]` Extra)
-        
-        When this package is installed with the `[cli]` extra, it makes a command line tool called `icy-test` available to access the core functionality of `intercom_test`, facilitating use of this functionality in languages other than Python.  Help on use of the tool can be obtained by running `icy-test --help`.
-        
-        
-        ## Contributing
-        
-        1. Fork it ( https://github.com/PayTrace/intercom_test )
-        2. Create your feature branch (`git checkout -b my-new-feature`)
-        3. Commit your changes (`git commit -am 'Add some feature'`)
-        4. Push to the branch (`git push origin my-new-feature`)
-        5. Create new Pull Request (on [GitHub](https://github.com))
-        
-        PayTrace uses *intercom_test* for coordinating testing of protocols between our components, and we consider this library to be in _alpha status_ at this time. It is under active development and maintenance! For further details on contributing, see [CONTRIBUTING.md](./CONTRIBUTING.md).
-        
-        ## TL; DR
-        
-        This package allows a cheaper version of integration tests to run as part of unit testing.  It reads and maintains the data files necessary for this style of testing.  Service providers and consumers maintain parity by testing with the same test cases.
-        
-        [docs]: https://intercom-test.readthedocs.io/en/latest/
-        
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Other Audience
 Classifier: Topic :: Software Development :: Testing
 Description-Content-Type: text/markdown
 Provides-Extra: cli
+License-File: LICENSE
+
+
+# The intercom_test Package
+
+This package provides Python tools to facilitate _Interface by Example_ programming.
+
+Test case data is stored in YAML to provide the widest possible access by tools and programming languages while still being friendly to the humans who often need to manually manipulate it.
+
+Package documentation is available at [Read the Docs][docs].
+
+## Interface by Example
+
+Integration testing has developed a reputation as a gigantic money- and time-suck occurring near the end of a project.  Software components are built _to specification_ in isolation from one another then, near the end of the project, stood up in an actual environment to finally talk to one another.  Inevitably, the two components disagreed on the proper interpretation of some aspect of specifications (think of NASA's lost Mars orbiter), leading to miscommunication or misdesign.  Though the very end of the project is not the best time to discover a need for significant changes, as there is limited opportunity to trade out lower-priority work for the changes required for successful integration, this is exactly when such issues will be discovered.
+
+Beyond the downsides of traditional integration testing enumerated above, the Agile philosophy espouses a general feeling that "Specifications documents are wrong."  This is not saying they are wrong in the sense that writing them is wrong, but that the documents themselves are _providing wrong information_ by:
+
+* Giving incomplete and/or ambiguous specifications
+* Contradicting the actual implementation and usage
+* Falling out of date with the implementation
+* Being more rigid than necessary, promoting byzantine implementations
+* Only being testable by writing test code, which may be buggy
+
+In essence, this is another way of saying "If it isn't tested, it isn't true."
+
+A more Agile approach is to document exact input/output pairs conforming to the desired interface.  Consumers of the interface can use these examples to configure mock responses during unit testing, while providers/implementers of the interface can test against the specified cases.  If both consumers and providers are testing against the same cases, a much greater degree of confidence can be developed that both sides are "speaking the same language."
+
+While *intercom_test* is a good tool for testing and communication, it is not a replacement for good communication between the teams developing the service provider and consumer.  Just because the consumer team adds a test case to the interface file does not create a guarantee that the provider could _ever_ make the test pass.  But the consumer development team could use *intercom_test* files to _propose_ a change to the team implementing the provider...in language much less ambiguous than is found in most interface specification documents.
+
+
+## Test Case Format
+
+Each test case is viewed as a `dict` of values to be consumed by the application's testing system, either as a feasible request/response pair for stubbing in a consumer or as a request/response pair with additional data for generating an integration test case for a provider.
+
+This library provides an iterable of test cases or test case runner callables.  As detailed below, these test cases can come from multiple data files and may be a merge of information in more than one file.  Within the data files, test case data is represented in YAML.
+
+## Challenges Solved
+
+* Correlating augmenting data for the service provider
+* Maintaining augmenting data for the service provider
+* Merging new test cases
+
+
+### Correlating Augmenting Data for the Service Provider
+
+The basic idea of storing machine-readable request/response pairs in a shared "repository" between service consumers and providers is straightforward.  The first difficulty arises because service consumers need only the request/response pair for testing where service providers typically need to establish some particular state and/or mocks of other external services for the test cases to pass.  This information will typically be tightly coupled to the provider's implementation (e.g. it's database tables) and really should not be shared as part of the interface example.  This raises the problem of correlating the _augmenting data_ for the service provider with the test case data shared by both components.
+
+The first reasonable solution might be to insist that each test case provide an unique identifier which could be used to look up the augmenting data in a dictionary- or hashtable-like structure.  This is feasible but still puts an additional burden on the format of the data in the shared test cases: it must now incorporate this unique identifier in some way.  This unique identifier is also not typically helpful to the interface consumer and thus constitutes noise on that side of the interface.  The unique identifier also, and subtly as shown below, allows bad behavior by provider-test writers.
+
+An alternative is to derive a hash value for each test case from the key fields of the request.  Since the consumer needs each response to have a different request to effectively make all test case responses available, this also helps to identify cases in the test set where different responses are indicated for the same request.  Using this correlation method, it will be difficult for all the provider-side tests to pass as the provider-side can only have a single augmenting data set correlated with the _request_; when using unique identifiers, the provider side can test multiple cases with different augmentation data for the same request, subtly breaking the consumers' ability to use tests.  Because interface consumers benefit by being able to actually invoke each response, this is the better (if more complicated) solution and the one taken by *intercom_test*.
+
+Typically, the interface case data will be stored in a directory that is shared between consumers and providers (e.g. a Git submodule, a Subversion external) where the augmentation data would live in the same repository as the test code for the provider.  This reduces exposure of implementation details, loosening the coupling between providers and consumers.  It also reduces churn in the interface case files, especially where changes to the persistent storage of the provider occur.
+
+
+### Maintaining Augmenting Data for the Service Provider
+
+While the hash value derived for identifying the test case described in the previous section works well for _implementation_ of this library, it is much more difficult for a human to use that hash value to correlate the augmenting data with the test case.  Essentially, making a new entry in the compact data format file manually is not feasible.  *intercom_test* incorporates functionality to update such high-performance files from a more human-friendly format, which identifies the test case simply by copying the whole case from the shared interface file and adding new keys to the `dict`.  If the test case runner is wrapped by the provided decorator function (possibly through generation of *case runners*), the compact format data files will be automatically updated from these programmer-friendly _update files_ when all of the interface tests pass.
+
+Beyond automatically wrapping the test function in the compact data updating decorator, the *case runners* that *intercom_test* can generate have an additional advantage: they automatically log the case data they are about to test.  If the testing framework captures and displays logging events for failed tests, it becomes simple to paste the test case data into an update file, alter it as necessary to get the test passing, and have the compact data file automatically updated with the new, correct test data.
+
+
+## Merging New Test Cases
+
+The simplest organization of the shared test case data (i.e. the request/response pair) would be to put them in a single file using a file format supporting a data sequence: e.g. JSON, XML, or YAML.  This becomes problematic when two branches of development both try to add new items at the end of the file, which inevitably causes a merge conflict.  While this conflict is predictable and fairly easily managed with good tools, it would be preferable to avoid the conflict in the normal course of development.
+
+This essentially means distributing the test cases through multiple files.  *intercom_test* provides facilities for organizing test cases in multiple files and combining them in a predictable, mergeable way as and when desired.
+
+
+## Command Line Interface (`[cli]` Extra)
+
+When this package is installed with the `[cli]` extra, it makes a command line tool called `icy-test` available to access the core functionality of `intercom_test`, facilitating use of this functionality in languages other than Python.  Help on use of the tool can be obtained by running `icy-test --help`.
+
+
+## Contributing
+
+1. Fork it ( https://github.com/PayTrace/intercom_test )
+2. Create your feature branch (`git checkout -b my-new-feature`)
+3. Commit your changes (`git commit -am 'Add some feature'`)
+4. Push to the branch (`git push origin my-new-feature`)
+5. Create new Pull Request (on [GitHub](https://github.com))
+
+PayTrace uses *intercom_test* for coordinating testing of protocols between our components, and we consider this library to be in _alpha status_ at this time. It is under active development and maintenance! For further details on contributing, see [CONTRIBUTING.md](./CONTRIBUTING.md).
+
+## TL; DR
+
+This package allows a cheaper version of integration tests to run as part of unit testing.  It reads and maintains the data files necessary for this style of testing.  Service providers and consumers maintain parity by testing with the same test cases.
+
+[docs]: https://intercom-test.readthedocs.io/en/latest/
+
+
```

