# Comparing `tmp/streams.py-0.1.3.tar.gz` & `tmp/streams_py-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streams.py-0.1.3.tar", last modified: Tue Dec  6 16:07:33 2022, max compression
+gzip compressed data, was "streams_py-0.2.tar", max compression
```

## Comparing `streams.py-0.1.3.tar` & `streams_py-0.2.tar`

### file list

```diff
@@ -1,30 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 16:07:33.515545 streams.py-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2022-12-06 16:07:17.000000 streams.py-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       34 2022-12-06 16:07:17.000000 streams.py-0.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    12504 2022-12-06 16:07:33.515545 streams.py-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11949 2022-12-06 16:07:17.000000 streams.py-0.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       80 2022-12-06 16:07:17.000000 streams.py-0.1.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 16:07:33.511546 streams.py-0.1.3/pystreamapi/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2022-12-06 16:07:17.000000 streams.py-0.1.3/pystreamapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      336 2022-12-06 16:07:17.000000 streams.py-0.1.3/pystreamapi/__iterate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2439 2022-12-06 16:07:17.000000 streams.py-0.1.3/pystreamapi/__stream.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 16:07:33.511546 streams.py-0.1.3/pystreamapi/lazy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-06 16:07:17.000000 streams.py-0.1.3/pystreamapi/lazy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2022-12-06 16:07:17.000000 streams.py-0.1.3/pystreamapi/lazy/process.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2022-12-06 16:07:17.000000 streams.py-0.1.3/pystreamapi/lazy/queue.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 16:07:33.511546 streams.py-0.1.3/pystreamapi/parallel/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-06 16:07:17.000000 streams.py-0.1.3/pystreamapi/parallel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2022-12-06 16:07:17.000000 streams.py-0.1.3/pystreamapi/parallel/itertools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 16:07:33.515545 streams.py-0.1.3/pystreamapi/streams/
--rw-r--r--   0 runner    (1001) docker     (123)     9405 2022-12-06 16:07:17.000000 streams.py-0.1.3/pystreamapi/streams/__base_stream.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-06 16:07:17.000000 streams.py-0.1.3/pystreamapi/streams/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3344 2022-12-06 16:07:17.000000 streams.py-0.1.3/pystreamapi/streams/__parallel_stream.py
--rw-r--r--   0 runner    (1001) docker     (123)     2646 2022-12-06 16:07:17.000000 streams.py-0.1.3/pystreamapi/streams/__sequential_stream.py
--rw-r--r--   0 runner    (1001) docker     (123)      820 2022-12-06 16:07:33.515545 streams.py-0.1.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 16:07:33.515545 streams.py-0.1.3/streams.py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12504 2022-12-06 16:07:33.000000 streams.py-0.1.3/streams.py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      628 2022-12-06 16:07:33.000000 streams.py-0.1.3/streams.py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-06 16:07:33.000000 streams.py-0.1.3/streams.py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2022-12-06 16:07:33.000000 streams.py-0.1.3/streams.py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2022-12-06 16:07:33.000000 streams.py-0.1.3/streams.py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-06 16:07:33.000000 streams.py-0.1.3/streams.py.egg-info/zip-safe
+-rw-r--r--   0        0        0    35149 2023-06-03 14:38:14.090693 streams_py-0.2/LICENSE
+-rw-r--r--   0        0        0     9389 2023-06-03 14:38:14.090693 streams_py-0.2/README.md
+-rw-r--r--   0        0        0      750 2023-06-03 14:38:14.094693 streams_py-0.2/pyproject.toml
+-rw-r--r--   0        0        0       82 2023-06-03 14:38:14.094693 streams_py-0.2/pystreamapi/__init__.py
+-rw-r--r--   0        0        0      336 2023-06-03 14:38:14.094693 streams_py-0.2/pystreamapi/__iterate.py
+-rw-r--r--   0        0        0     3483 2023-06-03 14:38:14.094693 streams_py-0.2/pystreamapi/__stream.py
+-rw-r--r--   0        0        0        0 2023-06-03 14:38:14.094693 streams_py-0.2/pystreamapi/_lazy/__init__.py
+-rw-r--r--   0        0        0      626 2023-06-03 14:38:14.094693 streams_py-0.2/pystreamapi/_lazy/process.py
+-rw-r--r--   0        0        0      593 2023-06-03 14:38:14.094693 streams_py-0.2/pystreamapi/_lazy/queue.py
+-rw-r--r--   0        0        0        0 2023-06-03 14:38:14.094693 streams_py-0.2/pystreamapi/_parallel/__init__.py
+-rw-r--r--   0        0        0     2970 2023-06-03 14:38:14.094693 streams_py-0.2/pystreamapi/_parallel/fork_and_join.py
+-rw-r--r--   0        0        0    10186 2023-06-03 14:38:14.094693 streams_py-0.2/pystreamapi/_streams/__base_stream.py
+-rw-r--r--   0        0        0        0 2023-06-03 14:38:14.094693 streams_py-0.2/pystreamapi/_streams/__init__.py
+-rw-r--r--   0        0        0     3733 2023-06-03 14:38:14.094693 streams_py-0.2/pystreamapi/_streams/__parallel_stream.py
+-rw-r--r--   0        0        0     2672 2023-06-03 14:38:14.094693 streams_py-0.2/pystreamapi/_streams/__sequential_stream.py
+-rw-r--r--   0        0        0     3020 2023-06-03 14:38:14.094693 streams_py-0.2/pystreamapi/_streams/numeric/__numeric_base_stream.py
+-rw-r--r--   0        0        0      646 2023-06-03 14:38:14.094693 streams_py-0.2/pystreamapi/_streams/numeric/__parallel_numeric_stream.py
+-rw-r--r--   0        0        0      508 2023-06-03 14:38:14.094693 streams_py-0.2/pystreamapi/_streams/numeric/__sequential_numeric_stream.py
+-rw-r--r--   0        0        0      221 2023-06-03 14:38:14.094693 streams_py-0.2/pystreamapi/conditions/__init__.py
+-rw-r--r--   0        0        0      307 2023-06-03 14:38:14.094693 streams_py-0.2/pystreamapi/conditions/combiners.py
+-rw-r--r--   0        0        0     9223 2023-06-03 14:38:14.094693 streams_py-0.2/pystreamapi/conditions/date.py
+-rw-r--r--   0        0        0     4937 2023-06-03 14:38:14.094693 streams_py-0.2/pystreamapi/conditions/numeric.py
+-rw-r--r--   0        0        0     1385 2023-06-03 14:38:14.094693 streams_py-0.2/pystreamapi/conditions/string.py
+-rw-r--r--   0        0        0      735 2023-06-03 14:38:14.094693 streams_py-0.2/pystreamapi/conditions/types.py
+-rw-r--r--   0        0        0    10290 1970-01-01 00:00:00.000000 streams_py-0.2/PKG-INFO
```

### Comparing `streams.py-0.1.3/LICENSE` & `streams_py-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `streams.py-0.1.3/pystreamapi/lazy/process.py` & `streams_py-0.2/pystreamapi/_lazy/process.py`

 * *Files identical despite different names*

