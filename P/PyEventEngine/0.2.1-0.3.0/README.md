# Comparing `tmp/PyEventEngine-0.2.1.tar.gz` & `tmp/pyeventengine-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyEventEngine-0.2.1.tar", last modified: Wed Jun  7 19:56:04 2023, max compression
+gzip compressed data, was "pyeventengine-0.3.0.tar", last modified: Tue May 28 10:27:56 2024, max compression
```

## Comparing `PyEventEngine-0.2.1.tar` & `pyeventengine-0.3.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0 bolun     (1000) bolun     (1000)        0 2023-06-07 19:56:04.152082 PyEventEngine-0.2.1/
-drwxrwxrwx   0 bolun     (1000) bolun     (1000)        0 2023-06-07 19:56:03.840799 PyEventEngine-0.2.1/EventEngine/
-drwxrwxrwx   0 bolun     (1000) bolun     (1000)        0 2023-06-07 19:56:03.967363 PyEventEngine-0.2.1/EventEngine/Core/
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)    11736 2023-05-29 07:51:43.000000 PyEventEngine-0.2.1/EventEngine/Core/_Event.py
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)     3488 2023-05-29 09:31:15.000000 PyEventEngine-0.2.1/EventEngine/Core/_Topic.py
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)     5821 2023-06-07 19:47:58.000000 PyEventEngine-0.2.1/EventEngine/Core/_Topic_c.py
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)     3128 2023-06-07 19:32:17.000000 PyEventEngine-0.2.1/EventEngine/Core/__init__.py
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)       43 2023-06-07 18:11:39.000000 PyEventEngine-0.2.1/EventEngine/__init__.py
-drwxrwxrwx   0 bolun     (1000) bolun     (1000)        0 2023-06-07 19:56:03.999337 PyEventEngine-0.2.1/EventEngine/cpp/
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)     9038 2023-06-07 19:15:36.000000 PyEventEngine-0.2.1/EventEngine/cpp/topic_api.cpp
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)     1066 2023-05-27 08:57:55.000000 PyEventEngine-0.2.1/LICENSE
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)     2001 2023-06-07 19:56:04.154077 PyEventEngine-0.2.1/PKG-INFO
-drwxrwxrwx   0 bolun     (1000) bolun     (1000)        0 2023-06-07 19:56:04.115557 PyEventEngine-0.2.1/PyEventEngine.egg-info/
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)     2001 2023-06-07 19:56:03.000000 PyEventEngine-0.2.1/PyEventEngine.egg-info/PKG-INFO
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)      350 2023-06-07 19:56:03.000000 PyEventEngine-0.2.1/PyEventEngine.egg-info/SOURCES.txt
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)        1 2023-06-07 19:56:03.000000 PyEventEngine-0.2.1/PyEventEngine.egg-info/dependency_links.txt
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)       12 2023-06-07 19:56:03.000000 PyEventEngine-0.2.1/PyEventEngine.egg-info/top_level.txt
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)     1507 2023-05-27 08:57:55.000000 PyEventEngine-0.2.1/README.md
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)       79 2023-06-07 19:56:04.163074 PyEventEngine-0.2.1/setup.cfg
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)     1633 2023-06-07 19:02:25.000000 PyEventEngine-0.2.1/setup.py
+drwxrwxrwx   0 bolun     (1000) bolun     (1000)        0 2024-05-28 10:27:56.222565 pyeventengine-0.3.0/
+drwxrwxrwx   0 bolun     (1000) bolun     (1000)        0 2024-05-28 10:27:56.121041 pyeventengine-0.3.0/EventEngine/
+drwxrwxrwx   0 bolun     (1000) bolun     (1000)        0 2024-05-28 10:27:56.154549 pyeventengine-0.3.0/EventEngine/Core/
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)     3227 2024-05-28 10:24:33.000000 pyeventengine-0.3.0/EventEngine/Core/__init__.py
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)    13778 2024-05-28 10:17:54.000000 pyeventengine-0.3.0/EventEngine/Core/_event.py
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)     4525 2024-05-28 10:21:19.000000 pyeventengine-0.3.0/EventEngine/Core/_topic.py
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)     3001 2024-05-28 06:54:14.000000 pyeventengine-0.3.0/EventEngine/Core/_topic_c.py
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)       43 2024-05-28 10:24:33.000000 pyeventengine-0.3.0/EventEngine/__init__.py
+drwxrwxrwx   0 bolun     (1000) bolun     (1000)        0 2024-05-28 10:27:56.163058 pyeventengine-0.3.0/EventEngine/cpp/
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)     9271 2024-05-28 06:20:25.000000 pyeventengine-0.3.0/EventEngine/cpp/topic_api.cpp
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)     1066 2024-05-28 06:20:25.000000 pyeventengine-0.3.0/LICENSE
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)     2103 2024-05-28 10:27:56.220564 pyeventengine-0.3.0/PKG-INFO
+drwxrwxrwx   0 bolun     (1000) bolun     (1000)        0 2024-05-28 10:27:56.217565 pyeventengine-0.3.0/PyEventEngine.egg-info/
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)     2103 2024-05-28 10:27:56.000000 pyeventengine-0.3.0/PyEventEngine.egg-info/PKG-INFO
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)      350 2024-05-28 10:27:56.000000 pyeventengine-0.3.0/PyEventEngine.egg-info/SOURCES.txt
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)        1 2024-05-28 10:27:56.000000 pyeventengine-0.3.0/PyEventEngine.egg-info/dependency_links.txt
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)       12 2024-05-28 10:27:56.000000 pyeventengine-0.3.0/PyEventEngine.egg-info/top_level.txt
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)     1507 2024-05-28 06:20:25.000000 pyeventengine-0.3.0/README.md
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)       79 2024-05-28 10:27:56.224565 pyeventengine-0.3.0/setup.cfg
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)     1733 2024-05-28 10:24:33.000000 pyeventengine-0.3.0/setup.py
```

### Comparing `PyEventEngine-0.2.1/EventEngine/Core/_Event.py` & `pyeventengine-0.3.0/EventEngine/Core/_event.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,161 +1,205 @@
-from __future__ import annotations
-
 import datetime
