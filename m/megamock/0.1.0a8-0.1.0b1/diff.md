# Comparing `tmp/megamock-0.1.0a8.tar.gz` & `tmp/megamock-0.1.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "megamock-0.1.0a8.tar", max compression
+gzip compressed data, was "megamock-0.1.0b1.tar", max compression
```

## Comparing `megamock-0.1.0a8.tar` & `megamock-0.1.0b1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1072 2023-02-23 18:15:29.866540 megamock-0.1.0a8/LICENSE
--rw-r--r--   0        0        0    10248 2023-04-05 21:01:46.160410 megamock-0.1.0a8/README.md
--rw-r--r--   0        0        0      282 2023-04-11 18:50:21.187235 megamock-0.1.0a8/megamock/__init__.py
--rw-r--r--   0        0        0     3055 2023-04-11 18:50:21.187235 megamock-0.1.0a8/megamock/import_machinery.py
--rw-r--r--   0        0        0     3881 2023-04-11 18:50:21.187235 megamock-0.1.0a8/megamock/import_references.py
--rw-r--r--   0        0        0    28546 2023-04-11 18:50:21.187235 megamock-0.1.0a8/megamock/megamocks.py
--rw-r--r--   0        0        0    13846 2023-04-11 18:50:21.187235 megamock-0.1.0a8/megamock/megapatches.py
--rw-r--r--   0        0        0     3672 2023-04-11 18:50:21.187235 megamock-0.1.0a8/megamock/megas.py
--rw-r--r--   0        0        0     3066 2023-04-05 19:30:52.816855 megamock-0.1.0a8/megamock/name_words.py
--rw-r--r--   0        0        0        0 2023-03-15 05:28:12.131080 megamock-0.1.0a8/megamock/plugins/__init__.py
--rw-r--r--   0        0        0      949 2023-03-27 18:29:48.174052 megamock-0.1.0a8/megamock/plugins/pytest.py
--rw-r--r--   0        0        0      303 2023-04-11 18:50:21.187235 megamock-0.1.0a8/megamock/type_util.py
--rw-r--r--   0        0        0     1135 2023-04-11 18:51:00.884290 megamock-0.1.0a8/pyproject.toml
--rw-r--r--   0        0        0    11352 1970-01-01 00:00:00.000000 megamock-0.1.0a8/setup.py
--rw-r--r--   0        0        0    11236 1970-01-01 00:00:00.000000 megamock-0.1.0a8/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-02-23 18:15:29.866540 megamock-0.1.0b1/LICENSE
+-rw-r--r--   0        0        0    10248 2023-04-05 21:01:46.160410 megamock-0.1.0b1/README.md
+-rw-r--r--   0        0        0      282 2023-04-11 18:50:21.187235 megamock-0.1.0b1/megamock/__init__.py
+-rw-r--r--   0        0        0     3055 2023-04-11 18:50:21.187235 megamock-0.1.0b1/megamock/import_machinery.py
+-rw-r--r--   0        0        0     3881 2023-04-11 18:50:21.187235 megamock-0.1.0b1/megamock/import_references.py
+-rw-r--r--   0        0        0    32321 2023-04-24 21:52:52.332384 megamock-0.1.0b1/megamock/megamocks.py
+-rw-r--r--   0        0        0    14610 2023-04-23 20:20:44.011780 megamock-0.1.0b1/megamock/megapatches.py
+-rw-r--r--   0        0        0     3672 2023-04-11 18:50:21.187235 megamock-0.1.0b1/megamock/megas.py
+-rw-r--r--   0        0        0     3066 2023-04-05 19:30:52.816855 megamock-0.1.0b1/megamock/name_words.py
+-rw-r--r--   0        0        0        0 2023-03-15 05:28:12.131080 megamock-0.1.0b1/megamock/plugins/__init__.py
+-rw-r--r--   0        0        0      949 2023-03-27 18:29:48.174052 megamock-0.1.0b1/megamock/plugins/pytest.py
+-rw-r--r--   0        0        0      303 2023-04-11 18:50:21.187235 megamock-0.1.0b1/megamock/type_util.py
+-rw-r--r--   0        0        0     1292 2023-04-24 22:01:38.494846 megamock-0.1.0b1/pyproject.toml
+-rw-r--r--   0        0        0    11352 1970-01-01 00:00:00.000000 megamock-0.1.0b1/setup.py
+-rw-r--r--   0        0        0    11236 1970-01-01 00:00:00.000000 megamock-0.1.0b1/PKG-INFO
```

### Comparing `megamock-0.1.0a8/LICENSE` & `megamock-0.1.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `megamock-0.1.0a8/README.md` & `megamock-0.1.0b1/README.md`

 * *Files identical despite different names*

