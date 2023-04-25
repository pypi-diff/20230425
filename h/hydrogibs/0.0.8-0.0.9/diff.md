# Comparing `tmp/hydrogibs-0.0.8.tar.gz` & `tmp/hydrogibs-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hydrogibs-0.0.8.tar", last modified: Tue Apr 25 01:48:01 2023, max compression
+gzip compressed data, was "hydrogibs-0.0.9.tar", last modified: Tue Apr 25 11:11:36 2023, max compression
```

## Comparing `hydrogibs-0.0.8.tar` & `hydrogibs-0.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 axel      (1000) axel      (1000)        0 2023-04-25 01:48:01.397836 hydrogibs-0.0.8/
--rw-rw-r--   0 axel      (1000) axel      (1000)     1073 2023-04-23 13:58:07.000000 hydrogibs-0.0.8/LICENSE
--rw-rw-r--   0 axel      (1000) axel      (1000)      541 2023-04-25 01:48:01.397836 hydrogibs-0.0.8/PKG-INFO
--rw-rw-r--   0 axel      (1000) axel      (1000)       37 2023-04-23 13:57:53.000000 hydrogibs-0.0.8/README.md
-drwxrwxr-x   0 axel      (1000) axel      (1000)        0 2023-04-25 01:48:01.393835 hydrogibs-0.0.8/hydrogibs/
--rw-rw-r--   0 axel      (1000) axel      (1000)    20256 2023-04-25 01:45:58.000000 hydrogibs-0.0.8/hydrogibs/GR4.py
--rw-rw-r--   0 axel      (1000) axel      (1000)      120 2023-04-25 01:47:38.000000 hydrogibs-0.0.8/hydrogibs/__init_.py
--rw-rw-r--   0 axel      (1000) axel      (1000)     9213 2023-04-24 14:45:59.000000 hydrogibs-0.0.8/hydrogibs/misc.py
-drwxrwxr-x   0 axel      (1000) axel      (1000)        0 2023-04-25 01:48:01.397836 hydrogibs-0.0.8/hydrogibs.egg-info/
--rw-rw-r--   0 axel      (1000) axel      (1000)      541 2023-04-25 01:48:01.000000 hydrogibs-0.0.8/hydrogibs.egg-info/PKG-INFO
--rw-rw-r--   0 axel      (1000) axel      (1000)      220 2023-04-25 01:48:01.000000 hydrogibs-0.0.8/hydrogibs.egg-info/SOURCES.txt
--rw-rw-r--   0 axel      (1000) axel      (1000)        1 2023-04-25 01:48:01.000000 hydrogibs-0.0.8/hydrogibs.egg-info/dependency_links.txt
--rw-rw-r--   0 axel      (1000) axel      (1000)       10 2023-04-25 01:48:01.000000 hydrogibs-0.0.8/hydrogibs.egg-info/top_level.txt
--rw-rw-r--   0 axel      (1000) axel      (1000)      489 2023-04-25 01:47:43.000000 hydrogibs-0.0.8/pyproject.toml
--rw-rw-r--   0 axel      (1000) axel      (1000)       38 2023-04-25 01:48:01.397836 hydrogibs-0.0.8/setup.cfg
+drwxrwxr-x   0 axel      (1000) axel      (1000)        0 2023-04-25 11:11:36.575677 hydrogibs-0.0.9/
+-rw-rw-r--   0 axel      (1000) axel      (1000)     1073 2023-04-23 13:58:07.000000 hydrogibs-0.0.9/LICENSE
+-rw-rw-r--   0 axel      (1000) axel      (1000)      541 2023-04-25 11:11:36.571677 hydrogibs-0.0.9/PKG-INFO
+-rw-rw-r--   0 axel      (1000) axel      (1000)       37 2023-04-23 13:57:53.000000 hydrogibs-0.0.9/README.md
+drwxrwxr-x   0 axel      (1000) axel      (1000)        0 2023-04-25 11:11:36.571677 hydrogibs-0.0.9/hydrogibs/
+-rw-rw-r--   0 axel      (1000) axel      (1000)    21448 2023-04-25 11:06:59.000000 hydrogibs-0.0.9/hydrogibs/GR4.py
+-rw-rw-r--   0 axel      (1000) axel      (1000)      120 2023-04-25 01:47:38.000000 hydrogibs-0.0.9/hydrogibs/__init_.py
+-rw-rw-r--   0 axel      (1000) axel      (1000)     9213 2023-04-24 14:45:59.000000 hydrogibs-0.0.9/hydrogibs/misc.py
+drwxrwxr-x   0 axel      (1000) axel      (1000)        0 2023-04-25 11:11:36.571677 hydrogibs-0.0.9/hydrogibs.egg-info/
+-rw-rw-r--   0 axel      (1000) axel      (1000)      541 2023-04-25 11:11:36.000000 hydrogibs-0.0.9/hydrogibs.egg-info/PKG-INFO
+-rw-rw-r--   0 axel      (1000) axel      (1000)      220 2023-04-25 11:11:36.000000 hydrogibs-0.0.9/hydrogibs.egg-info/SOURCES.txt
+-rw-rw-r--   0 axel      (1000) axel      (1000)        1 2023-04-25 11:11:36.000000 hydrogibs-0.0.9/hydrogibs.egg-info/dependency_links.txt
+-rw-rw-r--   0 axel      (1000) axel      (1000)       10 2023-04-25 11:11:36.000000 hydrogibs-0.0.9/hydrogibs.egg-info/top_level.txt
+-rw-rw-r--   0 axel      (1000) axel      (1000)      489 2023-04-25 11:10:05.000000 hydrogibs-0.0.9/pyproject.toml
+-rw-rw-r--   0 axel      (1000) axel      (1000)       38 2023-04-25 11:11:36.575677 hydrogibs-0.0.9/setup.cfg
```

### Comparing `hydrogibs-0.0.8/LICENSE` & `hydrogibs-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `hydrogibs-0.0.8/PKG-INFO` & `hydrogibs-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hydrogibs
-Version: 0.0.8
+Version: 0.0.9
 Summary: A small hydrology package
 Author-email: axel Giboulot <axel.giboulot@epfl.ch>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `hydrogibs-0.0.8/hydrogibs/GR4.py` & `hydrogibs-0.0.9/hydrogibs/GR4.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,45 +8,51 @@
 from collections import namedtuple
 
 
 def _transfer_func(n: float, X4: float):  # m/km/s
     """
     This function will make the transition between the
     water flow and the discharge through a convolution
+
+    discharge = convolution(_transfer_func(water_flow, time/X4))
     """
     if n < 1:
         return 3/(2*X4) * n**2
     if n < 2:
         return 3/(2*X4) * (2-n)**2
     return 0
 
 
 class Rain:
 