### Comparing `streams.py-0.1.3/pystreamapi/lazy/queue.py` & `streams_py-0.2/pystreamapi/_lazy/queue.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pystreamapi.lazy.process import Process
+from pystreamapi._lazy.process import Process
 
 
 class ProcessQueue:
     """A Queue for processes"""
 
     def __init__(self):
         self.__queue: List[Process] = []
```

### Comparing `streams.py-0.1.3/pystreamapi/streams/__base_stream.py` & `streams_py-0.2/pystreamapi/_streams/__base_stream.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,245 +1,256 @@
 import itertools
 from abc import abstractmethod
 from builtins import reversed
 from functools import cmp_to_key
-from typing import Iterable, Callable, Any, TypeVar, Iterator
+from typing import Iterable, Callable, Any, TypeVar, Iterator, Union
 
 from optional import Optional
+from optional.nothing import Nothing
+from optional.something import Something
 
-from pystreamapi.lazy.process import Process
-from pystreamapi.lazy.queue import ProcessQueue
+from pystreamapi._lazy.process import Process
+from pystreamapi._lazy.queue import ProcessQueue
 
-_K = TypeVar('_K')
+K = TypeVar('K')
 _V = TypeVar('_V')
+_identity_missing = object()
 
 
-class BaseStream(Iterable[_K]):
+class BaseStream(Iterable[K]):
     """
     A sequence of elements supporting sequential and parallel aggregate operations.
 
     To perform a computation, stream operations are composed into a stream pipeline. A stream
     pipeline consists of a source (which might be an array, a collection, a generator function,
     an I/O channel, etc.), zero or more intermediate operations (which transform a stream into
     another stream, such as filter(Predicate)), and a terminal operation (which produces a result
     or side effect, such as count() or forEach(Consumer)). Streams are lazy; computation on the
     source data is only performed when the terminal operation is initiated, and source elements
     are consumed only as needed.
     """
 
