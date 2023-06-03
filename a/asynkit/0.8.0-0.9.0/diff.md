# Comparing `tmp/asynkit-0.8.0.tar.gz` & `tmp/asynkit-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asynkit-0.8.0.tar", max compression
+gzip compressed data, was "asynkit-0.9.0.tar", max compression
```

## Comparing `asynkit-0.8.0.tar` & `asynkit-0.9.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1081 2023-05-21 13:35:17.074606 asynkit-0.8.0/LICENSE
--rw-r--r--   0        0        0    18163 2023-05-21 13:35:17.074606 asynkit-0.8.0/README.md
--rw-r--r--   0        0        0     1884 2023-05-21 13:35:17.074606 asynkit-0.8.0/pyproject.toml
--rw-r--r--   0        0        0      224 2023-05-21 13:35:17.074606 asynkit-0.8.0/src/asynkit/__init__.py
--rw-r--r--   0        0        0     1357 2023-05-21 13:35:17.074606 asynkit-0.8.0/src/asynkit/compat.py
--rw-r--r--   0        0        0    12701 2023-05-21 13:35:17.074606 asynkit-0.8.0/src/asynkit/coroutine.py
--rw-r--r--   0        0        0        0 2023-05-21 13:35:17.074606 asynkit-0.8.0/src/asynkit/experimental/__init__.py
--rw-r--r--   0        0        0     4293 2023-05-21 13:35:17.074606 asynkit-0.8.0/src/asynkit/experimental/anyio.py
--rw-r--r--   0        0        0        0 2023-05-21 13:35:17.074606 asynkit-0.8.0/src/asynkit/loop/__init__.py
--rw-r--r--   0        0        0     4164 2023-05-21 13:35:17.074606 asynkit-0.8.0/src/asynkit/loop/default.py
--rw-r--r--   0        0        0     4815 2023-05-21 13:35:17.074606 asynkit-0.8.0/src/asynkit/loop/eventloop.py
--rw-r--r--   0        0        0     2981 2023-05-21 13:35:17.074606 asynkit-0.8.0/src/asynkit/loop/extensions.py
--rw-r--r--   0        0        0     2922 2023-05-21 13:35:17.074606 asynkit-0.8.0/src/asynkit/loop/schedulingloop.py
--rw-r--r--   0        0        0      281 2023-05-21 13:35:17.074606 asynkit-0.8.0/src/asynkit/loop/types.py
--rw-r--r--   0        0        0    10597 2023-05-21 13:35:17.074606 asynkit-0.8.0/src/asynkit/monitor.py
--rw-r--r--   0        0        0        0 2023-05-21 13:35:17.074606 asynkit-0.8.0/src/asynkit/py.typed
--rw-r--r--   0        0        0     5352 2023-05-21 13:35:17.074606 asynkit-0.8.0/src/asynkit/scheduling.py
--rw-r--r--   0        0        0     1209 2023-05-21 13:35:17.074606 asynkit-0.8.0/src/asynkit/tools.py
--rw-r--r--   0        0        0    19113 1970-01-01 00:00:00.000000 asynkit-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-06-03 12:49:45.045481 asynkit-0.9.0/LICENSE
+-rw-r--r--   0        0        0    21296 2023-06-03 12:49:45.045481 asynkit-0.9.0/README.md
+-rw-r--r--   0        0        0     2078 2023-06-03 12:49:45.045481 asynkit-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0      124 2023-06-03 12:49:45.045481 asynkit-0.9.0/src/asynkit/__init__.py
+-rw-r--r--   0        0        0     1357 2023-06-03 12:49:45.045481 asynkit-0.9.0/src/asynkit/compat.py
+-rw-r--r--   0        0        0    17091 2023-06-03 12:49:45.045481 asynkit-0.9.0/src/asynkit/coroutine.py
+-rw-r--r--   0        0        0        0 2023-06-03 12:49:45.045481 asynkit-0.9.0/src/asynkit/experimental/__init__.py
+-rw-r--r--   0        0        0     4293 2023-06-03 12:49:45.045481 asynkit-0.9.0/src/asynkit/experimental/anyio.py
+-rw-r--r--   0        0        0        0 2023-06-03 12:49:45.045481 asynkit-0.9.0/src/asynkit/loop/__init__.py
+-rw-r--r--   0        0        0     4164 2023-06-03 12:49:45.045481 asynkit-0.9.0/src/asynkit/loop/default.py
+-rw-r--r--   0        0        0     4815 2023-06-03 12:49:45.045481 asynkit-0.9.0/src/asynkit/loop/eventloop.py
+-rw-r--r--   0        0        0     2981 2023-06-03 12:49:45.045481 asynkit-0.9.0/src/asynkit/loop/extensions.py
+-rw-r--r--   0        0        0     2922 2023-06-03 12:49:45.045481 asynkit-0.9.0/src/asynkit/loop/schedulingloop.py
+-rw-r--r--   0        0        0      281 2023-06-03 12:49:45.045481 asynkit-0.9.0/src/asynkit/loop/types.py
+-rw-r--r--   0        0        0    10720 2023-06-03 12:49:45.045481 asynkit-0.9.0/src/asynkit/monitor.py
+-rw-r--r--   0        0        0        0 2023-06-03 12:49:45.045481 asynkit-0.9.0/src/asynkit/py.typed
+-rw-r--r--   0        0        0     5352 2023-06-03 12:49:45.045481 asynkit-0.9.0/src/asynkit/scheduling.py
+-rw-r--r--   0        0        0     1209 2023-06-03 12:49:45.045481 asynkit-0.9.0/src/asynkit/tools.py
+-rw-r--r--   0        0        0    22246 1970-01-01 00:00:00.000000 asynkit-0.9.0/PKG-INFO
```

### Comparing `asynkit-0.8.0/LICENSE` & `asynkit-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `asynkit-0.8.0/README.md` & `asynkit-0.9.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 [![CI](https://github.com/kristjanvalur/py-asynkit/actions/workflows/ci.yml/badge.svg)](https://github.com/kristjanvalur/py-asynkit/actions/workflows/ci.yml)
 
 This module provides some handy tools for those wishing to have better control over the
 way Python's `asyncio` module does things.
 
 - Helper tools for controlling coroutine execution, such as `CoroStart` and `Monitor`
 - Utility classes such as `GeneratorObject`
-- Coroutine helpers such as `coro_iter()`
+- Coroutine helpers such as `coro_sync()`, `coro_iter()` and the `awaitmethod()` decorator
 - Scheduling helpers for `asyncio`, and extended event-loop implementations
 - _eager_ execution of Tasks
 - Limited support for `anyio` and `trio`.
 
 # Installation
 
 ```bash