+    """
+    Rain object to apply to a catchment
+    """
+
     def __init__(self, time: np.ndarray, rain_func: Callable) -> None:
 
         self.time = time
         self.rain_func = rain_func
         self.rainfall = np.array([rain_func(t) for t in time])
         self.timestep = time[1] - time[0]
 
     def __matmul__(self, catchment):
-        return GR4h(catchment, self).compute()
+        return GR4h(catchment, self).apply()
 
 
 class BlockRain:
     """
     A constant rain with a limited duration.
 
     Args:
         - intensity        (floaat)[mm/h]
         - duration         (float) [h]
         - timestep         (float) [h]: directly linked to precision
         - observation_span (float) [h]: the duration of the experiment
-    
+
     Can create a GR4h object when calles with a Catchment object:
     >>> gr4h = rain @ catchment
     >>> gr4h = GR4h(catchment, rain)
     """
 
     def __init__(self,
                  intensity: float,
@@ -80,19 +86,19 @@
     Stores GR4h catchment parameters.
 
     Returns a GR4h object when called with a Rain object:
         >>> catchment = Catchment(X1=8/100, X2=40, X3=0.1, X4=1)
         >>> rain = BlockRain(intensity=50)
         >>> gr4: GR4h = catchment @ rain  # first syntax
         >>> gr4: GR4h = GR4h(catchment, rain)  # second syntax
-    
+
     Args:
         X1 (float)  [-] : dQ = X1 * dPrecipitations
         X2 (float)  [mm]: Initial abstraction (vegetation interception)
-        X3 (float) [1/h]: Sub-surface water volume emptying rate dSs = X3 * V*dt
+        X3 (float) [1/h]: Sub-surface water volume emptying rate dQs = X3*V*dt
         X4 (float)  [h] : the hydrogram's raising time
     """
 
     def __init__(self,
                  X1: float,
                  X2: float,
                  X3: float,
@@ -115,93 +121,60 @@
         assert 0 <= X4, "Raising time must be positive"
 
     def __matmul__(self, rain):
         return GR4h(self, rain)
 
 
 Event = namedtuple("Event",
-                   ("volume",
+                   ("time",
+                    "rainfall",
+                    "volume",
                     "water_flow_rain",
                     "water_flow_volume",
                     "water_flow",
                     "discharge_rain",
                     "discharge_volume",
                     "discharge")
                    )
 
 
-class GR4h:
-    """
-    Object storing a Catchment object, a Rain object, and Event object
-    and eventually attributes relative to a diagram
-
-    A GR4h object is obtained when called with a Rain and a Catchment objects:
-        >>> catchment = Catchment(X1=8/100, X2=40, X3=0.1, X4=1)
-        >>> rain = BlockRain(intensity=50)
-        >>> gr4: GR4h = catchment @ rain  # first syntax
-        >>> gr4: GR4h = GR4h(catchment, rain)  # second syntax
-        >>> gr4.App()  # opens an interactive diagram in a tkinter window
-    
-    Args:
-        catchment (Catchment): contains essential parameters
-        rain      (Rain): contains the rainfall event details
-    
-    Returns:
-        gr4h (GR4h): Object contaning an Event object (discharges, water flow)
-        gr4h.event (Event): Contains the following arrays:
-                                - volume
-                                - water_flow
-                                - discharge
-                            The corresponding time is stored in gr4h.rain.time
-    """
-
-    def __init__(self, catchment: Catchment, rain: Rain) -> None:
-
-        self.catchment = catchment
-        self.rain = rain
+class GR4diagram:
 
-        if isinstance(self.rain, BlockRain):
-            self.compute = self.compute_block
-        else:
-            self.compute = self.compute_rain
-
-    def compute_block(self):
-
-        self.event = gr4_block_rain(self.catchment, self.rain)
-
-        return self
-
-    def compute_rain(self):
+    def __init__(self,
+                 event: Event,
+                 style: str = "ggplot",
+                 colors=("teal",
+                         "k",
+                         "indigo",
+                         "tomato",
+                         "green"),
+                 flows_margin=0.3,
+                 rain_margin=7,
+                 show=True) -> None:
+
+        self.style = style
+        self.colors = colors
+        self.flows_margin = flows_margin
+        self.rain_margin = rain_margin
 
-        self.event = gr4_diff(self.catchment, self.rain)
+        self.draw(event, show=show)
 
-        return self
-
-    def diagram(self, show=True, style: str = "ggplot",
-                colors=("teal", "k", "indigo", "tomato", "green"), k=1.3, kr=8):
+    def draw(self, event: Event, show=True):
         """Plots a diagram with rainfall, water flow and discharge"""
-        self.k = k
-        self.kr = kr
-
-        time = self.rain.time
-        rain = self.rain.rainfall
 
-        event = self.event
-        V = event.volume
-        dTp = event.water_flow_rain
-        dTv = event.water_flow_volume
+        time = event.time
+        rain = event.rainfall
+        dT = event.water_flow
         Qp = event.discharge_rain
         Qv = event.discharge_volume
+        Q = event.discharge
 
-        dT = dTp + dTv
-        Q = Qp + Qv
+        with plt.style.context(self.style):
 
-        with plt.style.context(style):
-
-            c1, c2, c3, c4, c5 = colors
+            c1, c2, c3, c4, c5 = self.colors
 
             fig, ax1 = plt.subplots(figsize=(7, 3.5), dpi=100)
             ax1.set_title("Runoff response to rainfall")
 
             patch = ax1.fill_between(
                 x=time,
                 y1=Q,
@@ -226,57 +199,183 @@
                 lw=0.0,
                 color=c5,
                 label="Sub-surface discharge"
             )
             ax1.set_ylabel("$Q$ (m³/s)", color=c1)
             ax1.set_xlabel("Time [h]")
             ax1.set_xlim((time.min(), time.max()))
-            ax1.set_ylim((0, k*Q.max()))
+            ax1.set_ylim((0, (1 + self.flows_margin)*Q.max()))
             yticks = ax1.get_yticks()
-            yticks = [y for y in yticks if y < max(yticks)/k]
+            yticks = [
+                y for y in yticks
+                if y < max(yticks)/(self.flows_margin + 1)
+            ]
             ax1.set_yticks(yticks)
             ax1.set_yticklabels(yticks, color=c1)
 
             ax2 = ax1.twinx()
             bars = ax2.bar(
                 time,
                 rain,
                 alpha=0.5,
                 width=time[1]-time[0],
                 color=c2,
                 label="Rainfall"
             )
             max_rain = rain.max()
-            ax2.set_ylim((self.kr*max_rain, 0))
+            ax2.set_ylim(((1 + self.rain_margin) * max_rain, 0))
             ax2.grid(False)
             ax2.set_yticks((0, max_rain))
             ax2.set_yticklabels(ax2.get_yticklabels(), color=c2)
 
             ax3 = ax2.twinx()
             line, = ax3.plot(time, dT, "-.",
                              color=c3, label="Water flow", lw=1.5)
             ax3.set_ylabel("$\\dot{T}$ (mm/h)", color=c3)
             ax3.set_xlabel("$t$ (h)")
-            ax3.set_ylim((0, k*dT.max()))
+            ax3.set_ylim((0, (1 + self.flows_margin) * dT.max()))
             yticks = ax3.get_yticks()
-            yticks = [y for y in yticks if y < max(yticks)/k]
+            yticks = [
+                y for y in yticks
+                if y < max(yticks)/(1 + self.flows_margin)
+            ]
             ax3.set_yticks(yticks)
             ax3.set_yticklabels(ax3.get_yticks(), color=c3)
             ax3.grid(False)
 
             lines = (bars, patch, patch1, patch2, line)
             labs = [line.get_label() for line in lines]
             ax1.legend(lines, labs)
 
             plt.tight_layout()
+
+            self.fig, self.axes, self.lines = fig, (ax1, ax2, ax3), lines
+
             if show:
                 plt.show()
+        return self
+
+    def update(self, event, rain_obj):
+
+        t = event.time
+        rain, discharge, discharge_p, discharge_v, water_flow = self.lines
+
+        discharge.set_verts((
+            list(zip(  # transposing data
+                np.concatenate((t, t[::-1])),
+                np.concatenate((
+                    event.discharge,
+                    np.maximum(
+                        event.discharge_rain,
+                        event.discharge_volume)[::-1]
+                ))
+            )),
+        ))
+        discharge_p.set_verts((
+            list(zip(t, event.discharge_rain)) + [(t[-1], 0)],
+        ))
+        discharge_v.set_verts((
+            list(zip(t, event.discharge_volume)) + [(t[-1], 0)],
+        ))
+        water_flow.set_data(t, event.water_flow)
+
+        if isinstance(rain_obj, BlockRain):
+            I0 = rain_obj.intensity
+            d = rain_obj.duration
+            for rect, v in zip(rain, t):
+                if v <= d:
+                    rect.set_height(I0)
+                else:
+                    rect.set_height(0)
+
+    def zoom(self, canvas):
+
+        rain, discharge, _, _, water_flow = self.lines
+        ax1, ax2, ax3 = self.axes
+
+        t, Q = discharge.get_paths()[0].vertices.T
+        Qm = Q.max()
+        Imax = max([b.get_height() for b in rain])
+        _, dT = water_flow.get_data()
+        dTm = dT.max()
+
+        ylim = Qm * (1 + self.flows_margin)
+        ax1.set_ylim((0, ylim if ylim else 1))
+        ax1.set_xlim((0, t.max()))
+        yticks = np.linspace(0, Qm, 7)
+        ax1.set_yticks(yticks)
+        ax1.set_yticklabels([f"{tick:.2}" for tick in yticks])
+
+        ylim = Imax * (1 + self.rain_margin)
+        ax2.set_ylim((ylim if ylim else 1, 0))
+        ax2.set_yticks((0, Imax))
+        ax2.set_yticklabels((0, f"{Imax:.1f}"))
+
+        ylim = dTm * (1 + self.flows_margin)
+        ax3.set_ylim((0, ylim if ylim else 1))
+        yticks = np.linspace(0, dTm, 7)
+        ax3.set_yticks(yticks)
+        ax3.set_yticklabels([f"{tick:.2}" for tick in yticks])
+
+        plt.tight_layout()
+        canvas.draw()
+
+
+class GR4h:
+    """
+    Object storing a Catchment object, a Rain object, and Event object
+    and eventually attributes relative to a diagram
+
+    A GR4h object is obtained when called with a Rain and a Catchment objects:
+        >>> catchment = Catchment(X1=8/100, X2=40, X3=0.1, X4=1)
+        >>> rain = BlockRain(intensity=50)
+        >>> gr4: GR4h = catchment @ rain  # first syntax
+        >>> gr4: GR4h = GR4h(catchment, rain)  # second syntax
+        >>> gr4.App()  # opens an interactive diagram in a tkinter window
+
+    Args:
+        catchment (Catchment): contains essential parameters
+        rain      (Rain): contains the rainfall event details
+
+    Returns:
+        gr4h (GR4h): Object contaning an Event object (discharges, water flow)
+        gr4h.event (Event): Contains the following arrays:
+                                - volume
+                                - water_flow
+                                - discharge
+                            The corresponding time is stored in gr4h.rain.time
+    """
+
+    def __init__(self, catchment: Catchment, rain: Rain) -> None:
+
+        self.catchment = catchment
+        self.rain = rain
+
+        if isinstance(self.rain, BlockRain):
+            self.apply = self.apply_block_rain
+        else:
+            self.apply = self.apply_rain
+
+        self.apply()
+
+    def apply_block_rain(self):
 
-        if not show:
-            return fig, (ax1, ax2, ax3), lines
+        self.event = gr4_block_rain(self.catchment, self.rain)
+
+        return self
+
+    def apply_rain(self):
+
+        self.event = gr4_diff(self.catchment, self.rain)
+
+        return self
+
+    def create_diagram(self, *args, **kwargs):
+
+        self.diagram = GR4diagram(self.event, *args, **kwargs)
 
     def App(self):
         GR4App(self)
 
 
 def gr4_diff(catchment, rain):
 
@@ -294,16 +393,18 @@
     i = time[np.cumsum(dP)*dt >= X2 - V0]
     t1 = i[0] if i.size else float("inf")
 
     dP_effective = dP.copy()
     dP_effective[time < t1] = 0
 
     # solution to the differential equation V' = -X3*V + (1-X1)*P
-    V = np.exp(-X3*time) * (1-X1) * \
+    V = (
+        np.exp(-X3*time) * (1-X1) *
         np.cumsum(np.exp(X3*time) * dP_effective) * dt
+    )
     V = V + V0 * np.exp(-X3*time)
 
     t_abstraction = time < t1
     dTp = X1*dP
     dTp[t_abstraction] = 0
     dTv = X3*V
     dTv[t_abstraction] = 0
@@ -312,15 +413,15 @@
         catchment.transfer_function(ni, X4)
         for ni in time[time <= 2*X4]/X4
     ])
 
     Qp = S * np.convolve(dTp, q)[:time.size] * dt
     Qv = S * np.convolve(dTv, q)[:time.size] * dt
 
-    return Event(V, dTp, dTv, dTp+dTv, Qp, Qv, Qp+Qv)
+    return Event(time, dP, V, dTp, dTv, dTp+dTv, Qp, Qv, Qp+Qv)
 
 
 def gr4_block_rain(catchment, block_rain) -> dict:
     """
     This method is fit for block events
     (constant rainfall intensity during a defined duration)
 
@@ -361,14 +462,15 @@
 
     # Unpack rain attributes
     dt = block_rain.timestep
     t0 = block_rain.duration
     tf = block_rain.observation_span
 
     I0 = block_rain.intensity
+    rainfall = block_rain.rainfall
 
     # Initializing time
     tf = 10*t0 if tf is None else tf
     t = np.arange(start=0, stop=tf, step=dt)
 
     # End of abstraction
     t1 = X2/I0
@@ -404,15 +506,15 @@
         transfer_function(ni, X4)
         for ni in t[t <= 2*X4]/X4
     ])
     # Convolve
     Qp = S * np.convolve(dTp, q)[:t.size] * dt
     Qv = S * np.convolve(dTv, q)[:t.size] * dt
 