-    def __init__(self, source: Iterable[_K]):
+    def __init__(self, source: Iterable[K]):
         self._source = source
         self._queue = ProcessQueue()
 
-    def __iter__(self) -> Iterator[_K]:
+    def __iter__(self) -> Iterator[K]:
         self._trigger_exec()
         return iter(self._source)
 
-    def __reversed__(self):
-        self.__reversed()
-        return self
-
     @classmethod
-    def concat(cls, *streams: "BaseStream[_K]"):
+    def concat(cls, *streams: "BaseStream[K]"):
         """
         Creates a lazily concatenated stream whose elements are all the elements of the first stream
         followed by all the elements of the other streams.
 
         :param streams: The streams to concatenate
         :return: The concatenated stream
         """
         return cls(itertools.chain(*list(streams)))
 
+    def distinct(self) -> 'BaseStream[_V]':
+        """Returns a stream consisting of the distinct elements of this stream."""
+        self._queue.append(Process(self.__distinct))
+        return self
+
+    def __distinct(self):
+        """Removes duplicate elements from the stream."""
+        self._source = list(set(self._source))
+
+    def drop_while(self, predicate: Callable[[K], bool]) -> 'BaseStream[_V]':
+        """
+        Returns, if this stream is ordered, a stream consisting of the remaining elements of this
+        stream after dropping the longest prefix of elements that match the given predicate.
+
+        :param predicate:
+        """
+        self._queue.append(Process(self.__drop_while, predicate))
+        return self
+
+    def __drop_while(self, predicate: Callable[[Any], bool]):
+        """Drops elements from the stream while the predicate is true."""
+        self._source = list(itertools.dropwhile(predicate, self._source))
+
     @abstractmethod
-    def filter(self, predicate: Callable[[_K], bool]):
+    def filter(self, predicate: Callable[[K], bool]) -> 'BaseStream[_V]':
         """
         Returns a stream consisting of the elements of this stream that match the given predicate.
 
         :param predicate:
         """
+
+    @abstractmethod
+    def flat_map(self, predicate: Callable[[K], Iterable[_V]]) -> 'BaseStream[_V]':
+        """
+        Returns a stream consisting of the results of replacing each element of this stream with
+        the contents of a mapped stream produced by applying the provided mapping function to
+        each element.
+
+        :param predicate:
+        """
+
+    def limit(self, max_size: int) -> 'BaseStream[_V]':
+        """
+        Returns a stream consisting of the elements of this stream, truncated to be no longer
+        than maxSize in length.
+
+        :param max_size:
+        """
+        self._queue.append(Process(self.__limit, max_size))
         return self
 
+    def __limit(self, max_size: int):
+        """Limits the stream to the first n elements."""
+        self._source = itertools.islice(self._source, max_size)
+
     @abstractmethod
-    def map(self, mapper: Callable[[_K], _V]) -> 'BaseStream[_V]':
+    def map(self, mapper: Callable[[K], _V]) -> 'BaseStream[_V]':
         """
         Returns a stream consisting of the results of applying the given function to the elements
         of this stream.
 
         :param mapper:
         """
-        return self
 
     @abstractmethod
-    def map_to_int(self):
+    def map_to_int(self) -> 'BaseStream[_V]':
         """
         Returns a stream consisting of the results of converting the elements of this stream to
         integers.
         """
-        return self
 
     @abstractmethod
-    def map_to_str(self):
+    def map_to_str(self) -> 'BaseStream[_V]':
         """
         Returns a stream consisting of the results of converting the elements of this stream to
         strings.
         """
