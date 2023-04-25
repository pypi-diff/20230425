# Comparing `tmp/reacton-1.6.0.tar.gz` & `tmp/reacton-1.6.1.tar.gz`

## Comparing `reacton-1.6.0.tar` & `reacton-1.6.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 reacton-1.6.0/react_ipywidgets/__init__.py
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 reacton-1.6.0/react_ipywidgets/core.py
--rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 reacton-1.6.0/reacton/__init__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 reacton-1.6.0/reacton/_version.py
--rw-r--r--   0        0        0   128540 2020-02-02 00:00:00.000000 reacton-1.6.0/reacton/bqplot.py
--rw-r--r--   0        0        0    95975 2020-02-02 00:00:00.000000 reacton-1.6.0/reacton/core.py
--rw-r--r--   0        0        0    88696 2020-02-02 00:00:00.000000 reacton-1.6.0/reacton/core_test.py
--rw-r--r--   0        0        0     9476 2020-02-02 00:00:00.000000 reacton-1.6.0/reacton/find.py
--rw-r--r--   0        0        0     5784 2020-02-02 00:00:00.000000 reacton-1.6.0/reacton/find_test.py
--rw-r--r--   0        0        0    13737 2020-02-02 00:00:00.000000 reacton-1.6.0/reacton/generate.py
--rw-r--r--   0        0        0     3277 2020-02-02 00:00:00.000000 reacton-1.6.0/reacton/generate_test.py
--rw-r--r--   0        0        0     9685 2020-02-02 00:00:00.000000 reacton-1.6.0/reacton/ipycanvas.py
--rw-r--r--   0        0        0     1404 2020-02-02 00:00:00.000000 reacton-1.6.0/reacton/ipyvue.py
--rw-r--r--   0        0        0   211230 2020-02-02 00:00:00.000000 reacton-1.6.0/reacton/ipyvuetify.py
--rw-r--r--   0        0        0   141249 2020-02-02 00:00:00.000000 reacton-1.6.0/reacton/ipywidgets.py
--rw-r--r--   0        0        0     2924 2020-02-02 00:00:00.000000 reacton-1.6.0/reacton/logging.py
--rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 reacton-1.6.0/reacton/patch.py
--rw-r--r--   0        0        0     2243 2020-02-02 00:00:00.000000 reacton-1.6.0/reacton/patch_display.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 reacton-1.6.0/reacton/py.typed
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 reacton-1.6.0/reacton/rx.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 reacton-1.6.0/reacton/test.vue
--rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 reacton-1.6.0/reacton/test_rx.py
--rw-r--r--   0        0        0     4943 2020-02-02 00:00:00.000000 reacton-1.6.0/reacton/utils.py
--rw-r--r--   0        0        0     2997 2020-02-02 00:00:00.000000 reacton-1.6.0/reacton/utils_test.py
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 reacton-1.6.0/reacton/work.py
--rw-r--r--   0        0        0      888 2020-02-02 00:00:00.000000 reacton-1.6.0/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 reacton-1.6.0/LICENSE
--rw-r--r--   0        0        0     1507 2020-02-02 00:00:00.000000 reacton-1.6.0/pyproject.toml
--rw-r--r--   0        0        0     2699 2020-02-02 00:00:00.000000 reacton-1.6.0/PKG-INFO
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 reacton-1.6.1/react_ipywidgets/__init__.py
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 reacton-1.6.1/react_ipywidgets/core.py
+-rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 reacton-1.6.1/reacton/__init__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 reacton-1.6.1/reacton/_version.py
+-rw-r--r--   0        0        0   128540 2020-02-02 00:00:00.000000 reacton-1.6.1/reacton/bqplot.py
+-rw-r--r--   0        0        0    96461 2020-02-02 00:00:00.000000 reacton-1.6.1/reacton/core.py
+-rw-r--r--   0        0        0    90141 2020-02-02 00:00:00.000000 reacton-1.6.1/reacton/core_test.py
+-rw-r--r--   0        0        0     9476 2020-02-02 00:00:00.000000 reacton-1.6.1/reacton/find.py
+-rw-r--r--   0        0        0     5784 2020-02-02 00:00:00.000000 reacton-1.6.1/reacton/find_test.py
+-rw-r--r--   0        0        0    13737 2020-02-02 00:00:00.000000 reacton-1.6.1/reacton/generate.py
+-rw-r--r--   0        0        0     3277 2020-02-02 00:00:00.000000 reacton-1.6.1/reacton/generate_test.py
+-rw-r--r--   0        0        0     9685 2020-02-02 00:00:00.000000 reacton-1.6.1/reacton/ipycanvas.py
+-rw-r--r--   0        0        0     1404 2020-02-02 00:00:00.000000 reacton-1.6.1/reacton/ipyvue.py
+-rw-r--r--   0        0        0   211230 2020-02-02 00:00:00.000000 reacton-1.6.1/reacton/ipyvuetify.py
+-rw-r--r--   0        0        0   141391 2020-02-02 00:00:00.000000 reacton-1.6.1/reacton/ipywidgets.py
+-rw-r--r--   0        0        0     2924 2020-02-02 00:00:00.000000 reacton-1.6.1/reacton/logging.py
+-rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 reacton-1.6.1/reacton/patch.py
+-rw-r--r--   0        0        0     2243 2020-02-02 00:00:00.000000 reacton-1.6.1/reacton/patch_display.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 reacton-1.6.1/reacton/py.typed
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 reacton-1.6.1/reacton/rx.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 reacton-1.6.1/reacton/test.vue
+-rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 reacton-1.6.1/reacton/test_rx.py
+-rw-r--r--   0        0        0     5314 2020-02-02 00:00:00.000000 reacton-1.6.1/reacton/utils.py
+-rw-r--r--   0        0        0     3704 2020-02-02 00:00:00.000000 reacton-1.6.1/reacton/utils_test.py
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 reacton-1.6.1/reacton/work.py
+-rw-r--r--   0        0        0      888 2020-02-02 00:00:00.000000 reacton-1.6.1/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 reacton-1.6.1/LICENSE
+-rw-r--r--   0        0        0     1507 2020-02-02 00:00:00.000000 reacton-1.6.1/pyproject.toml
+-rw-r--r--   0        0        0     2699 2020-02-02 00:00:00.000000 reacton-1.6.1/PKG-INFO
```

### Comparing `reacton-1.6.0/reacton/__init__.py` & `reacton-1.6.1/reacton/__init__.py`

 * *Files identical despite different names*

### Comparing `reacton-1.6.0/reacton/bqplot.py` & `reacton-1.6.1/reacton/bqplot.py`

 * *Files identical despite different names*

### Comparing `reacton-1.6.0/reacton/core.py` & `reacton-1.6.1/reacton/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -189,15 +189,15 @@
         pass
 
 
 class Element(Generic[W]):
     child_prop_name = "children"
     # to make every unique on_value callback to a unique wrapper
     # so that we can remove the listeners