@@ -29,14 +29,15 @@
 
 ```python
 @asynkit.eager
 async def get_slow_remote_data():
     result = await execute_remote_request()
     return result.important_data
 
+
 async def my_complex_thing():
     # kick off the request as soon as possible
     future = get_slow_remote_data()
     # The remote execution may now already be in flight. Do some work taking time
     intermediate_result = await some_local_computation()
     # wait for the result of the request
     return compute_result(intermediate_result, await future)
@@ -53,30 +54,34 @@
 
 This allows you to prepare and dispatch long running operations __as soon as possible__ while
 still being able to asynchronously wait for the result.
 
 `asynckit.eager` can also be used directly on the returned coroutine:
 ```python
 log = []
+
+
 async def test():
     log.append(1)
-    await asyncio.sleep(0.2) # some long IO
+    await asyncio.sleep(0.2)  # some long IO
     log.append(2)
 
+
 async def caller(convert):
     del log[:]
     log.append("a")
     future = convert(test())
     log.append("b")
-    await asyncio.sleep(0.1) # some other IO
+    await asyncio.sleep(0.1)  # some other IO
     log.append("c")
     await future
 
+
 # do nothing
-asyncio.run(caller(lambda c:c))
+asyncio.run(caller(lambda c: c))
 assert log == ["a", "b", "c", 1, 2]
 
 # Create a Task
 asyncio.run(caller(asyncio.create_task))
 assert log == ["a", "b", 1, "c", 2]
 
 # eager
@@ -100,82 +105,175 @@
 
 The result is an _awaitable_ which can be either directly awaited or passed
 to `asyncio.gather()`. The coroutine is executed in its own copy of the current context,
 just as would happen if it were directly turned into a `Task`.
 
 `func_eager()` is a decorator which automatically applies `coro_eager()` to the coroutine returned by an async function.
 
+## `coro_sync()` - Running coroutines synchronously
+
+If you are writing code which should work both synchronously and asynchronously,
+you can now write the code fully _async_ and then syn it _synchronously_ in the absence
+of an event loop.  Should the code cause any async features to be triggered, an exception is raised.  This helps avoid writing duplicate code.
+
+```python
+async def get_processed_data(datagetter):
+    data = datagetter()  # could be an async callback
+    data = await data if isawaitable(data) else data
+    return process_data(data)
+
+
+# will raise SynchronousError if it datagetter to be async
+def sync_get_processed_data(datagetter):
+    return asynkit.coro_sync(combine_stuff(cb1, cb2))
+```
+
+This sort of code might previously have been written thus:
+```python
+# may return an awaitable
+def get_processed_data(datagetter):
+    data = datagetter()
+    if isawaitable(data):
+        # return an awaitable helper function
+        async def helper():
+            data = await data
+            return process_data(data)
+
+        return helper
+    return process_data(data)  # duplication
+
+
+async def async_get_processed_data(datagetter):
+    r = get_processed_data(datagetter)
+    return await r if isawaitable(r) else r
+
+
+def sync_get_processed_data(datagetter):
+    r = get_processed_data(datagetter)
+    if isawaitable(r):
+        raise RuntimeError("callbacks failed to run synchronously")
+    return r
+```
+
+The above pattern, writing async methods as sync and returning async helpers,
+is common in library code which needs to work both in synchronous and asynchronous
+context.  Needless to say, it is very convoluted, hard to debug and contains a lot
+of code duplication where the same logic is repeated inside async helper methods.
+
+Using `coro_sync()` it is possible to write the entire logic as `async` methods and
+then selectively fail if the logic tries to invoke any truly async operations.
+
+`coro_sync()` can also be applied as a decorator:
+
+```python
+@asynkit.coro_sync
+async def sync_function():
+    return "look ma, no async!"
+
+
+assert sync_function().contains("look")
+```
+
+
 ## `CoroStart`
 
-This class manages the state of a partially run coroutine and is what what powers the `coro_eager()` function. 
+This class manages the state of a partially run coroutine and is what what powers the `coro_eager()` and `coro_sync()` functions. 
 When initialized, it will _start_ the coroutine, running it until it either suspends, returns, or raises
-an exception.
+an exception.  It can subsequently be _awaited_ to retreive the result.
 
 Similarly to a `Future`, it has these methods:
 
 - `done()` - returns `True` if the coroutine finished without blocking. In this case, the following two methods may be called to get the result.
 - `result()` - Returns the _return value_ of the coroutine or **raises** any _exception_ that it produced.
 - `exception()` - Returns any _exception_ raised, or `None` otherwise.
 
  But more importly it has these:
 
-- `as_coroutine()` - Returns an coroutine encapsulating the original coroutine's _continuation_.
-  If it has already finished, awaiting this coroutine is the same as calling `result()`, otherwise it continues the original coroutine's execution.
+- `__await__()` - A magic method making it directly _awaitable_. If it has already finished, awaiting this coroutine is the same as calling `result()`, otherwise it awaits the original coroutine's continued execution
+- `as_coroutine()` - A helper which returns a proper _coroutine_ object to await the `CoroStart`
 - `as_future()` - If `done()`, returns a `Future` holding its result, otherwise, a `RuntimeError`