### Comparing `megamock-0.1.0a8/megamock/import_machinery.py` & `megamock-0.1.0b1/megamock/import_machinery.py`

 * *Files identical despite different names*

### Comparing `megamock-0.1.0a8/megamock/import_references.py` & `megamock-0.1.0b1/megamock/import_references.py`

 * *Files identical despite different names*

### Comparing `megamock-0.1.0a8/megamock/megamocks.py` & `megamock-0.1.0b1/megamock/megamocks.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import traceback
 from abc import ABCMeta
 from collections import defaultdict
 from dataclasses import dataclass, field
 from inspect import isawaitable, isclass, iscoroutinefunction
 from typing import Any, Callable, Generic, Literal, TypeVar, cast, overload
 from unittest import mock
+from unittest.mock import create_autospec
 
 from megamock import name_words
 from megamock.type_util import MISSING, MISSING_TYPE
 
 T = TypeVar("T")
 U = TypeVar("U")
 
@@ -121,14 +122,15 @@
     spy: Any | None = None
     attr_assignments: dict[str, list[AttributeAssignment]] = field(
         default_factory=lambda: defaultdict(list)
     )
     spied_access: dict[str, list[SpyAccess]] = field(
         default_factory=lambda: defaultdict(list)
     )
+    name: str | None = None
 
     _wrapped_mock: _base_mock_types | None = None
 
 
 class _MegaMockMixin(Generic[T, U]):
     """
     Mixin used by MegaMock, NonCallableMegaMock, and AsyncMegaMock
@@ -169,14 +171,15 @@
             mock.Mock
             | mock.MagicMock
             | mock.NonCallableMock
             | mock.NonCallableMagicMock
             | None
         ) = None,
         _parent_mega_mock: _MegaMockMixin | None = None,
+        _name: str | None = None,
         _merged_type: type[U] | None = None,
         # warning: kwargs to MagicMock may not work correctly! Use at your own risk!
         **kwargs,
     ) -> None:
         """
         :param spec: The MegaMock's specification (template object)
         :param wraps: An object to wrap, this is included for legacy support. Prefer spy
@@ -188,27 +191,31 @@
             the mock will be a class. By default this is True. This must be omitted or
             False for the AsyncMock
         :param side_effect: The side effect to use for the mock. Exceptoins are raised,
             fuctions are called, and iterables are returned in order in subsequent calls
         :param return_value: The return value to use for the mock.
         :param _wraps_mock: the wrapped mock, for internal use
         :param _parent_mega_mock: The parent MegaMock, for internal use