-    _callback_wrappers: Dict[Callable, Callable] = {}
+    _callback_wrappers: Dict[Tuple[str, str, Callable], Callable] = {}
     create_lock: ContextManager = threading.Lock()
     _shared = False
 
     def __init__(self, component, args=None, kwargs=None):
         self.component = component
         self.mime_bundle = mime_bundle_default
         self._key: Optional[str] = None
@@ -415,25 +415,34 @@
 
         def on_change(change):
             if are_events_supressed():
                 return
             logger.info("event %r on %r with %r", name, widget, change)
             callback_exception_safe(change["new"])
 
-        self._callback_wrappers[callback] = on_change
+        key = (widget.model_id, name, callback)
+        self._callback_wrappers[key] = on_change
         widget.observe(on_change, target_name)
 
     def _remove_widget_event_listener(self, widget: widgets.Widget, name: str, callback: Callable):
         target_name = name[3:]
-        on_change = self._callback_wrappers[callback]
+        key = (widget.model_id, name, callback)
+        on_change = self._callback_wrappers[key]
+        del self._callback_wrappers[key]
         try:
             widget.unobserve(on_change, target_name)
         except ValueError:
             logger.error("Could not remove event listener %r from %r", name, widget)
 
+    def _cleanup_callbacks(self, widget: widgets.Widget):
+        args = self._get_widget_args()
+        for name, value in self.kwargs.items():
+            if name.startswith("on_") and name not in args and value is not None:
+                self._remove_widget_event_listener(widget, name, value)
+
 
 class Value(Generic[V], Protocol):
     def get(self) -> V:
         ...
 
     def set(self, value: V):
         ...
@@ -2054,14 +2063,15 @@
 
             for orphan in self._orphans.get(widget.model_id, set()):
                 orphan_widget = widgets.Widget.widgets.get(orphan)
                 if orphan_widget:
                     close(orphan_widget)
             if widget.model_id in self._orphans:
                 del self._orphans[widget.model_id]
+            el._cleanup_callbacks(widget)
             close(widget)
         if el.is_shared:
             del self._shared_widgets[el]
         else:
             del context.widgets[key]
         # elements can be removed multiple times, since they can be added multiple times
         # (even non-shared element can)
```

### Comparing `reacton-1.6.0/reacton/core_test.py` & `reacton-1.6.1/reacton/core_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,15 +102,15 @@
     before = set(widgets.Widget.widgets)
     yield
     after = set(widgets.Widget.widgets)
     leftover = after - before
     if leftover:
         leftover_widgets = [widgets.Widget.widgets[k] for k in leftover]
         assert not leftover_widgets