-import queue
-import threading
+import enum
+import inspect
 import time
 import traceback
-from typing import Iterable
+from collections import deque
+from logging import Logger
+from threading import Thread, Semaphore
+from typing import Iterable, TypedDict, NotRequired, Callable
+
+from . import LOGGER, LOG_LEVEL_EVENT, Topic, DEBUG
+
+LOGGER = LOGGER.getChild('Event')
+
 
-from . import LOGGER, LOG_LEVEL_EVENT, Topic
+class EventDict(TypedDict):
+    topic: str
+    args: NotRequired[tuple]
+    kwargs: NotRequired[dict]
 
 
 class EventHookBase(object):
     """
     Event object with
     a string topic for event engine to distribute event,
     and a list of handler to process data
     """
 
-    def __init__(self, topic: Topic, handler: list[callable] | callable | None = None):
+    def __init__(self, topic: Topic, logger: Logger = None, max_size: int = None):
         self.topic = topic
-
-        if callable(handler):
-            self.handlers = [handler]
-        elif isinstance(handler, Iterable):
-            self.handlers = []
-            for hdl in handler:
-                if callable(hdl):
-                    self.handlers.append(hdl)
-                else:
-                    raise ValueError(f'invalid handler {hdl}')
-        elif handler is None:
-            self.handlers = []
-        else:
-            raise ValueError(f'Invalid handler {handler}')
+        self.logger = LOGGER.getChild(f'EventHook.{topic}') if logger is None else logger
+        self.handlers: deque[Callable] = deque(maxlen=max_size)
 
     def __call__(self, *args, **kwargs):
         self.trigger(topic=self.topic, args=args, kwargs=kwargs)
 
-    def __iadd__(self, handler):
+    def __iadd__(self, handler: Callable):
         self.add_handler(handler)
         return self
 
-    def __isub__(self, handler):
+    def __isub__(self, handler: Callable):
         self.remove_handler(handler)
         return self
 
     def trigger(self, topic: Topic, args: tuple = None, kwargs: dict = None):
         if args is None:
             args = ()
 
         if kwargs is None:
             kwargs = {}
 
         for handler in self.handlers:
             try:
                 try:
                     handler(topic=topic, *args, **kwargs)
-                except TypeError:
-                    handler(*args, **kwargs)
+                except TypeError as e:
+                    if e.__str__().endswith("unexpected keyword argument 'topic'"):
+                        handler(*args, **kwargs)
+                    else:
+                        raise e
             except Exception as _:
-                LOGGER.error(traceback.format_exc())
+                self.logger.error(traceback.format_exc())
 
-    def add_handler(self, handler: callable):
+    def add_handler(self, handler: Callable):
+        if handler in self.handlers:
+            LOGGER.warning(f'Handler {handler} already in {self}. This action might cause it to trigger twice.')
         self.handlers.append(handler)
 
-    def remove_handler(self, handler: callable):
-        self.handlers.remove(handler)
+    def remove_handler(self, handler: Callable):
+        try:
+            self.handlers.remove(handler)
+        except ValueError as e:
+            self.logger.error(f'Handler {handler} not found in {self}.')
 
 
 class EventHook(EventHookBase):
-    def __init__(self, topic, handler):
-        self.logger = LOGGER.getChild(f'EventHook.{topic}')
-        super().__init__(topic=topic, handler=handler)
+    def __init__(self, topic: Topic, logger: Logger = None, max_size: int = None, handler: list[Callable] | Callable | None = None):
+        super().__init__(topic=topic, logger=logger, max_size=max_size)
+        self.with_topic: deque[bool] = deque()
+
+        if handler is None:
+            pass
+        elif callable(handler):
+            self.add_handler(handler)
+        elif isinstance(handler, Iterable):
+            for _handler in handler:
+                self.add_handler(handler=_handler)
+        else:
+            raise ValueError(f'Invalid handler {handler}, expect a Callable or a list of Callable.')
 
     def trigger(self, topic: Topic, args: tuple = None, kwargs: dict = None):
         ts = time.time()