-  is raised. This is suitable for using with
-  `asyncio.gather()` to avoid wrapping the result of an already completed coroutine into a `Task`.
-- `as_awaitable()` - If `done()`, returns `as_future()`, else returns `as_coroutine()`.
-  This is a convenience method for use with functions such as `asyncio.gather()`. 
+  is raised.
+- `as_awaitable()` - If `done()`, returns `as_future()`, else returns `self`.
+  This is a convenience method for use with functions such as `asyncio.gather()`, which would otherwise wrap a completed coroutine in a `Task`.
+
+In addition it has:
+
+- `aclose()` - If `not done()`, will throw a `GeneratorError` into the coroutine and wait for it to finish.  Otherwise does nothing.
+- `athrow(exc)` - If `not done()`, will throw the given error into the coroutine and wait for it to raise or return a value.
+- `close()` and `throw(exc)` - Synchronous versions of the above, will raise `RuntimeError` if the coroutine does not immediately exit.
+
+This means that a context manager such as `aclosing()` can be used to ensure
+that the coroutine is cleaned up in case of errors before it is awaited:
+
+```python
+# start foo() and run until it blocks
+async with aclosing(CoroStart(foo())) as coro:
+    ...  # do things, which may result in an error
+    return await coro
+```
 
 CoroStart can be provided with a `contextvars.Context` object, in which case the coroutine will be run using that
 context.
 
 ## Context helper
 
 `coro_await()` is a helper function to await a coroutine, optionally with a `contextvars.Context`
 object to activate:
 
 ```python
 var1 = contextvars.ContextVar("myvar")
 
+
 async def my_method():
     var1.set("foo")
-    
+
+
 async def main():
-    context=contextvars.copy_context()
+    context = contextvars.copy_context()
     var1.set("bar")
     await asynkit.coro_await(my_method(), context=context)
     # the coroutine didn't modify _our_ context
     assert var1.get() == "bar"
     # ... but it did modify the copied context
     assert context.get(var1) == "foo"
 ```
 
 This is similar to `contextvars.Context.run()` but works for async functions.  This function is
 implemented using `CoroStart`
 
-## `coro_iter` - helper for `__await__` methods
+## `awaitmethod` - decorator for `__await__` methods
 
-This helper function returns an `Generator` for a coroutine.  This is useful, if one
-wants to make an object _awaitable_ via the `__await__` method, which must only
-return `Iterator` objects.
+This decorator turns the decorated method into a `Generator` as required for
+`__await__` methods, which must only return `Iterator` objects.
+It does so by invoking the `coro_iter()` helper.
+
+This makes it simple to make a class _awaitable_ by decorating an `async`
+`__await__()` method.
 
 ```python
 class Awaitable:
     def __init__(self, cofunc):
         self.cofunc = cofunc
-    def __await__(self):
-        return asynkit.coro_iter(self.cofunc())
+        self.count = 0
+
+    @asynckit.awaitmethod
+    async def __await__(self):
+        await self.cofunc()
+        return self.count
+        self.count += 1
+
 
 async def main():
     async def sleeper():
         await asyncio.sleep(1)
+
     a = Awaitable(sleeper)
-    await a  # sleep once
-    await a  # sleep again
+    assert (await a) == 0  # sleep once
+    assert (await a) == 1  # sleep again
+
 
 asyncio.run(main())
 ```
 Unlike a regular _coroutine_ (the result of calling a _coroutine function_), an object with an `__await__` method can potentially be awaited multiple times.
 
 ## `Monitor`
 
@@ -186,14 +284,15 @@
 ```python
 async def coro(monitor):
     await monitor.oob("hello")
     await asyncio.sleep(0)
     await monitor.oob("dolly")
     return "done"
 
+
 async def runner():
     m = Monitor()
     c = coro(m)
     while True:
         try:
             print(await m.aawait(c))
         except OOBData as oob:
@@ -237,32 +336,33 @@
 condition, without resorting to the relatively heavy mechanism of creating, managing and synchronizing
 `Task` objects.  This can be useful if the coroutine needs to maintain state.
 
 Consider the following scenario. A _parser_ wants to read a line from a buffer, but fails, signalling
 this to the monitor:
 
 ```python
-    async def readline(m, buffer):
-        l = buffer.readline()
-        while not l.endswith("\n"):
-            await m.oob(None)  # ask for more data in the buffer
-            l += buffer.readline()
-        return l
-
-    async def manager(buffer, io):
-        m = Monitor()
-        a = m.awaitable(readline(m, buffer))
-        while True:
+async def readline(m, buffer):
+    l = buffer.readline()
+    while not l.endswith("\n"):
+        await m.oob(None)  # ask for more data in the buffer
+        l += buffer.readline()
+    return l
+
+
+async def manager(buffer, io):
+    m = Monitor()
+    a = m.awaitable(readline(m, buffer))
+    while True:
+        try:
+            return await a
+        except OOBData:
             try:
-                return await a
-            except OOBData:
-                try:
-                    buffer.fill(await io.read())
-                except Exception as exc:
-                    await m.athrow(c, exc)
+                buffer.fill(await io.read())
+            except Exception as exc:
+                await m.athrow(c, exc)
 ```
 
 In this example, `readline()` is trivial, but if it were a complicated parser with hierarchical
 invocation structure, then this pattern allows the decoupling of IO and the parsing of buffered data, maintaining the state of the parser while _the caller_ fills up the buffer.
 
 ## `GeneratorObject`
 
@@ -273,20 +373,22 @@
 by anyone, and not just by using `yield`, which makes composing such generators much simpler.
 
 The `GeneratorObject` leverages the `Monitor.oob()` method to deliver the _ayielded_ data to whomever is iterating over it:
 
 ```python
 async def generator(gen_obj):
     # yield directly to the generator