-        return self
-
-    @abstractmethod
-    def flat_map(self, predicate: Callable[[_K], Iterable[_V]]):
-        """
-        Returns a stream consisting of the results of replacing each element of this stream with
-        the contents of a mapped stream produced by applying the provided mapping function to
-        each element.
-
-        :param predicate:
-        """
-        return self
 
     @abstractmethod
-    def peek(self, action: Callable):
+    def peek(self, action: Callable) -> 'BaseStream[_V]':
         """
         Returns a stream consisting of the elements of this stream, additionally performing the
         provided action on each element as elements are consumed from the resulting stream.
 
         :param action:
         """
-        return self
 
-    def limit(self, max_size: int):
+    def reversed(self) -> 'BaseStream[_V]':
         """
-        Returns a stream consisting of the elements of this stream, truncated to be no longer
-        than maxSize in length.
-
-        :param max_size:
+        Returns a stream consisting of the elements of this stream, with their order being
+        reversed.
         """
-        self._queue.append(Process(self.__limit, max_size))
+        self._queue.append(Process(self.__reversed))
         return self
 
-    def __limit(self, max_size: int):
-        self._source = itertools.islice(self._source, max_size)
+    def __reversed(self):
+        """Reverses the stream."""
+        try:
+            self._source = reversed(self._source)
+        except TypeError:
+            self._source = reversed(list(self._source))
 
-    def skip(self, n: int):
+    def skip(self, n: int) -> 'BaseStream[_V]':
         """
         Returns a stream consisting of the remaining elements of this stream after discarding the
         first n elements of the stream.
 
         :param n:
         """
         self._queue.append(Process(self.__skip, n))
         return self
 
     def __skip(self, n: int):
+        """Skips the first n elements of the stream."""
         self._source = self._source[n:]
 
-    def distinct(self):
-        """Returns a stream consisting of the distinct elements of this stream."""
-        self._queue.append(Process(self.__distinct))
-        return self
-
-    def __distinct(self):
-        self._source = list(set(self._source))
-
-    def sorted(self, comparator: Callable[[_K], int] = None):
+    def sorted(self, comparator: Callable[[K], int] = None) -> 'BaseStream[_V]':
         """
         Returns a stream consisting of the elements of this stream, sorted according to natural
         order.
         """
         self._queue.append(Process(self.__sorted, comparator))
         return self
 
-    def __sorted(self, comparator: Callable[[_K], int] = None):
+    def __sorted(self, comparator: Callable[[K], int] = None):
+        """Sorts the stream."""
         if comparator is None:
             self._source = sorted(self._source)
         else:
             self._source = sorted(self._source, key=cmp_to_key(comparator))
 
-    def reversed(self):
-        """
-        Returns a stream consisting of the elements of this stream, with their order being
-        reversed.
-        """
-        self._queue.append(Process(self.__reversed))
-        return self
-
-    def __reversed(self):
-        try:
-            self._source = reversed(self._source)
-        except TypeError:
-            self._source = reversed(list(self._source))
-
-    def drop_while(self, predicate: Callable[[_K], bool]):
-        """
-        Returns, if this stream is ordered, a stream consisting of the remaining elements of this
-        stream after dropping the longest prefix of elements that match the given predicate.
-
-        :param predicate:
-        """
-        self._queue.append(Process(self.__drop_while, predicate))
-        return self
-
-    def __drop_while(self, predicate: Callable[[Any], bool]):
-        self._source = list(itertools.dropwhile(predicate, self._source))
-
-    def take_while(self, predicate: Callable[[_K], bool]):
+    def take_while(self, predicate: Callable[[K], bool]) -> 'BaseStream[_V]':
         """
         Returns, if this stream is ordered, a stream consisting of the longest prefix of elements
         taken from this stream that match the given predicate.
 
         :param predicate:
         """
         self._queue.append(Process(self.__take_while, predicate))
         return self
 
     def __take_while(self, predicate: Callable[[Any], bool]):
+        """Takes elements from the stream while the predicate is true."""
         self._source = list(itertools.takewhile(predicate, self._source))
 
+    # Terminal Operations:
+
     @abstractmethod