-
         if args is None:
             args = ()
 
         if kwargs is None:
             kwargs = {}
 
-        for handler in self.handlers:
+        for handler, with_topic in zip(self.handlers, self.with_topic):
             try:
-                try:
+                if with_topic:
                     handler(topic=topic, *args, **kwargs)
-                except TypeError:
+                else:
                     handler(*args, **kwargs)
             except Exception as _:
                 self.logger.error(traceback.format_exc())
 
-        self.logger.log(LOG_LEVEL_EVENT, f'EventHook {self.topic} tasks triggered {len(self.handlers):,} handlers, complete in {(time.time() - ts) * 1000:.3f}ms')
+        if DEBUG:
+            self.logger.log(LOG_LEVEL_EVENT, f'EventHook {self.topic} tasks triggered {len(self.handlers):,} handlers, complete in {(time.time() - ts) * 1000:.3f}ms.')
+
+    def add_handler(self, handler: Callable, with_topic: bool = None):
+        sig = inspect.signature(handler)
+
+        if with_topic is None:
+            for param in sig.parameters.values():
+                if param.name == 'topic' or param.kind == param.VAR_KEYWORD:
+                    with_topic = True
+                    break
+
+        super().add_handler(handler=handler)
+        self.with_topic.append(with_topic)
+
+    def remove_handler(self, handler: Callable):
+        try:
+            idx = self.handlers.index(handler)
+            self.handlers.__delitem__(idx)
+            self.with_topic.__delitem__(idx)
+        except ValueError as e:
+            pass
 
 
 class EventEngineBase(object):
     EventHook = EventHook
 
-    def __init__(self, max_size=0):
-        self.lock = threading.Lock()
-
-        self._max_size = max_size
-        self._queue: queue.Queue = queue.Queue(maxsize=self._max_size)
+    def __init__(self, logger: Logger = None, buffer_size: int = 0):
+        self.logger = LOGGER.getChild(f'EventEngine') if logger is None else logger
+        self._buffer_size = buffer_size
+        self._put_lock = Semaphore(self._buffer_size)
+        self._get_lock = Semaphore(0)
+        self._deque: deque[EventDict] = deque(maxlen=buffer_size if buffer_size else None)
         self._active: bool = False
-        self._engine: threading.Thread = threading.Thread(target=self._run, name='EventEngine')
+        self._engine: Thread = Thread(target=self._run, name='EventEngine')
         self._event_hooks: dict[Topic, EventHook] = {}
 
+        if buffer_size and buffer_size < 8:
+            self.logger.info(f'buffer_size={buffer_size} too small. This might cause a dead lock.')
+
     def _run(self) -> None:
         """
         Get event from queue and then process it.
         """
         while self._active:
+            self._get_lock.acquire(blocking=True, timeout=None)
+
             try:
-                event_dict = self._queue.get(block=True, timeout=1)
-                topic = event_dict['topic']
-                args = event_dict.get('args', ())
-                kwargs = event_dict.get('kwargs', {})
-                self._process(topic, *args, **kwargs)
-            except queue.Empty:
-                pass
+                event_dict = self._deque.pop()
+            except IndexError as e:
+                if not self._active:
+                    return
+                raise e
+
+            topic = event_dict['topic']
+            args = event_dict.get('args', ())
+            kwargs = event_dict.get('kwargs', {})
+            self._process(topic=topic, *args, **kwargs)
+
+            if self._buffer_size:
+                self._put_lock.release()
 
     def _process(self, topic: str, *args, **kwargs) -> None:
         """
         distribute data to registered event hook in the order of registration
         """
-        for _ in list(self._event_hooks):
-            m = _.match(topic=topic)
-            if m:
-                event_hook = self._event_hooks.get(_)
-
-                if event_hook is not None:
-                    event_hook.trigger(topic=m, args=args, kwargs=kwargs)
+        for event_topic, event_hook in self._event_hooks.items():
+            if matched_topic := event_topic.match(topic=topic):
+                event_hook.trigger(topic=matched_topic, args=args, kwargs=kwargs)
 
     def start(self) -> None:
         """
         Start event engine to process events and generate timer events.
         """
         if self._active:
-            LOGGER.warning('EventEngine already started!')
+            self.logger.warning(f'{self} already started!')
             return
 
         self._active = True
         self._engine.start()
 
     def stop(self) -> None:
         """
         Stop event engine.
         """
         if not self._active:
-            LOGGER.warning('EventEngine already stopped!')
+            self.logger.warning('EventEngine already stopped!')
             return
 
         self._active = False
+        self._get_lock.release()
         self._engine.join()
 
     def put(self, topic: str | Topic, block: bool = True, timeout: float = None, *args, **kwargs):
         """
         fast way to put an event, kwargs MUST NOT contain "topic", "block" and "timeout" keywords
         :param topic: the topic to put into engine
         :param block: block if necessary until a free slot is available
@@ -177,23 +221,28 @@
         :return: nothing
         """
         if isinstance(topic, Topic):
             topic = topic.value
         elif not isinstance(topic, str):
             raise ValueError(f'Invalid topic {topic}')
 