-        # raise RuntimeError(f"{leftover_widgets}")
+    assert reacton.core.Element._callback_wrappers == {}
 
 
 @pytest.fixture(params=["ButtonComponentWidget", "ButtonComponentFunction"])
 def ButtonComponent(request):
     return dict(ButtonComponentWidget=w.Button, ButtonComponentFunction=ButtonComponentFunction)[request.param]
 
 
@@ -1985,16 +1985,20 @@
         nonlocal set_value
         value, set_value = react.use_state(0)
         return w.IntSlider(value=value)
 
     slider, rc = react.render_fixed(Test())
     assert set_value is not None
     state = rc.state_get()
+    if "auto_subscribe_force_update_counter" in state["children"]["/"]["state"]:
+        del state["children"]["/"]["state"]["auto_subscribe_force_update_counter"]
     assert state == {"children": {"/": {"state": {"0": 0}}}, "state": {}}
     set_value(42)
+    if "auto_subscribe_force_update_counter" in state["children"]["/"]["state"]:
+        del state["children"]["/"]["state"]["auto_subscribe_force_update_counter"]
     assert state == {"children": {"/": {"state": {"0": 42}}}, "state": {}}
     assert slider.value == 42
     rc.close()
 
     box = widgets.VBox()
     hbox, rc = react.render(Test(), box, initial_state=state, handle_error=False)
     assert box.children[0].value == 42
@@ -3045,7 +3049,43 @@
     box, rc = react.render(Test(), handle_error=False)
     assert rc.find(widgets.Button).widget.description == "0"
     assert rc.render_count == 1
     set_state(1)
     assert rc.render_count == 2
     assert rc.find(widgets.Button).widget.description == "3"
     rc.close()
+
+
+def test_event_multiple():
+    @reacton.component
+    def Test():
+        count, set_count = reacton.use_state(0)
+
+        def add():
+            set_count(count + 1)
+
+        def remove():
+            set_count(count - 1)
+
+        with w.VBox() as main:
+            for i in range(count):
+                w.Button(description=str(i), on_click=remove)
+            w.Button(description="Add", on_click=add)
+        return main
+
+    box, rc = react.render(Test(), handle_error=False)
+    rc.find(widgets.Button, description="Add").widget.click()
+    rc.find(widgets.Button, description="0").assert_single()
+    assert len(rc.find(widgets.Button)) == 2
+
+    rc.find(widgets.Button, description="Add").widget.click()
+    rc.find(widgets.Button, description="1").assert_single()
+    assert len(rc.find(widgets.Button)) == 3
+
+    rc.find(widgets.Button, description="Add").widget.click()
+    rc.find(widgets.Button, description="2").assert_single()
+    assert len(rc.find(widgets.Button)) == 4
+
+    rc.find(widgets.Button, description="2").widget.click()
+    assert len(rc.find(widgets.Button)) == 3
+
+    rc.close()
```

### Comparing `reacton-1.6.0/reacton/find.py` & `reacton-1.6.1/reacton/find.py`

 * *Files identical despite different names*

### Comparing `reacton-1.6.0/reacton/find_test.py` & `reacton-1.6.1/reacton/find_test.py`

 * *Files identical despite different names*

### Comparing `reacton-1.6.0/reacton/generate.py` & `reacton-1.6.1/reacton/generate.py`

 * *Files identical despite different names*

### Comparing `reacton-1.6.0/reacton/generate_test.py` & `reacton-1.6.1/reacton/generate_test.py`

 * *Files identical despite different names*

### Comparing `reacton-1.6.0/reacton/ipycanvas.py` & `reacton-1.6.1/reacton/ipycanvas.py`

 * *Files identical despite different names*

### Comparing `reacton-1.6.0/reacton/ipyvue.py` & `reacton-1.6.1/reacton/ipyvue.py`

 * *Files identical despite different names*

### Comparing `reacton-1.6.0/reacton/ipyvuetify.py` & `reacton-1.6.1/reacton/ipyvuetify.py`

 * *Files identical despite different names*

### Comparing `reacton-1.6.0/reacton/ipywidgets.py` & `reacton-1.6.1/reacton/ipywidgets.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,27 +91,30 @@
     def _add_widget_event_listener(self, widget: widgets.Widget, name: str, callback: Callable):
         if name == "on_click":
             callback_exception_safe = _event_handler_exception_wrapper(callback)
 
             def on_click(change):
                 callback_exception_safe()
 
-            self._callback_wrappers[callback] = on_click
+            key = (widget.model_id, name, callback)
+            self._callback_wrappers[key] = on_click
             widget.on_click(on_click)
 
         else:
             super()._add_widget_event_listener(widget, name, callback)
 
     def _remove_widget_event_listener(self, widget: widgets.Widget, name: str, callback: Callable):
         if name == "on_click":