-    await gen_obj.ayield(1):
+    await gen_obj.ayield(1)
     # have someone else yield to it
     async def helper():
         await gen_obj.ayield(2)
+
     await asyncio.create_task(helper())
 
+
 async def runner():
     gen_obj = GeneratorObject()
     values = [val async for val in gen_obj(generator(gen_obj))]
     assert values == [1, 2]
 ```
 
 The `GeneratorObject`, when called, returns a `GeneratorObjectIterator` which behaves in
@@ -349,15 +451,17 @@
 
 ## Runnable task helpers
 
 A few functions are added to help working with tasks.
 
 The following identity applies:
 ```python
-asyncio.all_tasks() = asynkit.runnable_tasks() | asynkit.blocked_tasks() | asyncio.current_task()
+asyncio.all_tasks() = (
+    asynkit.runnable_tasks() | asynkit.blocked_tasks() | asyncio.current_task()
+)
 ```
 
 ### `runnable_tasks(loop=None)`
 
 Returns a set of the tasks that are currently runnable in the given loop
 
 ### `blocked_tasks(loop=None)`
@@ -432,27 +536,30 @@
 When using the asyncio backend, the module `asynkit.experimental.anyio` can be used, to provide "eager"-like
 behaviour to task creation.  It will return an `EagerTaskGroup` context manager:
 
 ```python
 from asynkit.experimental.anyio import create_eager_task_group
 from anyio import run, sleep
 
+
 async def func(task_status):
     print("hello")
-    task_status->started("world")
+    task_status.started("world")
     await sleep(0.01)
     print("goodbye")
 
+
 async def main():
 
     async with create_eager_task_group() as tg:
         start = tg.start(func)
         print("fine")
         print(await start)
-    print ("world")
+    print("world")
+
 
 run(main, backend="asyncio")
 ```
 
 This will result in the following output:
 
 ```
```

### Comparing `asynkit-0.8.0/pyproject.toml` & `asynkit-0.9.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "asynkit"
-version = "0.8.0"
+version = "0.9.0"
 description = "Async toolkit for advanced scheduling"
 authors = ["Kristján Valur Jónsson <sweskman@gmail.com>"]
 repository = "https://github.com/kristjanvalur/py-asynkit"
 readme = "README.md"
 keywords = ["asyncio", "eventloop"]
 license = "MIT"
 classifiers = [
@@ -15,28 +15,29 @@
 include=["src/asynkit/py.typed"]
 
 [tool.poe.tasks]
 lint = "ruff ."
 black = "black ."
 test = "pytest"
 cov = "pytest --cov=asynkit --cov-report term-missing --cov-branch"
-typing = "mypy -p asynkit"
+typing = "mypy -p asynkit -p tests"
 
 [tool.poetry.dependencies]
 python = "^3.7"
 typing-extensions = "^4.4.0"
 
 [tool.poetry.group.dev.dependencies]
 mypy = "^0.991"
 black = "^22.3.0"
 pytest = "^7.1.1"
 pytest-cov = "^3.0.0"
 poethepoet = "^0.13.1"
 ruff = "~0.0.190"
-anyio = {extras = ["trio"], version = "^3.6.2"}
+anyio = {extras = ["trio"], version = ">=3.6.0 <3.7.0"}  # typing introduced in 3.7
+blacken-docs = "^1.13.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
 #addopts = "-ra -q"
@@ -60,14 +61,20 @@
 [tool.mypy]
 
 [[tool.mypy.overrides]]
 module = "asynkit.*"
 strict = true
 
 [[tool.mypy.overrides]]
+module = "tests.*"
+check_untyped_defs = false
+allow_untyped_defs = true
+allow_untyped_calls = true
+
+[[tool.mypy.overrides]]
 module = [
     "asynkit.loop.eventloop",
     "asynkit.compat",
     "asynkit.tools",
 ]
 warn_unused_ignores=false
```

### Comparing `asynkit-0.8.0/src/asynkit/compat.py` & `asynkit-0.9.0/src/asynkit/compat.py`

 * *Files identical despite different names*

### Comparing `asynkit-0.8.0/src/asynkit/coroutine.py` & `asynkit-0.9.0/src/asynkit/coroutine.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,59 +1,79 @@
 import asyncio
 import functools
 import inspect
 import sys
 import types
 from contextvars import Context, copy_context
+from inspect import iscoroutinefunction
 from types import FrameType
 from typing import (
     Any,
     AsyncGenerator,
     Awaitable,
     Callable,
     Coroutine,
     Generator,
+    Iterator,
     Optional,
     Tuple,
+    Type,
     TypeVar,
     Union,
     cast,
     overload,
 )
 
 from typing_extensions import ParamSpec
 
 from .tools import create_task
 
 __all__ = [
     "CoroStart",
+    "awaitmethod",
     "coro_await",
     "coro_eager",
     "func_eager",
     "eager",
     "coro_get_frame",
     "coro_is_new",
     "coro_is_suspended",
     "coro_is_finished",
     "coro_iter",
+    "coro_sync",
+    "SynchronousError",
+    "CoroutineAbort",
 ]
 
 PYTHON_37 = sys.version_info.major == 3 and sys.version_info.minor == 7
 
 T = TypeVar("T")
+S = TypeVar("S")
 P = ParamSpec("P")
 T_co = TypeVar("T_co", covariant=True)
-CoroLike = Union[Coroutine[Any, Any, T], Generator[Any, Any, T]]
 Suspendable = Union[Coroutine, Generator, AsyncGenerator]
 
 """
 Tools and utilities for advanced management of coroutines
 """
 
 
+class SynchronousError(RuntimeError):
+    """
+    An exception thrown when a coroutine does not complete
+    synchronously.
+    """
+
+
+class CoroutineAbort(BaseException):
+    """
+    Exception thrown into coroutine to abort it.
+    """
+
+
 # Helpers to find if a coroutine (or a generator as created by types.coroutine)
 # has started or finished
 
 
 def _coro_getattr(coro: Suspendable, suffix: str) -> Any:
     """
     Get an attribute of a coroutine or coroutine like object
@@ -139,15 +159,15 @@
     `context`: A context object to run the coroutine in
     """
 
     __slots__ = ["coro", "context", "start_result"]
 
     def __init__(
         self,
-        coro: CoroLike[T_co],
+        coro: Coroutine[Any, Any, T_co],
         *,
         context: Optional[Context] = None,
     ):
         self.coro = coro
         self.context = context
         self.start_result: Optional[Tuple[Any, Optional[BaseException]]] = self._start()
 
@@ -209,17 +229,85 @@
                         self.context.run(self.coro.send, in_value)
                         if self.context
                         else self.coro.send(in_value)
                     )
                 except StopIteration as exc:
                     return cast(T_co, exc.value)
 