-    return Event(V, dTp, dTv, dTp+dTv, Qp, Qv, Qp+Qv)
+    return Event(t, rainfall, V, dTp, dTv, dTp+dTv, Qp, Qv, Qp+Qv)
 
 
 class GR4App:
 
     def __init__(self, gr4: GR4h,
                  appearance: str = "dark",
                  color_theme: str = "dark-blue"):
@@ -427,15 +529,16 @@
         self.root.bind('<Return>', self.entries_update)
         # self.ww = self.root.winfo_screenwidth()
         # self.wh = self.root.winfo_screenheight()
         # self.root.geometry(f"{self.ww*0.8:.0f}x{self.wh*0.5:.0f}")
 
         self.dframe = ctk.CTkFrame(master=self.root)
         self.dframe.grid(row=0, column=1, sticky="NSEW")
-        self.draw_diagram()
+
+        self.init_diagram()
 
         self.pframe = ctk.CTkFrame(master=self.root)
         self.pframe.grid(column=0, row=0, sticky="NSEW")
 
         # entryframe = ctk.CTkLabel(text="GR4 parameters",
         #                           master=self.pframe,
         #                           font=("monospace", 24))
@@ -446,49 +549,45 @@
         self.entries = dict()
         self.define_entry("X1", "-")
         self.define_entry("X2", "mm")
         self.define_entry("X3", "1/h")
         self.define_entry("X4", "h")
         self.define_entry("surface", "km²", "S")
         self.define_entry("initial_volume", "mm", "V0")