+        if self._buffer_size:
+            self._put_lock.acquire()
+
         event_dict = {'topic': topic}
 
         if args is not None:
             event_dict['args'] = args
 
         if kwargs is not None:
             event_dict['kwargs'] = kwargs
 
-        self._queue.put(event_dict, block=block, timeout=timeout)
+        self._deque.append(event_dict)
+
+        self._get_lock.release()
 
     def register_hook(self, hook: EventHook) -> None:
         """
         register a hook event
         """
         if hook.topic in self._event_hooks:
             for handler in hook.handlers:
@@ -204,52 +253,47 @@
     def unregister_hook(self, topic: Topic) -> None:
         """
         Unregister an existing hook
         """
         if topic in self._event_hooks:
             self._event_hooks.pop(topic)
 
-    def register_handler(self, topic: Topic, handler: Iterable[callable] | callable) -> None:
+    def register_handler(self, topic: Topic, handler: Iterable[Callable] | Callable) -> None:
         """
         Register one or more handler for a specific topic
         """
 
         if not isinstance(topic, Topic):
             raise TypeError(f'Invalid topic {topic}')
 
         if topic not in self._event_hooks:
-            self._event_hooks[topic] = self.EventHook(topic=topic, handler=handler)
+            self._event_hooks[topic] = self.EventHook(topic=topic, handler=handler, logger=self.logger.getChild(topic.value))
         else:
             self._event_hooks[topic].add_handler(handler)
 
-    def unregister_handler(self, topic: Topic, handler: callable) -> None:
+    def unregister_handler(self, topic: Topic, handler: Callable) -> None:
         """
         Unregister an existing handler function.
         """
         if topic in self._event_hooks:
             self._event_hooks[topic].remove_handler(handler=handler)
 
     @property
-    def max_size(self):
-        return self._max_size
-
-    @max_size.setter
-    def max_size(self, size: int):
-        self._max_size = size
-        self._queue.maxsize = size
+    def buffer_size(self):
+        return self._buffer_size
 
 
 class EventEngine(EventEngineBase):
     EventHook = EventHook
 
-    def __init__(self, max_size=0):
-        super().__init__(max_size=max_size)
-        self.timer: dict[float | str, threading.Thread] = {}
+    def __init__(self, buffer_size=0):
+        super().__init__(buffer_size=buffer_size)
+        self.timer: dict[float | str, Thread] = {}
 
-    def register_handler(self, topic, handler):
+    def register_handler(self, topic: Topic | str | enum.Enum, handler: Callable):
         topic = Topic.cast(topic)
         super().register_handler(topic=topic, handler=handler)
 
     def publish(self, topic, block: bool = True, timeout: float = None, args=None, kwargs=None):
         topic = Topic.cast(topic)
         super().publish(topic=topic, block=block, timeout=timeout, args=args, kwargs=kwargs)
 