+    @overload
+    async def athrow(self, exc: Type[BaseException]) -> T_co:
+        ...
+
+    @overload
+    async def athrow(self, exc: BaseException) -> T_co:
+        ...
+
+    async def athrow(self, exc: Union[Type[BaseException], BaseException]) -> T_co:
+        """
+        Throw an exception into a started coroutine if it is not done, instead
+        of continuing it.
+        """
+        value = exc if isinstance(exc, BaseException) else exc()
+
+        try:
+            self.start_result = (
+                self.context.run(self.coro.throw, type(value), value)
+                if self.context
+                else self.coro.throw(type(value), value)
+            ), None
+        except BaseException as exception:
+            self.start_result = (None, exception)
+        return await self
+
+    @overload
+    def throw(self, exc: Type[BaseException]) -> T_co:
+        ...
+
+    @overload
+    def throw(self, exc: BaseException) -> T_co:
+        ...
+
+    def throw(
+        self, exc: Union[Type[BaseException], BaseException], tries: int = 1
+    ) -> T_co:
+        """
+        Throw an exception into the started coroutine. If the coroutine fails to
+        exit, the exception will be re-thrown, up to 'tries' times.  If the coroutine
+        handles the error and returns, the value is returned
+        """
+        value = exc if isinstance(exc, BaseException) else exc()
+        for i in range(tries):
+            try:
+                self.coro.throw(type(value), value)
+            except StopIteration as err:
+                return cast(T_co, err.value)
+        else:
+            raise RuntimeError(f"coroutine ignored {type(value).__name__}")
+
     def close(self) -> None:
-        self.coro.close()
+        """
+        Close the coroutine.  It must immediatly exit.
+        """
         self.start_result = None
+        self.coro.close()
+
+    async def aclose(self) -> None:
+        """
+        Close the coroutine, throwing a GeneratorExit() into it if it is not done.
+        It may perform async cleanup before exiting.
+        """
+        if self.start_result is None:
+            return
+        if self.done():
+            self.start_result = None
+            return
+        try:
+            await self.athrow(GeneratorExit())
+        except GeneratorExit:
+            pass
 
     def done(self) -> bool:
         """returns true if the coroutine finished without blocking"""
         return self.start_result is not None and self.start_result[1] is not None
 
     def result(self) -> T_co:
         """
@@ -241,15 +329,15 @@
             raise asyncio.InvalidStateError("CoroStart: coroutine not done()")
         if isinstance(exc, StopIteration):
             return None
         return exc
 
     async def as_coroutine(self) -> T_co:
         """
-        Continue execution of the coroutine that was started by start()
+        Continue execution of the coroutine that was started by start().
         Returns a coroutine which can be awaited
         """
         return await self
 
     def as_future(self) -> Awaitable[T_co]:
         """
         if `done()` convert the result of the coroutine into a `Future`