-    def find_any(self) -> Optional:
+    def all_match(self, predicate: Callable[[K], bool]):
         """
-        Returns an Optional describing some element of the stream, or an empty Optional if the
-        stream is empty.
+        Returns whether all elements of this stream match the provided predicate.
+
+        :param predicate: The callable predicate
         """
 
-    @abstractmethod
-    def for_each(self, predicate: Callable):
+    def any_match(self, predicate: Callable[[K], bool]):
         """
-        Performs an action for each element of this stream.
+        Returns whether any elements of this stream match the provided predicate.
 
-        :param predicate:
+        :param predicate: The callable predicate
         """
+        self._trigger_exec()
+        return any(predicate(element) for element in self._source)
 
-    @abstractmethod
-    def reduce(self, predicate: Callable[[_K, _K], _K], identity) -> _K:
+    def count(self):
         """
-        Performs a reduction on the elements of this stream, using the provided identity value
-        and an associative accumulation function, and returns the reduced value.
+        Returns the count of elements in this stream.
 
-        :param predicate:
-        :param identity:
+        :return: Number of elements in the stream
         """
+        self._trigger_exec()
+        return len(self._source)
 
     @abstractmethod
-    def all_match(self, predicate: Callable[[_K], bool]):
+    def find_any(self) -> Optional:
+        """
+        Returns an Optional describing some element of the stream, or an empty Optional if the
+        stream is empty.
         """
-        Returns whether all elements of this stream match the provided predicate.
 
-        :param predicate: The callable predicate
+    def find_first(self):
         """
+        Returns an Optional describing the first element of this stream, or an empty Optional if
+        the stream is empty. :return:
+        """
+        self._trigger_exec()
+        if len(self._source) > 0:
+            return Optional.of(self._source[0])
+        return Optional.empty()
 
-    def any_match(self, predicate: Callable[[_K], bool]):
+    @abstractmethod
+    def for_each(self, predicate: Callable):
         """
-        Returns whether any elements of this stream match the provided predicate.
+        Performs an action for each element of this stream.
 
-        :param predicate: The callable predicate
+        :param predicate:
         """
-        self._trigger_exec()
-        return any(predicate(element) for element in self._source)
 
-    def none_match(self, predicate: Callable[[_K], bool]):
+    def none_match(self, predicate: Callable[[K], bool]):
         """
         Returns whether no elements of this stream match the provided predicate.
 
         :param predicate:
         """
         self._trigger_exec()
         return not any(predicate(element) for element in self._source)
@@ -254,23 +265,25 @@
     def max(self):
         """Returns the maximum element of this stream."""
         self._trigger_exec()
         if len(self._source) > 0:
             return Optional.of(max(self._source))
         return Optional.empty()
 
-    def find_first(self):
+    @abstractmethod
+    def reduce(self, predicate: Callable[[K, K], K], identity=_identity_missing,
+               depends_on_state=False) -> Union[K, Something, Nothing]:
         """
-        Returns an Optional describing the first element of this stream, or an empty Optional if
-        the stream is empty. :return:
+        Performs a reduction on the elements of this stream, using the provided identity value
+        and an associative accumulation function, and returns the reduced value.
+
+        :param depends_on_state: Weather processing order changes result or not
+        :param predicate:
+        :param identity: Default value
         """
-        self._trigger_exec()
-        if len(self._source) > 0:
-            return Optional.of(self._source[0])
-        return Optional.empty()
 
     def to_list(self):
         """Accumulates the elements of this stream into a List."""
         self._trigger_exec()
         return list(self._source)
 
     def to_tuple(self):
@@ -279,18 +292,10 @@
         return tuple(self._source)
 
     def to_set(self):
         """Accumulates the elements of this stream into a Set."""
         self._trigger_exec()
         return set(self._source)
 
-    def count(self):
-        """
-        Returns the count of elements in this stream.
-
-        :return: Number of elements in the stream
-        """
-        self._trigger_exec()
-        return len(self._source)
-
     def _trigger_exec(self):
+        """Triggers execution of the stream."""
         self._queue.execute_all()
```

### Comparing `streams.py-0.1.3/pystreamapi/streams/__parallel_stream.py` & `streams_py-0.2/pystreamapi/_streams/__parallel_stream.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,61 @@
-from typing import Callable, Any
 from functools import reduce as seq_reduce