@@ -273,28 +317,28 @@
         :return: the topic of timer event hook
         """
         if isinstance(interval, datetime.timedelta):
             interval = interval.total_seconds()
 
         if interval == 1:
             topic = Topic('EventEngine.Internal.Timer.Second')
-            timer = threading.Thread(target=self._second_timer, kwargs={'topic': topic})
+            timer = Thread(target=self._second_timer, kwargs={'topic': topic})
         elif interval == 60:
             topic = Topic('EventEngine.Internal.Timer.Minute')
-            timer = threading.Thread(target=self._minute_timer, kwargs={'topic': topic})
+            timer = Thread(target=self._minute_timer, kwargs={'topic': topic})
         else:
             topic = Topic(f'EventEngine.Internal.Timer.{interval}')
-            timer = threading.Thread(target=self._run_timer, kwargs={'interval': interval, 'topic': topic, 'activate_time': activate_time})
+            timer = Thread(target=self._run_timer, kwargs={'interval': interval, 'topic': topic, 'activate_time': activate_time})
 
         if interval not in self.timer:
             self.timer[interval] = timer
             timer.start()
         else:
             if activate_time is not None:
-                LOGGER.debug(f'Timer thread with interval [{datetime.timedelta(seconds=interval)}] already initialized! Argument [activate_time] takes no effect!')
+                self.logger.debug(f'Timer thread with interval [{datetime.timedelta(seconds=interval)}] already initialized! Argument [activate_time] takes no effect!')
 
         return topic
 
     def _run_timer(self, interval: datetime.timedelta | float | int, topic: Topic, activate_time: datetime.datetime = None) -> None:
         if isinstance(interval, datetime.timedelta):
             interval = interval.total_seconds()
```

### Comparing `PyEventEngine-0.2.1/EventEngine/Core/_Topic.py` & `pyeventengine-0.3.0/EventEngine/Core/_topic.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,11 @@
-from __future__ import annotations
-
 import re
 from enum import Enum
 from string import Formatter
+from typing import Self, Type
 
 
 class Topic(dict):
     """
     topic for event hook. e.g. "TickData.002410.SZ.Realtime"
     """
 
@@ -26,37 +25,41 @@
 
     def __bool__(self):
         return True
 
     def __hash__(self):
         return self.value.__hash__()
 
-    def match(self, topic: str) -> Topic | None:
+    def match(self, topic: str) -> Self | None:
         if self._value == topic:
-            return self.__class__(topic=topic)
+            # return self.__class__(topic=topic)
+            return self
         else:
             return None
 
     @classmethod
-    def cast(cls, topic: Topic | str | Enum, dtype=None) -> Topic:
-        if isinstance(topic, Enum):
-            topic = topic.value
-        elif isinstance(topic, Topic):
+    def cast(cls, topic: Self | str | Enum, dtype: Type[Self] = None) -> Self:
+        if isinstance(topic, cls):
             return topic
-
-        if dtype is None:
-            if re.search(r'{(.+?)}', topic):
-                t = PatternTopic(pattern=topic)
-            elif '*' in topic or '+' in topic or '|' in topic:
-                re.compile(pattern=topic)
-                t = RegularTopic(pattern=topic)
+        elif isinstance(topic, Enum):
+            t = topic.value
+            return cls.cast(t)
+        elif isinstance(topic, str):
+            if dtype is None:
+                if re.search(r'{(.+?)}', topic):
+                    t = PatternTopic(pattern=topic)
+                elif '*' in topic or '+' in topic or '|' in topic:
+                    re.compile(pattern=topic)
+                    t = RegularTopic(pattern=topic)
+                else:
+                    t = Topic(topic=topic)
             else:
-                t = Topic(topic=topic)
+                t = dtype(topic)
         else:
-            t = dtype(topic)
+            raise NotImplementedError(f'Can not cast {topic} into {cls}.')
 
         return t
 
     @property
     def value(self) -> str:
         return self._value
 
@@ -85,26 +88,49 @@
 
     def __init__(self, pattern: str):
         super().__init__(topic=pattern)
 
     def __call__(self, **kwargs):
         return self.format_map(kwargs)
 
+    # @classmethod
+    # def extract_mapping(cls, target: str, pattern: str):
+    #     pattern = re.escape(pattern)
+    #     regex = re.sub(r'\\{(.+?)\\}', r'(?P<_\1>.+)', pattern)
+    #     match = re.match(regex, target)
+    #     if match:
+    #         values = list(match.groups())
+    #         keys = re.findall(r'\\{(.+?)\\}', pattern)
+    #         m = dict(zip(keys, values))
+    #         return m
+    #     else:
+    #         raise Topic.Error(f'pattern {pattern} not in string {target} found!')
+
     @classmethod
     def extract_mapping(cls, target: str, pattern: str):
-        pattern = re.escape(pattern)
-        regex = re.sub(r'\\{(.+?)\\}', r'(?P<_\1>.+)', pattern)
-        match = re.match(regex, target)
-        if match:
-            values = list(match.groups())
-            keys = re.findall(r'\\{(.+?)\\}', pattern)
-            m = dict(zip(keys, values))
-            return m
-        else:
-            raise Topic.Error(f'pattern {pattern} not in string {target} found!')
+        dictionary = {}
+
+        result_parts = target.split('.')
+        pattern_parts = pattern.split('.')
+
+        # Check if the number of parts in result and pattern are the same
+        if len(result_parts) != len(pattern_parts):
+            return dictionary
+
+        # Generate the mapping dictionary
+        for result_part, pattern_part in zip(result_parts, pattern_parts):  # type: str
+            if pattern_part[0] == '{' and pattern_part[-1] == '}':
+                content = pattern_part[1:-1]
+                dictionary[content] = result_part
+            else:
+                if result_part != pattern_part:
+                    dictionary.clear()
+                    break
+
+        return dictionary
 
     def format_map(self, mapping: dict) -> Topic:
         for key in self.keys():
             if key not in mapping:
                 mapping[key] = f'{{{key}}}'
 
         return Topic.cast(self._value.format_map(mapping))
```

### Comparing `PyEventEngine-0.2.1/EventEngine/Core/__init__.py` & `pyeventengine-0.3.0/EventEngine/Core/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-from __future__ import annotations
-
 import logging
 import sys
 import time
 
-__all__ = ['set_logger', 'LOG_LEVEL_EVENT', 'Topic', 'RegularTopic', 'PatternTopic', 'EventHook', 'EventEngine', 'LOGGER']
+__all__ = ['set_logger', 'LOG_LEVEL_EVENT', 'Topic', 'RegularTopic', 'PatternTopic', 'EventHook', 'EventEngine', 'LOGGER', 'use_cpp_override']
 LOGGER: logging.Logger | None = None
+DEBUG = False
 LOG_LEVEL = logging.INFO
-LOG_LEVEL_EVENT = LOG_LEVEL - 1
+LOG_LEVEL_EVENT = LOG_LEVEL - 5
 
 
 class ColoredFormatter(logging.Formatter):
     """Logging Formatter to add colors and count warning / errors"""
 
     def __init__(self, fmt=None, datefmt=None, style='{', validate=True):
         self.format_str = '[{asctime} {name} - {threadName} - {module}:{lineno} - {levelname}] {message}' if fmt is None else fmt
@@ -79,19 +78,22 @@
     return LOGGER
 
 
 def set_logger(logger: logging.Logger):
     global LOGGER
     LOGGER = logger
 
+    _event.LOGGER = LOGGER.getChild('Event')
 
-_ = get_logger()
 
-# use c++ optimized module
-try:
-    from ._Topic_c import Topic, RegularTopic, PatternTopic
-except Exception as _:
-    from ._Topic import Topic, RegularTopic, PatternTopic
+def use_cpp_override():
+    try:
+        from ._topic_c import Topic, RegularTopic, PatternTopic
+        from . import _topic as _Topic_native
+    except Exception as _:
+        LOGGER.warning(_)
 
-    LOGGER.warning(_)
 
-from ._Event import EventHook, EventEngine
+_ = get_logger()
+
+from ._topic import Topic, RegularTopic, PatternTopic
+from ._event import EventHook, EventEngine
```

### Comparing `PyEventEngine-0.2.1/EventEngine/cpp/topic_api.cpp` & `pyeventengine-0.3.0/EventEngine/cpp/topic_api.cpp`

 * *Files 6% similar despite different names*

```diff
@@ -1,70 +1,80 @@
 #include <iostream>
 #include <regex>
 #include <string>
 #include <unordered_map>
+#include <utility>
 #include <vector>
 
 extern "C" {
-    #include <stdio.h>
-    #include <stdlib.h>
+#include <stdlib.h>
 }
 
 class Topic : public std::unordered_map<std::string, std::string> {
 public:
     class Error : public std::exception {
     public:
-        explicit Error(const std::string& msg) : message(msg) {}
-        const char* what() const noexcept override { return message.c_str(); }
+        explicit Error(std::string msg) : message(std::move(msg)) {}
+
+        [[nodiscard]] const char *what() const noexcept override { return message.c_str(); }
 
     private:
         std::string message;
     };
 
-    explicit Topic(const std::string& topic) : _value(topic) {}
+    explicit Topic(std::string topic) : _value(std::move(topic)) {}
 
     std::string value() const { return _value; }
 
-    Topic match(const std::string& topic) const {
+    virtual Topic match(const std::string &topic) const {
         if (_value == topic) {
             return Topic(topic);
         } else {
             return Topic("");
         }
     }
 
     std::string _value;
 };
 
 class RegularTopic : public Topic {
 public:
-    explicit RegularTopic(const std::string& pattern) : Topic(pattern) {}
+    explicit RegularTopic(const std::string &pattern) : Topic(pattern) {}
 
-    Topic match(const std::string& topic) const {
-        std::regex regex(_value);
+    static int is_match(const std::string &topic, const std::string &pattern) {
+        std::regex regex(pattern);
         if (std::regex_match(topic, regex)) {
+            return 1;
+        } else {
+            return 0;
+        }
+    }
+
+    Topic match(const std::string &topic) const override {
+        int result = is_match(topic, _value);
+        if (result == 1) {
             Topic match(topic);
             match["pattern"] = _value;
             return match;
         } else {
             return Topic("");
         }
     }
 };
 
 class PatternTopic : public Topic {
 public:
-    explicit PatternTopic(const std::string& pattern) : Topic(pattern) {}
+    explicit PatternTopic(const std::string &pattern) : Topic(pattern) {}
 
-    Topic format_map(const std::unordered_map<std::string, std::string>& mapping) const {
+    Topic format_map(const std::unordered_map<std::string, std::string> &mapping) const {
         std::string result = _value;
 
         std::vector<std::string> contentVec = keys();
 
-        for (const auto& content : contentVec) {
+        for (const auto &content: contentVec) {
             auto it = mapping.find(content);
             if (it != mapping.end()) {
                 std::string replacement = it->second;
                 std::string searchStr = "{" + content + "}";
                 size_t startPos = result.find(searchStr);
                 while (startPos != std::string::npos) {
                     result.replace(startPos, searchStr.length(), replacement);
@@ -75,15 +85,14 @@
 
         return Topic(result);
     }
 
     std::vector<std::string> keys() const {
         std::vector<std::string> contentVec;
         std::vector<std::string> keys;
-        std::string pattern = _value;
 
         size_t startPos = _value.find('{');
         size_t endPos;
 
         while (startPos != std::string::npos) {
             endPos = _value.find('}', startPos + 1);
             if (endPos == std::string::npos)
@@ -94,26 +103,26 @@
 
             startPos = _value.find('{', endPos + 1);
         }
 
         return keys;
     }
 
-    Topic match(const std::string& topic) const {
-        try {
-            std::unordered_map<std::string, std::string> keyword_dict = extract_mapping(topic, _value);
-            Topic match(topic);
-            match.insert(keyword_dict.begin(), keyword_dict.end());
-            return match;
-        } catch (const Error&) {
+    Topic match(const std::string &topic) const override {
+        std::unordered_map<std::string, std::string> keyword_dict = extract_mapping(topic, _value);
+        if (keyword_dict.empty()) {
             return Topic("");
         }
+
+        Topic match(topic);
+        match.insert(keyword_dict.begin(), keyword_dict.end());
+        return match;
     }
 
-    static std::unordered_map<std::string, std::string> extract_mapping(const std::string& target, const std::string& pattern) {
+    static std::unordered_map<std::string, std::string> extract_mapping(const std::string &target, const std::string &pattern) {
         std::unordered_map<std::string, std::string> dictionary;
 
         std::vector<std::string> resultParts;
         std::vector<std::string> patternParts;
 
         // Split the result string by '.'
         size_t startPos = 0;
@@ -137,15 +146,14 @@
             dotPos = pattern.find('.', startPos);
         }
         lastPart = pattern.substr(startPos);
         patternParts.push_back(lastPart);
 
         // Check if the number of parts in result and pattern are the same
         if (resultParts.size() != patternParts.size()) {
-            throw Error("Pattern not match");
             return dictionary;
         }
 
         // Generate the mapping dictionary
         size_t numParts = resultParts.size();
         for (size_t i = 0; i < numParts; ++i) {
             std::string resultPart = resultParts[i];
@@ -153,121 +161,128 @@
 
             if (patternPart.front() == '{' && patternPart.back() == '}') {
                 std::string content = patternPart.substr(1, patternPart.length() - 2);
                 dictionary[content] = resultPart;
             } else {
                 if (resultPart != patternPart) {
                     dictionary.clear();
-                    throw Error("Pattern not match");
                     return dictionary;
                 }
             }
         }
-
         return dictionary;
     }
 };
 
 extern "C" {
-    Topic* create_topic(const char* topic) {
-        return new Topic(topic);
-    }
+Topic *create_topic(const char *topic) {
+    return new Topic(topic);
+}
 
-    void get_topic_value(const Topic* topic, char* buffer, size_t bufferSize) {
-        std::string value = topic->value();
-        strncpy(buffer, value.c_str(), bufferSize - 1);
-        buffer[bufferSize - 1] = '\0';
-    }
+void get_topic_value(const Topic *topic, char *buffer, size_t bufferSize) {
+    std::string value = topic->value();
+    strncpy(buffer, value.c_str(), bufferSize - 1);
+    buffer[bufferSize - 1] = '\0';
+}
 
-    const char* get_topic_value_no_buffer(const Topic* topic) {
-        return topic->_value.c_str();
-    }
+const char *get_topic_value_no_buffer(const Topic *topic) {
+    return topic->_value.c_str();
+}
 
-    void delete_topic(Topic* topic) {
-        delete topic;
-    }
+void delete_topic(Topic *topic) {
+    delete topic;
+}
 
-    Topic* match_topic(const Topic* topic, const char* match_topic) {
-        return new Topic(topic->match(match_topic));
-    }
+Topic *match_topic(const Topic *topic, const char *match_topic) {
+    return new Topic(topic->match(match_topic));
+}
 
-    RegularTopic* create_regular_topic(const char* pattern) {
-        return new RegularTopic(pattern);
-    }
+RegularTopic *create_regular_topic(const char *pattern) {
+    return new RegularTopic(pattern);
+}
 
-    Topic* match_regular_topic(const RegularTopic* topic, const char* match_topic) {
-        return new Topic(topic->match(match_topic));
-    }
+Topic *match_regular_topic(const RegularTopic *topic, const char *match_topic) {
+    return new Topic(topic->match(match_topic));
+}
 
-    PatternTopic* create_pattern_topic(const char* pattern) {
-        return new PatternTopic(pattern);
-    }
+PatternTopic *create_pattern_topic(const char *pattern) {
+    return new PatternTopic(pattern);
+}
 
-    Topic* match_pattern_topic(const PatternTopic* topic, const char* match_topic) {
-        return new Topic(topic->match(match_topic));
-    }
+Topic *match_pattern_topic(const PatternTopic *topic, const char *match_topic) {
+    return new Topic(topic->match(match_topic));
+}
 
-    std::vector<std::string>* get_pattern_topic_keys(const PatternTopic* topic) {
-        return new std::vector<std::string>(topic->keys());
-    }
+std::vector<std::string> *get_pattern_topic_keys(const PatternTopic *topic) {
+    return new std::vector<std::string>(topic->keys());
+}
 
-    void extract_mapping(const char* target, const char* pattern, std::vector<std::string>* keys, std::vector<std::string>* values) {
-        std::string target_str(target);
-        std::string pattern_str(pattern);
-
-        std::unordered_map<std::string, std::string> mapping = PatternTopic::extract_mapping(target_str, pattern_str);
-
-        // Populate the keys and values vectors
-        for (const auto& entry : mapping) {
-            keys->push_back(entry.first);
-            values->push_back(entry.second);
-        }
-    }
+int is_regular_match(const char *topic, const char *pattern) {
+    std::string topicStr(topic);
+    std::string patternStr(pattern);
+    int result = RegularTopic::is_match(topicStr, patternStr);
+    return result;
+}
 
-    const char* get_vector_value(const std::vector<std::string>* vec, int index) {
-        if (index >= 0 && index < static_cast<int>(vec->size()))
-            return vec->at(index).c_str();
-        else
-            return "";
+void extract_mapping(const char *target, const char *pattern, std::vector<std::string> *keys, std::vector<std::string> *values) {
+    std::string target_str(target);
+    std::string pattern_str(pattern);
+
+    std::unordered_map<std::string, std::string> mapping = PatternTopic::extract_mapping(target_str, pattern_str);
+
+    // Populate the keys and values vectors
+    for (const auto &entry: mapping) {
+        keys->push_back(entry.first);
+        values->push_back(entry.second);
     }
+}
 
-    const int vector_size(const std::vector<std::string>* v){
-        return v->size();
-    }
+const char *get_vector_value(const std::vector<std::string> *vec, int index) {
+    if (index >= 0 && index < static_cast<int>(vec->size()))
+        return vec->at(index).c_str();
+    else
+        return "";
+}
 
-    void delete_vector(std::vector<std::string>* vec) {
-        delete vec;
-    }
+int vector_size(const std::vector<std::string> *vec) {
+    return vec->size();
+}
+
+void delete_vector(const std::vector<std::string> *vec) {
+    delete vec;
+}
 }
 
 int main() {
     Topic topic("TickData.002410.SZ.Realtime");
     std::cout << topic.value() << std::endl;
 
     RegularTopic regularTopic("TickData.(.+).((SZ)|(SH)).((Realtime)|(History))");
     Topic match1 = regularTopic.match("TickData.1234.SZ.Realtime");
     Topic match2 = regularTopic.match("OtherData.5678.SH.History");
     std::cout << match1.value() << std::endl;
     std::cout << match2.value() << std::endl;
 
     PatternTopic patternTopic("TickData.{symbol}.{market}.{flag}");
-    for (std::string i: patternTopic.keys())
-    std::cout << i << std::endl;
+    for (const std::string &i: patternTopic.keys())
+        std::cout << i << std::endl;
 
-    Topic formatted = patternTopic.format_map({{"symbol", "AAPL"}, {"market", "NASDAQ"}, {"flag", "Realtime"}});
+    Topic formatted = patternTopic.format_map({{"symbol", "AAPL"},
+                                               {"market", "NASDAQ"},
+                                               {"flag",   "Realtime"}});
     std::cout << formatted.value() << std::endl;
 
     Topic match3 = patternTopic.match("TickData.ABC.NYSE.Realtime");
     Topic match4 = patternTopic.match("OtherData.XYZ.LSE.History");
 
     std::cout << "topic: " << match3.value() << std::endl;
-    for (const auto& entry : match3) {
+    for (const auto &entry: match3) {
         std::cout << entry.first << " : " << entry.second << std::endl;
     }
 
     std::cout << "topic: " << match4.value() << std::endl;
-    for (const auto& entry : match4) {
+    for (const auto &entry: match4) {
         std::cout << entry.first << " : " << entry.second << std::endl;
     }
 
     return 0;
 }
```

### Comparing `PyEventEngine-0.2.1/LICENSE` & `pyeventengine-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `PyEventEngine-0.2.1/PKG-INFO` & `pyeventengine-0.3.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 Metadata-Version: 2.1
 Name: PyEventEngine
-Version: 0.2.1
+Version: 0.3.0
 Summary: Basic event engine
 Home-page: https://github.com/BolunHan/PyEventEngine.git
 Author: Bolun.Han
 Author-email: Bolun.Han@outlook.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # PyEventEngine
```

### Comparing `PyEventEngine-0.2.1/PyEventEngine.egg-info/PKG-INFO` & `pyeventengine-0.3.0/PyEventEngine.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 Metadata-Version: 2.1
 Name: PyEventEngine
-Version: 0.2.1
+Version: 0.3.0
 Summary: Basic event engine
 Home-page: https://github.com/BolunHan/PyEventEngine.git
 Author: Bolun.Han
 Author-email: Bolun.Han@outlook.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # PyEventEngine
```

### Comparing `PyEventEngine-0.2.1/README.md` & `pyeventengine-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `PyEventEngine-0.2.1/setup.py` & `pyeventengine-0.3.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,14 +36,16 @@
     include_package_data=True,
     package_data={
     },
     classifiers=[
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.8',
     license='MIT',
     install_requires=[],
     ext_modules=[
         setuptools.extension.Extension(r'EventEngine.topic_api', sources=[r'EventEngine/cpp/topic_api.cpp'], include_dirs=[], language='c++', optional=True),
```