-            on_click = self._callback_wrappers[callback]
+            key = (widget.model_id, name, callback)
+            on_click = self._callback_wrappers[key]
+            del self._callback_wrappers[key]
             widget.on_click(on_click, remove=True)
 
         else:
-            super()._add_widget_event_listener(widget, name, callback)
+            super()._remove_widget_event_listener(widget, name, callback)
 
 
 if __name__ == "__main__":
     from . import generate
 
     class CodeGen(generate.CodeGen):
         element_classes = {ipywidgets.Button: ButtonElement}
```

### Comparing `reacton-1.6.0/reacton/logging.py` & `reacton-1.6.1/reacton/logging.py`

 * *Files identical despite different names*

### Comparing `reacton-1.6.0/reacton/patch.py` & `reacton-1.6.1/reacton/patch.py`

 * *Files identical despite different names*

### Comparing `reacton-1.6.0/reacton/patch_display.py` & `reacton-1.6.1/reacton/patch_display.py`

 * *Files identical despite different names*

### Comparing `reacton-1.6.0/reacton/test_rx.py` & `reacton-1.6.1/reacton/test_rx.py`

 * *Files identical despite different names*

### Comparing `reacton-1.6.0/reacton/utils.py` & `reacton-1.6.1/reacton/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,19 +44,27 @@
     if type(a) != type(b):  # is this always true? after a == b failed?
         return False
     if isinstance(a, Element):
         return same_component(a.component, b.component) and equals(a.args, b.args) and equals(a.kwargs, b.kwargs)
     elif isinstance(a, types.FunctionType) and isinstance(b, types.FunctionType):
         if a.__code__ != b.__code__:
             return False
+        if not equals(a.__defaults__, b.__defaults__):
+            return False
+        if not equals(a.__kwdefaults__, b.__kwdefaults__):
+            return False
+        # comparing the closure is tricky, because the cells are not comparable
         if a.__closure__ is None and b.__closure__ is None:
+            # easy case, both have no closure
             return True
         elif a.__closure__ is None or b.__closure__ is None:
+            # one has a closure, the other not
             return False
         else:
+            # both have a closure
             for cell_a, cell_b in zip(a.__closure__, b.__closure__):
                 if not (equals(cell_a, cell_b) or equals(cell_a.cell_contents, cell_b.cell_contents)):
                     return False
         return True
     elif isinstance(a, dict) and isinstance(b, dict):
         if len(a) != len(b):
             return False
```

### Comparing `reacton-1.6.0/reacton/utils_test.py` & `reacton-1.6.1/reacton/utils_test.py`

 * *Files 20% similar despite different names*

```diff
@@ -80,14 +80,44 @@
     f3 = make_function_empty_cell(2, ar2, ar2)
     assert f1 == f1
     assert f1 != f2
     assert equals(f1, f1)
     assert equals(f1, f2)
     assert not equals(f1, f3)
 
+    def make_function_default_arg(a):
+        def func(x, c=a):
+            return x + c
+
+        return func
+
+    f1 = make_function_default_arg(1)
+    f2 = make_function_default_arg(1)
+    f3 = make_function_default_arg(2)
+    assert f1 == f1
+    assert f1 != f2
+    assert equals(f1, f1)
+    assert equals(f1, f2)
+    assert not equals(f1, f3)
+
+    def make_function_default_kwarg(a):
+        def func(x, *, c=a):
+            return x + c
+
+        return func
+
+    f1 = make_function_default_kwarg(1)
+    f2 = make_function_default_kwarg(1)
+    f3 = make_function_default_kwarg(2)
+    assert f1 == f1
+    assert f1 != f2
+    assert equals(f1, f1)
+    assert equals(f1, f2)
+    assert not equals(f1, f3)
+
     def make_el(a):
         def on_click():
             pass
 
         return w.Button(on_click=on_click, label=f"{a}")
 
     el1 = make_el(1)
```

### Comparing `reacton-1.6.0/.gitignore` & `reacton-1.6.1/.gitignore`

 * *Files identical despite different names*

### Comparing `reacton-1.6.0/LICENSE` & `reacton-1.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `reacton-1.6.0/pyproject.toml` & `reacton-1.6.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `reacton-1.6.0/PKG-INFO` & `reacton-1.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reacton
-Version: 1.6.0
+Version: 1.6.1
 Project-URL: Home, https://www.github.com/widgetti/reacton
 Project-URL: Documentation, https://reacton.solara.dev
 Project-URL: Source code, https://www.github.com/widgetti/reacton
 Author-email: "Maarten A. Breddels" <maartenbreddels@gmail.com>
 License: The MIT License (MIT)
         
         Copyright (c) 2022 Maarten A. Breddels
```