+        :param _name: The name of the mock, for internal use
         """
         self.meganame = self._generate_meganame()
+
         self._linked_mock = None
         megamock_attrs = MegaMockAttributes()
+        megamock_attrs.name = self._generate_mock_name(spec, _parent_mega_mock, _name)
         self._wrapped_legacy_mock = None
         self._mock_return_value_cache = MISSING
 
         megamock_attrs.parent = _parent_mega_mock
         if instance is None:
             if iscoroutinefunction(spec) or isawaitable(spec):
                 instance = False
             else:
                 instance = True
+
         if wraps and spy:
             # if spy is used, then the spied value is also wrapped
             raise Exception("Cannot both wrap and spy")
 
         megamock_attrs.wraps = wraps = wraps or spy
         megamock_attrs.spec = spec
         if wraps and not _wraps_mock:
@@ -241,14 +248,43 @@
             megamock_attrs._wrapped_mock = _wraps_mock
 
         # must be last as the setattr behavior will change after this
         self.megamock = megamock_attrs
         # shortcut to the wrapped mock to avoid performance penalty
         self._wrapped_legacy_mock = megamock_attrs._wrapped_mock
 
+    def _generate_mock_name(
+        self,
+        spec: Any,
+        parent_mega_mock: _MegaMockMixin | None,
+        name: str | None,
+    ) -> str:
+        mock_name = ""
+        if spec is None:
+            mock_name = "MegaMock()"
+        if parent_mega_mock is not None:
+            mock_name = parent_mega_mock.megamock.name or "MegaMock()"
+            mock_name += f".{name}" if name else "()"
+        try:
+            if spec is not None:
+                spec_name = getattr(spec, "__name__", None)
+                if spec_name is not None:
+                    if mock_name:
+                        mock_name += "."
+                    mock_name += spec_name
+                else:
+                    if mock_name:
+                        mock_name += " -> "
+                    mock_name += spec.__class__.__name__
+        except AttributeError:
+            mock_name += "mock"
+            if parent_mega_mock:
+                mock_name += "()"
+        return mock_name
+
     def _generate_meganame(self) -> str:
         """
         Generate a random adjective / noun / number name for the mock
         """
         return (
             f"{random.choice(name_words.ADJECTIVES)} "
             f"{random.choice(name_words.NOUNS)} "
@@ -272,15 +308,17 @@
         if self._wrapped_legacy_mock is not None:
             if (val := self._mock_return_value_cache) is MISSING:
                 if isinstance(
                     self._mock_return_value_,
                     mock.NonCallableMagicMock | mock.NonCallableMock,
                 ):
                     val = self._mock_return_value_cache = MegaMock.from_legacy_mock(
-                        self._mock_return_value_, None, self.megamock.wraps
+                        self._mock_return_value_,
+                        None,
+                        self.megamock.wraps,
                     )
                 else:
                     val = self._mock_return_value_cache = self._mock_return_value_
             return val
         return self.__dict__.get(
             "_mock_return_value", self.__class__._mock_return_value
         )
@@ -304,21 +342,29 @@
         if (wrapped := self._wrapped_legacy_mock) is not None:
             result = getattr(wrapped, key)
             if not isinstance(result, _MegaMockMixin) and isinstance(
                 result, mock.NonCallableMock | mock.NonCallableMagicMock
             ):
                 mega_result = MegaMock.from_legacy_mock(
                     result,
-                    getattr(self.megamock.spec, key, None),
+                    getattr(self.megamock.spec, key, self.megamock.spec),
                     self.megamock.wraps,
                     parent_megamock=self,
                 )
+                # return_value is referenced when a call is made.
+                # This actually accesses _mock_return_value
+                if key == "_mock_return_value":
+                    mega_result.megamock.name = f"{self.megamock.name}()"
+                else:
+                    mega_result.megamock.name = f"{self.megamock.name}.{key}"
                 setattr(wrapped, key, mega_result)
                 return mega_result
             return result
+        if not self.megamock.spec and not self.megamock.wraps:
+            return self._get_child_mock(_name=key)
         raise AttributeError(key)
 
     def __setattr__(self, key, value) -> None:
         if key in ("megamock", "_wrapped_legacy_mock"):
             self.__dict__[key] = value
             return
         if key in self.USE_SUPER_SETATTR:
@@ -439,15 +485,15 @@
         Link the call behavior to another mock. This is currently used by `MegaPatch.it`
         to link the class (type) mock with the class (instance) mock.
         """
         self.__dict__["_linked_mock"] = other
 
     def __repr__(self) -> str:
         return (
-            f"<{self.__class__.__name__} name='{self._mock_name}' "
+            f"<{self.__class__.__name__} name='{self.megamock.name}' "
             f"| {self.meganame}>"
         )
 
 
 class MegaMock(_MegaMockMixin[T, U], mock.MagicMock, Generic[T, U]):
     """
     The primary MegaMock class. Use MegaMock.it if providing a spec,
@@ -678,26 +724,71 @@
                     # instance of a class Mock
                     return cast(Callable, spec)(self.megamock.parent, *args, **kwargs)
                 return cast(Callable, spec)(*args, **kwargs)
             if self._linked_mock is not None:
                 # why is the mock not called as a bound method
                 return self._linked_mock(self, *args, **kwargs)
             result = wrapped(*args, **kwargs)
+            self._validate_spec_was_callable()
             if not isinstance(result, _MegaMockMixin) and isinstance(
                 result, mock.NonCallableMock | mock.NonCallableMagicMock
             ):
+                call_spec = self._get_call_spec()
                 mega_result = MegaMock.from_legacy_mock(
-                    result,
-                    None,
-                    self.megamock.wraps,
+                    result, call_spec, self.megamock.wraps, parent_megamock=self
                 )
                 return mega_result
             return result
         return super().__call__(*args, **kwargs)
 
+    def _validate_spec_was_callable(self) -> None:
+        """
+        The create_autospec functionality properly creates a non-callable mock object.
+        So, for example, MegaMock.it(Foo) properly indicates that the instance Foo is
+        not callable.
+
+        However, a nested call to a non-callable mock object will not be properly
+        indicated as non-callable. For example, if we have a class Foo with a mocked
+        method that returns a non-callable Bar, then the autospec'ed object will create
+        a callable mock object in place of a mock Bar.
+
+        In this case, _get_call_spec is used to give the mocked method a spec for a Bar
+        instance, based on the return type annotation. This function then checks that
+        spec and enforces the callability of it.
+
+        In other words:
+
+        MegaMock.it(Foo)()  <-- _validate_spec_was_callable is not needed
+        MegaMock.it(Foo).do_something()() <-- _validate_spec_was_callable is needed
+        """
+        if self.megamock.wraps is not None:
+            return
+        if self.megamock.spec is None:
+            return
+        if not callable(self.megamock.spec):
+            raise TypeError(f"{self.megamock.spec} is not callable")
+
+    def _get_call_spec(self) -> Any:
+        """
+        Determine what the spec is for a function's return based on the annnotations.
+
+        This is used to a create a mock object with the same traits as the spec.
+        """
+        if self.megamock.spec is None:
+            return None
+        if isclass(self.megamock.spec) and hasattr(self.megamock.spec, "__call__"):
+            spec = self.megamock.spec.__call__
+        else:
+            spec = self.megamock.spec
+        annotations = getattr(spec, "__annotations__", {})
+        return_type = annotations.get("return", None)
+        if return_type is None:
+            return None
+        return create_autospec(return_type, instance=True)
+
 
 class NonCallableMegaMock(
     _MegaMockMixin[T, U], mock.NonCallableMagicMock, Generic[T, U]
 ):
     @staticmethod
     def it(
         spec: T | None = None,
```

### Comparing `megamock-0.1.0a8/megamock/megapatches.py` & `megamock-0.1.0b1/megamock/megapatches.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 
+import functools
 import inspect
 import logging
 import sys
 from functools import cached_property
 from types import ModuleType
 from typing import Any, Callable, Generic, Iterable, TypeVar, cast
 from unittest import mock
@@ -65,32 +66,37 @@
     ) -> None:
         self._patches = patches
         self._thing: Any | None = thing
         self._new_value: MegaMock = new_value
         self._return_value = return_value
         self._mocker = mocker
 
+        self._started = False
+
     @property
     def patches(self) -> list[mock._patch]:
         return list(self._patches)
 
     @property
     def thing(self) -> Any:
         return self._thing
 
     @property
     def new_value(self) -> MegaMock[T, U] | Any:
         return self._new_value
 
+    def new_value_is_mock(self) -> bool:
+        val = self.new_value
+        return isinstance(val, MegaMock) or hasattr(val, "return_value")
+
     @property
     def mock(self) -> MegaMock[T, U]:
-        val = self.new_value
-        if not isinstance(val, MegaMock) and not hasattr(val, "return_value"):
-            raise ValueError(f"New value {val!r} is not a mock!")
-        return val
+        if not self.new_value_is_mock():
+            raise ValueError(f"New value {self.new_value!r} is not a mock!")
+        return self.new_value
 
     @property
     def megainstance(self) -> U:
         return self.mock.megainstance
 
     @property
     def return_value(self) -> MegaMock[T, U]:
@@ -130,30 +136,56 @@
         """
         try:
             self.return_value.__exit__.side_effect = new_side_effect  # type: ignore
         except AttributeError:
             raise ValueError("Not a context manager")
 
     def start(self) -> None:
+        if self._started:
+            return
         # support for pytest-mock and similar
         if not hasattr(self._mocker, "stopall"):
             # built-in mock
             for patch in self._patches:
                 patch.start()
         MegaPatch._active_patches.add(self)
+        self._started = True
 
     def stop(self) -> None:
         # support for pytest-mock and similar
         if hasattr(self._mocker, "stopall"):
             self._mocker.stopall()
         else:
             # built-in mock
             for patch in self._patches:
                 patch.stop()
         MegaPatch._active_patches.remove(self)
+        self._started = False
+
+    def __enter__(self) -> MegaPatch[T, U]:
+        self.start()
+        return self
+
+    def __exit__(self, *args: Any) -> None:
+        self.stop()
+
+    def __call__(self, func) -> Callable[..., Any]:
+        """
+        Decorator to patch a function
+        """
+
+        @functools.wraps(func)
+        def wrapper(*args: Any, **kwargs: Any) -> Any:
+            self.start()
+            try:
+                return func(*args, **kwargs)
+            finally:
+                self.stop()
+
+        return wrapper
 
     @staticmethod
     def active_patches() -> list[MegaPatch]:
         return list(MegaPatch._active_patches)
 
     @staticmethod
     def stop_all() -> None:
```

### Comparing `megamock-0.1.0a8/megamock/megas.py` & `megamock-0.1.0b1/megamock/megas.py`

 * *Files identical despite different names*

### Comparing `megamock-0.1.0a8/megamock/name_words.py` & `megamock-0.1.0b1/megamock/name_words.py`

 * *Files identical despite different names*

### Comparing `megamock-0.1.0a8/megamock/plugins/pytest.py` & `megamock-0.1.0b1/megamock/plugins/pytest.py`

 * *Files identical despite different names*

### Comparing `megamock-0.1.0a8/pyproject.toml` & `megamock-0.1.0b1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "megamock"
-version = "0.1.0-alpha.8"
+version = "0.1.0-beta.1"
 description = "Mega mocking capabilities - stop using dot-notated paths!"
 authors = ["James Hutchison <jamesghutchison@proton.me>"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/JamesHutchison/megamock"
 repository = "https://github.com/JamesHutchison/megamock"
 keywords = ["mock", "test"]
@@ -25,17 +25,21 @@
 [tool.poetry.group.dev.dependencies]
 black = "^23.1.0"
 flake8 = "^6.0.0"
 pytest = "^7.2.1"
 pytest-asyncio = "^0.20.3"
 mypy = "^1.1.1"
 
+[tool.poetry.group.dev-hot-reloading.dependencies]
+pytest-hot-reloading = "^0.1.0a2"
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
+# addopts = "-p megamock.plugins.pytest -p pytest_hot_reloading.plugin"
 addopts = "-p megamock.plugins.pytest"
 asyncio_mode = "auto"
 
 [tool.isort]
 profile = "black"
```

### Comparing `megamock-0.1.0a8/setup.py` & `megamock-0.1.0b1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['asttokens>=2.2.1,<2.3.0', 'varname[asttokens]>=0.10.0,<0.11.0']
 
 setup_kwargs = {
     'name': 'megamock',
-    'version': '0.1.0a8',
+    'version': '0.1.0b1',
     'description': 'Mega mocking capabilities - stop using dot-notated paths!',
     'long_description': '# **MegaMock** - _The Developer Experience Upgrade for Python Mocking_\n\nPew pew! Sane defaults for mocking behavior! Patch objects, variables, attributes, etc by passing in the thing in question, rather than passing in dot-delimited path strings! Create tests faster than ever!\n\nSupported Python Versions: 3.10+\n### Installation\n\nPip installation:\n```\npip install megamock\n```\n\n[poetry](https://python-poetry.org/) (as a development dependency):\n```\npoetry add megamock --group=dev\n```\n\n# Why Use MegaMock? (short version)\nMegaMock is a library that provides a better interface for mocking and patching in Python. Its version\nof patch doesn\'t have any gotchas based on how you import something, and it also automatically\ncreates mocks using best practices. Additionally, the generated mock types are unions of the mocked object\nand `MegaMock`, allowing you to better leverage your IDE\'s autocomplete.\n\n![Sample MegaMock vs Mock Comparison](docs/img/megamock-example.gif)\n\nMock:\n\n```python\nclass_mock = mock.create_autospec(ClassICareAbout, instance=True)\n# cmd / alt clicking on "method_call" doesn\'t direct you to the definition\nclass_mock.method_call.return_value = "some value"\n\n# can\'t simply cmd / alt click and go to ClassICareAbout\nwith mock.patch("some.hard.to.remember.and.long.dot.path.ClassICareAbout", class_mock) as mock_instance:\n    do_something()\n```\n\nMegaMock:\n\n```python\n# cmd / alt clicking on ClassICareAbout takes you to the definition\npatch = MegaPatch.it(ClassICareAbout)\nmock_instance = patch.megainstance\n# cmd / alt clicking on "method_call" directs you to the definition\nmock_instance.method_call.return_value = "some value"\n\ndo_something()\n```\n\n# Why Use MegaMock? (long version)\nMegaMock was created to address some shortcomings in the built-in Python library:\n- Legacy code holds back "best practice" defaults, so many developers write sub-optimal mocks\n  that allow things that should not be allowed. Likewise, writing better mocks are more work,\n  so there\'s a tendency to write simpler code because, at that point in time, the developer\n  felt that is all that was needed. MegaMock\'s simple interface provides sane defaults.\n- `mock.patch` is very commonly used, and can work well when `autospec=True`, but has the drawback that\n  you need to pass in a string to the thing that is being patched. Most (all?) IDEs do not properly\n  recognize these strings as references to the objects that are being patched, and thus automated\n  refactoring and reference finding skips them. Likewise, automatically getting a dot referenced path\n  to an object is also commonly missing functionality. This all adds additional burden to the developer.\n  With `MegaPatch`, you can import an object as you normally would into the test, then pass in thing\n  itself you want to patch. This even works for methods, attributes, and nested classes! Additionally, your IDE\'s autocomplete for attributes\n  will work in many situations as well!\n- `mock.patch` has a gotcha where the string you provide must match where the reference lives.\n  So, for example, if you have in `my_module.py`: `from other_module import Thing`, then doing\n  `mock.patch("other_module.Thing")` won\'t actually work, because the reference in `my_module` still\n  points to the original. You can work around this by doing `import other_module` and referencing `Thing`\n  by `other_module.Thing`. MegaMock does not have this problem, and it doesn\'t matter how you import.\n\n## Features\n\nSee the [full features list](FEATURES.md).\n## Example Usage\n\n### Production Code\n```python\nfrom module.submodule import MyClassToMock\n\n\ndef my_method(...):\n    ...\n    a_thing = MyClassToMock(...)\n    do_something_with_a_thing(a_thing)\n    ...\n\n\ndef do_something_with_a_thing(a_thing: MyClassToMock) -> None:\n    result = a_thing.some_method(...)\n    if result == "a value":\n        ...\n```\n\n### Test Code\n```python\nfrom megamock import MegaPatch\nfrom module.submodule import MyClassToMock\n\n\ndef test_something(...):\n    patch = MegaPatch.it(MyClassToMock.some_method)\n    patch.return_value = "a value"\n\n    my_method(...)\n```\n\n## Documentation\n\n### Usage (pytest)\n\nWith [pytest](https://pytest.org), MegaMock is easily leveraged by using the included pytest plugin. You can use it by adding `-p megamock.plugins.pytest`\nto the command line.\n\nCommand line example:\n```\npytest -p megamock.plugins.pytest\n```\n\n`pyproject.toml` example:\n```toml\n[tool.pytest.ini_options]\naddopts = "-p megamock.plugins.pytest"\n```\n\nThe pytest plugin also automatically stops `MegaPatch`es after each test. To disable this behavior, pass in the `--do_not_autostop_megapatches`\ncommand line argument. If `pytest-mock` is installed, the default mocker will be switched to the `pytest-mock` `mocker`.\n\n### Usage (other test frameworks)\n\nIf you\'re not using the pytest plugin, import and execution order is important for MegaMock. When running tests, you will need to execute the `start_import_mod`\nfunction prior to importing any production or test code. You will also want it so the loader is not used in production.\n\n-------------------\n\n**Core Classes**\n\n`MegaMock` - the primary class for a mocked object. This is similar to `MagicMock`. Use `MegaMock.it(MyObject)` to make `MyObject` the [spec](https://docs.python.org/3/library/unittest.mock.html#unittest.mock.create_autospec).\n\n`MegaPatch` - the class for patching. This is similar to `patch`. Use `MegaPath.it(MyObject)` to replace new instances of the `MyObject` class.\n\n`Mega` - helper class for accessing mock attributes without having to memorize the due to lost type inference. Use `Mega(some_megamock)`.\nNote that the `assert_` methods, such as `assert_called_once`, is now `called_once` and returns a boolean. The assertion error\nis stored in `Mega.last_assertion_error`.\n\n--------------------\n\nDependency injection example:\n```python\n\nfrom megamock import MegaMock\n\ndef test_something(...):\n    manager = MegaMock.it(MyManagerClass)\n    service = SomeService(manager)\n    ...\n```\n\nMegaPatch example:\n```python\nfrom elsewhere import Service\n\nfrom megamock import MegaPatch\n\ndef test_something(...):\n    patched = MegaPatch.it(Service.make_external_call)\n    patched.return_value = SomeValue(...)\n    service = SomeService(...)\n\n    code_under_test(service)\n    ...\n```\n\n`MegaMock` objects have the same attributes as regular `MagicMock`s plus `megamock` and `megainstance`\nFor example, `my_mega_mock.megamock.spy` is the object being spied, if set. `my_class_mock.megainstance` is the instance returned when the class is instantiated.\n\nThe [guidance document](GUIDANCE.md) is available to provide in-depth information on using mocking and MegaMock. Continuing reading to\nquickly jump in to examples.\n\n-----------------------\n\n### Learning By Example\n\nAll examples below have the following imports:\n\n```python\nfrom my_module import MyClass\nfrom megamock import Mega, MegaMock, MegaPatch\n```\n\nCreating a mock instance of a class:\n\n```python\nmock_instance = MegaMock.it(MyClass)\n```\n\nCreating a mock class itself:\n\n```python\nmock_class = MegaMock.it(MyClass, instance=False)\n```\n\nSpying an object:\n\n```python\nmy_thing = MyClass()\nspied_class = MegaMock(spy=my_thing)\n\n# ... do stuff with spied_class...\n\nMega(spied_class.some_method).call_args_list  # same as wraps\n\n# check whether a value was accessed\n# if things aren\'t as expected, you can pull up the debugger and see the stack traces\nassert len(spied_class.megamock.spied_access["some_attribute"]) == 1\n\nspy_access_list = spied_class.megamock.spied_access["some_attribute"]\nspy_access: SpyAccess = spy_access_list[0]\nspy_access.attr_value  # shallow copy of what was returned\nspy_access.stacktrace  # where the access happened\nspy_access.time  # when it happened (from time.time())\nspy_access.top_of_stacktrace  # a shorthand property intended to be used when debugging in the IDE\nspy_access.format_stacktrace()  # return a list of strings for the stacktrace\nspy_access.print_stacktrace()  # display the stacktrace to the console\n```\n\n\nPatching a class:\n\n```python\nmock_patch = MegaPatch.it(MyClass)\n\n# the class itself\nmock_patch.new_value\n\n# the class instance\nmock_patch.megainstance\n\n# the return value of the __call__ method on the class\nmock_patch.megainstance.return_value\n```\n\nPatching a class attribute:\n\n```python\n# temporarily update the max retries to 0\nmega_patch = MegaPatch.it(MyClass.max_retries, new=0)\n```\n\nPatching a class method:\n\n```python\nmega_patch = MegaPatch.it(MyClass.my_method, return_value=...)\n```\n\nAlternatively:\n```python\nmega_patch = MegaPatch.it(MyClass.my_method)\nmega_patch.mock.return_value = ...\n```\n\n```python\nmega_patch = MegaPatch.it(MyClass.my_method)\nmega_patch.new_value.return_value = ...\n```\n\nYou can also alter the return value of your mock without creating a separate mock object first.\n\n```python\nmega_patch.return_value.user = SomeUser()\n```\n\nWorking with `MegaPatch` and classes:\n\n`mega_patch.new_value` is the class _type_ itself\n\n```python\nmega_patch = MegaPatch.it(MyClass)\n\nmega_patch.new_value.x is MyClass.x\n```\n\n`mega_patch.return_value` is the class _instance_ returned. However, there is the property\n`megainstance` which is preferred because it has better type hinting.\n\n```python\nmega_patch = MegaPatch.it(MyClass)\n\n# instead of this, for which the static type is Any:\nmega_patch.return_value is MyClass()\n\n# use this, which has a static type of MegaMock | MyClass:\nmega_patch.megainstance is MyClass()\n```\n\nPatching a module attribute:\n\n```python\nimport my_module\n\nMegaPatch.it(my_module.some_attribute, new=...)\n```\n\nPatching a method of a nested class:\n\n```python\nimport my_module\n\nMegaPatch.it(\n    my_module.MyClass.MyNestedClass.some_method,\n    return_value=...\n)\n```\n\nSetting the return value:\n\n```python\nmy_mock.my_method.return_value = "foo"\n```\n\nTurning on real logic:\n\n```python\nimport my_module\nfrom mega_mock import UseRealLogic\n\nmega_patch = MegaPatch.it(my_module.SomeClass)\nMega(mega_patch.megainstance.some_pure_logic_method).use_real_logic()\n\ndo_something_that_invokes_that_function(...)\n```\n\n# Congrats on Reading This Far! Here\'s an Art Gallery!\n\n![MegaMock](docs/img/megamock-v2-cropped.png)\n\nNobody said it was a big art gallery. Feel free to submit a PR that helps fix that. No artistic skill required.\n',
     'author': 'James Hutchison',
     'author_email': 'jamesghutchison@proton.me',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/JamesHutchison/megamock',
```

### Comparing `megamock-0.1.0a8/PKG-INFO` & `megamock-0.1.0b1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: megamock
-Version: 0.1.0a8
+Version: 0.1.0b1
 Summary: Mega mocking capabilities - stop using dot-notated paths!
 Home-page: https://github.com/JamesHutchison/megamock
 License: MIT
 Keywords: mock,test
 Author: James Hutchison
 Author-email: jamesghutchison@proton.me
 Requires-Python: >=3.10,<4.0
```