-        self.define_entry("observation_span", "mm", "tf")
+
         if isinstance(self.gr4.rain, BlockRain):
+            self.define_entry("observation_span", "mm", "tf")
             self.define_entry("intensity", "mm/h", "I0")
             self.define_entry("duration", "h", "t0")
 
         ctk.CTkButton(master=self.pframe,
                       text="Reset zoom",
-                      command=self.zoom).grid(pady=10)
+                      command=lambda: self.diagram.zoom(self.canvas)
+                      ).grid(pady=10)
 
         self.root.mainloop()
 
-    def zoom(self):
+    def init_diagram(self):
 
-        t, Q = self.disch.get_paths()[0].vertices.T
-        Qm = Q.max()
-        Imax = max([b.get_height() for b in self.rain])
-        _, dT = self.wflow.get_data()
-        dTm = dT.max()
+        diagram = GR4diagram(self.gr4.event, show=False)
 
-        self.ax1.set_ylim((0, Qm * self.gr4.k))
-        self.ax1.set_xlim((0, t.max()))
-        yticks = np.linspace(0, Qm, 7)
-        self.ax1.set_yticks(yticks)
-        self.ax1.set_yticklabels([f"{tick:.3}" for tick in yticks])
-
-        self.ax2.set_ylim((Imax * self.gr4.kr, 0))
-        self.ax2.set_yticks((0, Imax))
-        self.ax2.set_yticklabels((0, f"{Imax:.1f}"))
-        self.ax3.set_ylim((0, dTm * self.gr4.k))
-        yticks = np.linspace(0, dTm, 7)
-        self.ax3.set_yticks(yticks)
-        self.ax3.set_yticklabels([f"{tick:.3}" for tick in yticks])
+        self.ax1, self.ax2, self.ax3 = diagram.axes
 