+from typing import Callable, Any, Iterable
+
 from joblib import Parallel, delayed
 from optional import Optional
 
-import pystreamapi.streams.__base_stream as stream
-from pystreamapi.lazy.process import Process
-from pystreamapi.parallel.itertools import reduce, pfilter
+import pystreamapi._streams.__base_stream as stream
+from pystreamapi._lazy.process import Process
+from pystreamapi._parallel.fork_and_join import Parallelizer
 
 _identity_missing = object()
 
 
 class ParallelStream(stream.BaseStream):
     """The parallel implementation of BaseStream"""
 
+    def __init__(self, source: Iterable[stream.K]):
+        super().__init__(source)
+        self.parallelizer = Parallelizer()
+
+    def all_match(self, predicate: Callable[[Any], bool]):
+        self._trigger_exec()
+        return all(Parallel(n_jobs=-1, prefer="threads")(delayed(predicate)(element)
+                                                         for element in self._source))
+
     def filter(self, predicate: Callable[[Any], bool]):
         self._queue.append(Process(self.__filter, predicate))
         return self
 
     def __filter(self, predicate: Callable[[Any], bool]):
-        self._source = pfilter(self._source, predicate)
+        self._set_parallelizer_src()
+        self._source = self.parallelizer.filter(predicate)
+
+    def find_any(self):
+        self._trigger_exec()
+        if len(self._source) > 0:
+            return Optional.of(self._source[0])
+        return Optional.empty()
+
+    def flat_map(self, predicate: Callable[[Any], stream.BaseStream]):
+        self._queue.append(Process(self.__flat_map, predicate))
+        return self
+
+    def __flat_map(self, predicate: Callable[[Any], stream.BaseStream]):
+        new_src = []
+        for element in Parallel(n_jobs=-1, prefer="threads")(delayed(predicate)(element)
+                                                             for element in self._source):
+            new_src.extend(element.to_list())
+        self._source = new_src
+
+    def for_each(self, predicate: Callable):
+        self._trigger_exec()
+        Parallel(n_jobs=-1, prefer="threads")(delayed(predicate)(element)
+                                              for element in self._source)
 
     def map(self, mapper: Callable[[Any], Any]):
         self._queue.append(Process(self.__map, mapper))
         return self
 
     def __map(self, predicate: Callable[[Any], Any]):
         self._source = Parallel(n_jobs=-1, prefer="threads")(delayed(predicate)(element)
@@ -38,51 +71,31 @@
     def map_to_str(self):
         self._queue.append(Process(self.__map_to_str))
         return self
 
     def __map_to_str(self):
         self.__map(str)
 
-    def flat_map(self, predicate: Callable[[Any], stream.BaseStream]):
-        self._queue.append(Process(self.__flat_map, predicate))
-        return self
-
-    def __flat_map(self, predicate: Callable[[Any], stream.BaseStream]):
-        new_src = []
-        for element in Parallel(n_jobs=-1, prefer="threads")(delayed(predicate)(element)
-                                                             for element in self._source):
-            new_src.extend(element.to_list())
-        self._source = new_src
-
     def peek(self, action: Callable):
         self._queue.append(Process(self.__peek, action))
         return self
 
     def __peek(self, predicate: Callable):
         Parallel(n_jobs=-1, prefer="threads")(delayed(predicate)(element)
                                               for element in self._source)
 
     def reduce(self, predicate: Callable[[Any, Any], Any], identity=_identity_missing,
-               depends_on_state=True):
+               depends_on_state=False):
         self._trigger_exec()
-        reduce_func = reduce if depends_on_state is False else seq_reduce
+        self._set_parallelizer_src()
+        reduce_func = seq_reduce if depends_on_state else self.__reduce
         if len(self._source) > 0:
             if identity is not _identity_missing:
                 return reduce_func(predicate, self._source)
             return Optional.of(reduce_func(predicate, self._source))
         return identity if identity is not _identity_missing else Optional.empty()
 