@@ -274,18 +362,20 @@
         is to be passed directly to methods such as `asyncio.gather()`.
         In such cases, we want to avoid a `done()` instance to cause
         a `Task` to be created just to retrieve the result.
         """
         if self.done():
             return self.as_future()
         else:
-            return self.as_coroutine()
+            return self
 
 
-async def coro_await(coro: CoroLike[T], *, context: Optional[Context] = None) -> T:
+async def coro_await(
+    coro: Coroutine[Any, Any, T], *, context: Optional[Context] = None
+) -> T:
     """
     A simple await, using the partial run primitives, equivalent to
     `async def coro_await(coro): return await coro`
     `context` can be provided for the coroutine to run in instead
     of the currently active context.
     """
     cs = CoroStart(coro, context=context)
@@ -392,7 +482,74 @@
             except StopIteration as exc:
                 return cast(T, exc.value)
         else:
             try:
                 out_value = coro.send(in_value)
             except StopIteration as exc:
                 return cast(T, exc.value)
+
+
+def awaitmethod(
+    func: Callable[[S], Coroutine[Any, Any, T]]
+) -> Callable[[S], Iterator[T]]:
+    """
+    Decorator to make a function return an awaitable.
+    The function must be a coroutine function.
+    Specifically intended to be used for __await__ methods.
+    """
+
+    @functools.wraps(func)
+    def wrapper(self: S) -> Iterator[T]:
+        return coro_iter(func(self))
+
+    return wrapper
+
+
+@overload
+def coro_sync(coro: Coroutine[Any, Any, T]) -> T:
+    ...
+
+
+@overload
+def coro_sync(coro: Callable[P, Coroutine[Any, Any, T]]) -> Callable[P, T]:
+    ...
+
+
+def coro_sync(
+    coro: Union[Coroutine[Any, Any, T], Callable[P, Coroutine[Any, Any, T]]]
+) -> Union[T, Callable[P, T]]:
+
+    """Runs a corouting synchronlously.  If the coroutine blocks, a
+    SynchronousError is raised.
+
+    Can also be used as a decorator for an async function.
+    """
+    if iscoroutinefunction(coro):
+        # we are a decorator
+        coro2 = cast(Callable[..., Coroutine[Any, Any, T]], coro)
+
+        @functools.wraps(coro)
+        def helper(*args: Any, **kwargs: Any) -> T:
+            return coro_sync(coro2(*args, **kwargs))
+
+        return helper
+    coro = cast(Coroutine[Any, Any, T], coro)
+    # We are running a coroutine synchronously
+    start = CoroStart[T](coro)
+    if start.done():
+        return start.result()
+    # kill the coroutine
+    try:
+        # we can't use GeneratorExit because that gets special handling and
+        # a traceback is not collected.
+        start.throw(CoroutineAbort())
+    except BaseException as err:
+        raise SynchronousError("coroutine failed to complete synchronously") from err
+    else:
+        raise SynchronousError(
+            "coroutine failed to complete synchronously (caught BaseException)"
+        )
+    finally:
+        try:
+            start.close()
+        except RuntimeError:
+            pass
```

### Comparing `asynkit-0.8.0/src/asynkit/experimental/anyio.py` & `asynkit-0.9.0/src/asynkit/experimental/anyio.py`

 * *Files identical despite different names*

### Comparing `asynkit-0.8.0/src/asynkit/loop/default.py` & `asynkit-0.9.0/src/asynkit/loop/default.py`

 * *Files identical despite different names*

### Comparing `asynkit-0.8.0/src/asynkit/loop/eventloop.py` & `asynkit-0.9.0/src/asynkit/loop/eventloop.py`

 * *Files identical despite different names*

### Comparing `asynkit-0.8.0/src/asynkit/loop/extensions.py` & `asynkit-0.9.0/src/asynkit/loop/extensions.py`

 * *Files identical despite different names*

### Comparing `asynkit-0.8.0/src/asynkit/loop/schedulingloop.py` & `asynkit-0.9.0/src/asynkit/loop/schedulingloop.py`

 * *Files identical despite different names*

### Comparing `asynkit-0.8.0/src/asynkit/monitor.py` & `asynkit-0.9.0/src/asynkit/monitor.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,22 @@
     Union,
     cast,
     overload,
 )
 
 from .coroutine import coro_is_finished, coro_is_new
 
+__all__ = [
+    "GeneratorObject",
+    "GeneratorObjectIterator",
+    "Monitor",
+    "MonitorAwaitable",
+    "OOBData",
+]
+
 T = TypeVar("T")
 V = TypeVar("V")
 T_co = TypeVar("T_co", covariant=True)
 T_contra = TypeVar("T_contra", contravariant=True)
 
 
 class OOBData(Exception):
```

### Comparing `asynkit-0.8.0/src/asynkit/scheduling.py` & `asynkit-0.9.0/src/asynkit/scheduling.py`

 * *Files identical despite different names*

### Comparing `asynkit-0.8.0/src/asynkit/tools.py` & `asynkit-0.9.0/src/asynkit/tools.py`

 * *Files identical despite different names*

### Comparing `asynkit-0.8.0/PKG-INFO` & `asynkit-0.9.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asynkit
-Version: 0.8.0
+Version: 0.9.0
 Summary: Async toolkit for advanced scheduling
 Home-page: https://github.com/kristjanvalur/py-asynkit
 License: MIT
 Keywords: asyncio,eventloop
 Author: Kristján Valur Jónsson
 Author-email: sweskman@gmail.com
 Requires-Python: >=3.7,<4.0
@@ -27,15 +27,15 @@
 [![CI](https://github.com/kristjanvalur/py-asynkit/actions/workflows/ci.yml/badge.svg)](https://github.com/kristjanvalur/py-asynkit/actions/workflows/ci.yml)
 
 This module provides some handy tools for those wishing to have better control over the
 way Python's `asyncio` module does things.
 
 - Helper tools for controlling coroutine execution, such as `CoroStart` and `Monitor`
 - Utility classes such as `GeneratorObject`
-- Coroutine helpers such as `coro_iter()`
+- Coroutine helpers such as `coro_sync()`, `coro_iter()` and the `awaitmethod()` decorator
 - Scheduling helpers for `asyncio`, and extended event-loop implementations
 - _eager_ execution of Tasks
 - Limited support for `anyio` and `trio`.
 
 # Installation
 
 ```bash
@@ -53,14 +53,15 @@
 
 ```python
 @asynkit.eager
 async def get_slow_remote_data():
     result = await execute_remote_request()
     return result.important_data
 
+
 async def my_complex_thing():
     # kick off the request as soon as possible
     future = get_slow_remote_data()
     # The remote execution may now already be in flight. Do some work taking time
     intermediate_result = await some_local_computation()
     # wait for the result of the request
     return compute_result(intermediate_result, await future)
@@ -77,30 +78,34 @@
 
 This allows you to prepare and dispatch long running operations __as soon as possible__ while
 still being able to asynchronously wait for the result.
 
 `asynckit.eager` can also be used directly on the returned coroutine:
 ```python
 log = []
+
+
 async def test():
     log.append(1)
-    await asyncio.sleep(0.2) # some long IO
+    await asyncio.sleep(0.2)  # some long IO
     log.append(2)
 
+
 async def caller(convert):
     del log[:]
     log.append("a")
     future = convert(test())
     log.append("b")
-    await asyncio.sleep(0.1) # some other IO
+    await asyncio.sleep(0.1)  # some other IO
     log.append("c")
     await future
 
+
 # do nothing
-asyncio.run(caller(lambda c:c))
+asyncio.run(caller(lambda c: c))
 assert log == ["a", "b", "c", 1, 2]
 
 # Create a Task
 asyncio.run(caller(asyncio.create_task))
 assert log == ["a", "b", 1, "c", 2]
 
 # eager
@@ -124,82 +129,175 @@
 
 The result is an _awaitable_ which can be either directly awaited or passed
 to `asyncio.gather()`. The coroutine is executed in its own copy of the current context,
 just as would happen if it were directly turned into a `Task`.
 
 `func_eager()` is a decorator which automatically applies `coro_eager()` to the coroutine returned by an async function.
 
+## `coro_sync()` - Running coroutines synchronously
+
+If you are writing code which should work both synchronously and asynchronously,
+you can now write the code fully _async_ and then syn it _synchronously_ in the absence
+of an event loop.  Should the code cause any async features to be triggered, an exception is raised.  This helps avoid writing duplicate code.
+
+```python
+async def get_processed_data(datagetter):
+    data = datagetter()  # could be an async callback
+    data = await data if isawaitable(data) else data
+    return process_data(data)
+
+
+# will raise SynchronousError if it datagetter to be async
+def sync_get_processed_data(datagetter):
+    return asynkit.coro_sync(combine_stuff(cb1, cb2))
+```
+
+This sort of code might previously have been written thus:
+```python
+# may return an awaitable
+def get_processed_data(datagetter):
+    data = datagetter()
+    if isawaitable(data):
+        # return an awaitable helper function
+        async def helper():
+            data = await data
+            return process_data(data)
+
+        return helper
+    return process_data(data)  # duplication
+
+
+async def async_get_processed_data(datagetter):
+    r = get_processed_data(datagetter)
+    return await r if isawaitable(r) else r
+
+
+def sync_get_processed_data(datagetter):
+    r = get_processed_data(datagetter)
+    if isawaitable(r):
+        raise RuntimeError("callbacks failed to run synchronously")
+    return r
+```
+
+The above pattern, writing async methods as sync and returning async helpers,
+is common in library code which needs to work both in synchronous and asynchronous
+context.  Needless to say, it is very convoluted, hard to debug and contains a lot
+of code duplication where the same logic is repeated inside async helper methods.
+
+Using `coro_sync()` it is possible to write the entire logic as `async` methods and
+then selectively fail if the logic tries to invoke any truly async operations.
+
+`coro_sync()` can also be applied as a decorator:
+
+```python
+@asynkit.coro_sync
+async def sync_function():
+    return "look ma, no async!"
+
+
+assert sync_function().contains("look")
+```
+
+
 ## `CoroStart`
 
-This class manages the state of a partially run coroutine and is what what powers the `coro_eager()` function. 
+This class manages the state of a partially run coroutine and is what what powers the `coro_eager()` and `coro_sync()` functions. 
 When initialized, it will _start_ the coroutine, running it until it either suspends, returns, or raises
-an exception.
+an exception.  It can subsequently be _awaited_ to retreive the result.
 
 Similarly to a `Future`, it has these methods:
 
 - `done()` - returns `True` if the coroutine finished without blocking. In this case, the following two methods may be called to get the result.
 - `result()` - Returns the _return value_ of the coroutine or **raises** any _exception_ that it produced.
 - `exception()` - Returns any _exception_ raised, or `None` otherwise.
 
  But more importly it has these:
 
-- `as_coroutine()` - Returns an coroutine encapsulating the original coroutine's _continuation_.
-  If it has already finished, awaiting this coroutine is the same as calling `result()`, otherwise it continues the original coroutine's execution.
+- `__await__()` - A magic method making it directly _awaitable_. If it has already finished, awaiting this coroutine is the same as calling `result()`, otherwise it awaits the original coroutine's continued execution
+- `as_coroutine()` - A helper which returns a proper _coroutine_ object to await the `CoroStart`
 - `as_future()` - If `done()`, returns a `Future` holding its result, otherwise, a `RuntimeError`
-  is raised. This is suitable for using with
-  `asyncio.gather()` to avoid wrapping the result of an already completed coroutine into a `Task`.
-- `as_awaitable()` - If `done()`, returns `as_future()`, else returns `as_coroutine()`.
-  This is a convenience method for use with functions such as `asyncio.gather()`. 
+  is raised.
+- `as_awaitable()` - If `done()`, returns `as_future()`, else returns `self`.
+  This is a convenience method for use with functions such as `asyncio.gather()`, which would otherwise wrap a completed coroutine in a `Task`.
+
+In addition it has:
+
+- `aclose()` - If `not done()`, will throw a `GeneratorError` into the coroutine and wait for it to finish.  Otherwise does nothing.
+- `athrow(exc)` - If `not done()`, will throw the given error into the coroutine and wait for it to raise or return a value.
+- `close()` and `throw(exc)` - Synchronous versions of the above, will raise `RuntimeError` if the coroutine does not immediately exit.
+
+This means that a context manager such as `aclosing()` can be used to ensure
+that the coroutine is cleaned up in case of errors before it is awaited:
+
+```python
+# start foo() and run until it blocks
+async with aclosing(CoroStart(foo())) as coro:
+    ...  # do things, which may result in an error
+    return await coro
+```
 
 CoroStart can be provided with a `contextvars.Context` object, in which case the coroutine will be run using that
 context.
 
 ## Context helper
 
 `coro_await()` is a helper function to await a coroutine, optionally with a `contextvars.Context`
 object to activate:
 
 ```python
 var1 = contextvars.ContextVar("myvar")
 
+
 async def my_method():
     var1.set("foo")
-    
+
+
 async def main():
-    context=contextvars.copy_context()
+    context = contextvars.copy_context()
     var1.set("bar")
     await asynkit.coro_await(my_method(), context=context)
     # the coroutine didn't modify _our_ context
     assert var1.get() == "bar"
     # ... but it did modify the copied context
     assert context.get(var1) == "foo"
 ```
 
 This is similar to `contextvars.Context.run()` but works for async functions.  This function is
 implemented using `CoroStart`
 
-## `coro_iter` - helper for `__await__` methods
+## `awaitmethod` - decorator for `__await__` methods
 
-This helper function returns an `Generator` for a coroutine.  This is useful, if one
-wants to make an object _awaitable_ via the `__await__` method, which must only
-return `Iterator` objects.
+This decorator turns the decorated method into a `Generator` as required for
+`__await__` methods, which must only return `Iterator` objects.
+It does so by invoking the `coro_iter()` helper.
+
+This makes it simple to make a class _awaitable_ by decorating an `async`
+`__await__()` method.
 
 ```python
 class Awaitable:
     def __init__(self, cofunc):
         self.cofunc = cofunc
-    def __await__(self):
-        return asynkit.coro_iter(self.cofunc())
+        self.count = 0
+
+    @asynckit.awaitmethod
+    async def __await__(self):
+        await self.cofunc()
+        return self.count
+        self.count += 1
+
 
 async def main():
     async def sleeper():
         await asyncio.sleep(1)
+
     a = Awaitable(sleeper)
-    await a  # sleep once
-    await a  # sleep again
+    assert (await a) == 0  # sleep once
+    assert (await a) == 1  # sleep again
+
 
 asyncio.run(main())
 ```
 Unlike a regular _coroutine_ (the result of calling a _coroutine function_), an object with an `__await__` method can potentially be awaited multiple times.
 
 ## `Monitor`
 
@@ -210,14 +308,15 @@
 ```python
 async def coro(monitor):
     await monitor.oob("hello")
     await asyncio.sleep(0)
     await monitor.oob("dolly")
     return "done"
 
+
 async def runner():
     m = Monitor()
     c = coro(m)
     while True:
         try:
             print(await m.aawait(c))
         except OOBData as oob:
@@ -261,32 +360,33 @@
 condition, without resorting to the relatively heavy mechanism of creating, managing and synchronizing
 `Task` objects.  This can be useful if the coroutine needs to maintain state.
 
 Consider the following scenario. A _parser_ wants to read a line from a buffer, but fails, signalling
 this to the monitor:
 
 ```python
-    async def readline(m, buffer):
-        l = buffer.readline()
-        while not l.endswith("\n"):
-            await m.oob(None)  # ask for more data in the buffer
-            l += buffer.readline()
-        return l
-
-    async def manager(buffer, io):
-        m = Monitor()
-        a = m.awaitable(readline(m, buffer))
-        while True:
+async def readline(m, buffer):
+    l = buffer.readline()
+    while not l.endswith("\n"):
+        await m.oob(None)  # ask for more data in the buffer
+        l += buffer.readline()
+    return l
+
+
+async def manager(buffer, io):
+    m = Monitor()
+    a = m.awaitable(readline(m, buffer))
+    while True:
+        try:
+            return await a
+        except OOBData:
             try:
-                return await a
-            except OOBData:
-                try:
-                    buffer.fill(await io.read())
-                except Exception as exc:
-                    await m.athrow(c, exc)
+                buffer.fill(await io.read())
+            except Exception as exc:
+                await m.athrow(c, exc)
 ```
 
 In this example, `readline()` is trivial, but if it were a complicated parser with hierarchical
 invocation structure, then this pattern allows the decoupling of IO and the parsing of buffered data, maintaining the state of the parser while _the caller_ fills up the buffer.
 
 ## `GeneratorObject`
 
@@ -297,20 +397,22 @@
 by anyone, and not just by using `yield`, which makes composing such generators much simpler.
 
 The `GeneratorObject` leverages the `Monitor.oob()` method to deliver the _ayielded_ data to whomever is iterating over it:
 
 ```python
 async def generator(gen_obj):
     # yield directly to the generator
-    await gen_obj.ayield(1):
+    await gen_obj.ayield(1)
     # have someone else yield to it
     async def helper():
         await gen_obj.ayield(2)
+
     await asyncio.create_task(helper())
 
+
 async def runner():
     gen_obj = GeneratorObject()
     values = [val async for val in gen_obj(generator(gen_obj))]
     assert values == [1, 2]
 ```
 
 The `GeneratorObject`, when called, returns a `GeneratorObjectIterator` which behaves in
@@ -373,15 +475,17 @@
 
 ## Runnable task helpers
 
 A few functions are added to help working with tasks.
 
 The following identity applies:
 ```python
-asyncio.all_tasks() = asynkit.runnable_tasks() | asynkit.blocked_tasks() | asyncio.current_task()
+asyncio.all_tasks() = (
+    asynkit.runnable_tasks() | asynkit.blocked_tasks() | asyncio.current_task()
+)
 ```
 
 ### `runnable_tasks(loop=None)`
 
 Returns a set of the tasks that are currently runnable in the given loop
 
 ### `blocked_tasks(loop=None)`
@@ -456,27 +560,30 @@
 When using the asyncio backend, the module `asynkit.experimental.anyio` can be used, to provide "eager"-like
 behaviour to task creation.  It will return an `EagerTaskGroup` context manager:
 
 ```python
 from asynkit.experimental.anyio import create_eager_task_group
 from anyio import run, sleep
 
+
 async def func(task_status):
     print("hello")
-    task_status->started("world")
+    task_status.started("world")
     await sleep(0.01)
     print("goodbye")
 
+
 async def main():
 
     async with create_eager_task_group() as tg:
         start = tg.start(func)
         print("fine")
         print(await start)
-    print ("world")
+    print("world")
+
 
 run(main, backend="asyncio")
 ```
 
 This will result in the following output:
 
 ```
```