-        plt.tight_layout()
+        self.canvas = FigureCanvasTkAgg(diagram.fig, master=self.dframe)
+        toolbar = NavigationToolbar2Tk(self.canvas)
+        toolbar.update()
+        self.canvas._tkcanvas.pack()
         self.canvas.draw()
+        self.canvas.get_tk_widget().pack()
+        self.canvas.mpl_connect('key_press_event',
+                                lambda arg: key_press_handler(
+                                    arg, self.canvas, toolbar
+                                ))
+        self.diagram = diagram
+        self.root.update()
 
     def define_entry(self, key: str, unit, alias: str = None):
 
         entryframe = ctk.CTkFrame(master=self.pframe)
         entryframe.grid(sticky="NSEW")
         unit_str = f"[{unit}]"
         name = key if alias is None else alias
@@ -571,78 +670,27 @@
                 elif hasattr(self.gr4.rain, key):
                     setattr(self.gr4.rain, key, v)
                 else:
                     raise KeyError(f"{key} not an attribute")
 
         self.update()
 
-    def draw_diagram(self):
-
-        self.fig, axes, lines = self.gr4.diagram(show=False)
-        self.ax1, self.ax2, self.ax3 = axes
-        self.rain, self.disch, self.dischp, self.dischv, self.wflow = lines
-
-        self.canvas = FigureCanvasTkAgg(self.fig, master=self.dframe)
-        toolbar = NavigationToolbar2Tk(self.canvas)
-        toolbar.update()
-        self.canvas._tkcanvas.pack()
-        self.canvas.draw()
-        self.canvas.get_tk_widget().pack()
-        self.canvas.mpl_connect('key_press_event',
-                                lambda arg: key_press_handler(
-                                    arg, self.canvas, toolbar
-                                ))
-        self.root.update()
-
     def update(self):
 