-    def all_match(self, predicate: Callable[[Any], bool]):
-        self._trigger_exec()
-        return all(Parallel(n_jobs=-1, prefer="threads")(delayed(predicate)(element)
-                                                         for element in self._source))
+    def __reduce(self, pred, _):
+        return self.parallelizer.reduce(pred)
 
-    def find_any(self):
-        self._trigger_exec()
-        if len(self._source) > 0:
-            return Optional.of(self._source[0])
-        return Optional.empty()
-
-    def for_each(self, predicate: Callable):
-        self._trigger_exec()
-        Parallel(n_jobs=-1, prefer="threads")(delayed(predicate)(element)
-                                              for element in self._source)
+    def _set_parallelizer_src(self):
+        self.parallelizer.set_source(self._source)
```

### Comparing `streams.py-0.1.3/pystreamapi/streams/__sequential_stream.py` & `streams_py-0.2/pystreamapi/_streams/__sequential_stream.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,53 @@
 from functools import reduce
 from typing import Callable, Any
 
 from optional import Optional
 
-import pystreamapi.streams.__base_stream as stream
-from pystreamapi.lazy.process import Process
+import pystreamapi._streams.__base_stream as stream
+from pystreamapi._lazy.process import Process
 
 _identity_missing = object()
 
 
 class SequentialStream(stream.BaseStream):
     """The sequential implementation of BaseStream"""
 
+    def all_match(self, predicate: Callable[[Any], bool]):
+        self._trigger_exec()
+        return all(predicate(element) for element in self._source)
+
     def filter(self, predicate: Callable[[Any], bool]):
         self._queue.append(Process(self.__filter, predicate))
         return self
 
     def __filter(self, predicate: Callable[[Any], bool]):
         self._source = [element for element in self._source if predicate(element)]
 
+    def find_any(self):
+        self._trigger_exec()
+        if len(self._source) > 0:
+            return Optional.of(self._source[0])
+        return Optional.empty()
+
+    def flat_map(self, predicate: Callable[[Any], stream.BaseStream]):
+        self._queue.append(Process(self.__flat_map, predicate))
+        return self
+
+    def __flat_map(self, predicate: Callable[[Any], stream.BaseStream]):
+        new_src = []
+        for element in [predicate(element) for element in self._source]:
+            new_src.extend(element.to_list())
+        self._source = new_src
+
+    def for_each(self, predicate: Callable):
+        self._trigger_exec()
+        for element in self._source:
+            predicate(element)
+
     def map(self, mapper: Callable[[Any], Any]):
         self._queue.append(Process(self.__map, mapper))
         return self
 
     def __map(self, predicate: Callable[[Any], Any]):
         self._source = [predicate(element) for element in self._source]
 
@@ -36,47 +61,22 @@
     def map_to_str(self):
         self._queue.append(Process(self.__map_to_str))
         return self
 
     def __map_to_str(self):
         self.__map(str)
 
-    def flat_map(self, predicate: Callable[[Any], stream.BaseStream]):
-        self._queue.append(Process(self.__flat_map, predicate))
-        return self
-
-    def __flat_map(self, predicate: Callable[[Any], stream.BaseStream]):
-        new_src = []
-        for element in [predicate(element) for element in self._source]:
-            new_src.extend(element.to_list())
-        self._source = new_src
-
     def peek(self, action: Callable):
         self._queue.append(Process(self.__peek, action))
         return self
 
     def __peek(self, predicate: Callable):
         for element in self._source:
             predicate(element)
 
-    def reduce(self, predicate: Callable, identity=_identity_missing):
+    def reduce(self, predicate: Callable, identity=_identity_missing, depends_on_state=False):
         self._trigger_exec()
         if len(self._source) > 0:
             if identity is not _identity_missing:
                 return reduce(predicate, self._source)
             return Optional.of(reduce(predicate, self._source))
         return identity if identity is not _identity_missing else Optional.empty()
-
-    def all_match(self, predicate: Callable[[Any], bool]):
-        self._trigger_exec()
-        return all(predicate(element) for element in self._source)
-
-    def find_any(self):
-        self._trigger_exec()
-        if len(self._source) > 0:
-            return Optional.of(self._source[0])
-        return Optional.empty()
-
-    def for_each(self, predicate: Callable):
-        self._trigger_exec()
-        for element in self._source:
-            predicate(element)
```