-        self.gr4.compute()
-        t = self.gr4.rain.time
-
-        event = self.gr4.event
-
-        self.disch.set_verts((
-            list(zip(  # transposing data
-                np.concatenate((t, t[::-1])),
-                np.concatenate((
-                    event.discharge,
-                    np.maximum(
-                        event.discharge_rain,
-                        event.discharge_volume)[::-1]
-                ))
-            )),
-        ))
-        self.dischp.set_verts((
-            list(zip(t, event.discharge_rain)) + [(t[-1], 0)],
-        ))
-        self.dischv.set_verts((
-            list(zip(t, event.discharge_volume)) + [(t[-1], 0)],
-        ))
-        self.wflow.set_data(t, event.water_flow)
-
-        rain = self.gr4.rain
-        if isinstance(rain, BlockRain):
-            I0 = rain.intensity
-            d = rain.duration
-            for rect, v in zip(self.rain, t):
-                if v <= d:
-                    rect.set_height(I0)
-                else:
-                    rect.set_height(0)
-
+        self.gr4.apply()
+        self.diagram.update(self.gr4.event, self.gr4.rain)
         self.canvas.draw()
-        # self.root.update()
 
 
 def GR4_demo():
-    time = np.linspace(0, 10, 1000)
+    # time = np.linspace(0, 10, 1000)
     # gr4 = Catchment(8/100, 40, 0.1, 1, initial_volume=30) @ Rain(
     #     time,
     #     rain_func=lambda t: 50 if t < 2 else 0
     # )
     gr4 = Catchment(8/100, 40, 0.1, 1) @ BlockRain(50, duration=1.8)
-    gr4 = gr4.compute()
+    gr4 = gr4.apply()
     gr4.App()
 
 
 if __name__ == "__main__":
     GR4_demo()
```

### Comparing `hydrogibs-0.0.8/hydrogibs/misc.py` & `hydrogibs-0.0.9/hydrogibs/misc.py`

 * *Files identical despite different names*

### Comparing `hydrogibs-0.0.8/hydrogibs.egg-info/PKG-INFO` & `hydrogibs-0.0.9/hydrogibs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hydrogibs
-Version: 0.0.8
+Version: 0.0.9
 Summary: A small hydrology package
 Author-email: axel Giboulot <axel.giboulot@epfl.ch>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

