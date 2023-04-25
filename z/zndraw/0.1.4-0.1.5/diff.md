# Comparing `tmp/zndraw-0.1.4.tar.gz` & `tmp/zndraw-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zndraw-0.1.4.tar", max compression
+gzip compressed data, was "zndraw-0.1.5.tar", max compression
```

## Comparing `zndraw-0.1.4.tar` & `zndraw-0.1.5.tar`

### file list

```diff
@@ -1,18 +1,20 @@
--rw-r--r--   0        0        0    13576 2023-04-12 16:10:14.508402 zndraw-0.1.4/LICENSE
--rw-r--r--   0        0        0     2020 2023-04-24 08:50:45.092660 zndraw-0.1.4/README.md
--rw-r--r--   0        0        0      797 2023-04-24 08:51:03.752461 zndraw-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      166 2023-04-21 17:52:18.309756 zndraw-0.1.4/zndraw/__init__.py
--rw-r--r--   0        0        0     3976 2023-04-24 08:50:45.102660 zndraw-0.1.4/zndraw/app.py
--rw-r--r--   0        0        0     1659 2023-04-23 21:22:34.280010 zndraw-0.1.4/zndraw/cli.py
--rw-r--r--   0        0        0     2695 2023-04-24 08:50:45.102660 zndraw-0.1.4/zndraw/examples/__init__.py
--rw-r--r--   0        0        0     4278 2023-04-24 08:50:45.102660 zndraw-0.1.4/zndraw/globals.py
--rw-r--r--   0        0        0     1208 2023-04-22 20:55:05.579300 zndraw-0.1.4/zndraw/io.py
--rw-r--r--   0        0        0      880 2023-04-21 17:52:18.319756 zndraw-0.1.4/zndraw/main.py
--rw-r--r--   0        0        0     9533 2023-04-17 10:14:40.724969 zndraw-0.1.4/zndraw/static/favion-192x192.png
--rw-r--r--   0        0        0     3521 2023-04-23 21:22:34.290009 zndraw-0.1.4/zndraw/static/main.css
--rw-r--r--   0        0        0    21070 2023-04-24 08:50:45.112660 zndraw-0.1.4/zndraw/static/main.js
--rw-r--r--   0        0        0     2893 2023-04-24 08:50:45.112660 zndraw-0.1.4/zndraw/static/modules/draw.js
--rw-r--r--   0        0        0      854 2023-04-24 06:27:16.592781 zndraw-0.1.4/zndraw/static/modules/keypress.js
--rw-r--r--   0        0        0    10032 2023-04-24 08:50:45.112660 zndraw-0.1.4/zndraw/static/modules/particles.js
--rw-r--r--   0        0        0    16455 2023-04-24 08:50:45.112660 zndraw-0.1.4/zndraw/templates/index.html
--rw-r--r--   0        0        0     2912 1970-01-01 00:00:00.000000 zndraw-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0    13576 2023-04-12 16:10:14.508402 zndraw-0.1.5/LICENSE
+-rw-r--r--   0        0        0     2020 2023-04-24 08:50:45.092660 zndraw-0.1.5/README.md
+-rw-r--r--   0        0        0      834 2023-04-25 07:53:59.807276 zndraw-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      166 2023-04-21 17:52:18.309756 zndraw-0.1.5/zndraw/__init__.py
+-rw-r--r--   0        0        0     1139 2023-04-25 07:53:59.817276 zndraw-0.1.5/zndraw/analyse.py
+-rw-r--r--   0        0        0     4682 2023-04-25 09:20:10.132886 zndraw-0.1.5/zndraw/app.py
+-rw-r--r--   0        0        0     1659 2023-04-23 21:22:34.280010 zndraw-0.1.5/zndraw/cli.py
+-rw-r--r--   0        0        0     2695 2023-04-24 08:50:45.102660 zndraw-0.1.5/zndraw/examples/__init__.py
+-rw-r--r--   0        0        0     4278 2023-04-24 08:50:45.102660 zndraw-0.1.5/zndraw/globals.py
+-rw-r--r--   0        0        0     1208 2023-04-22 20:55:05.579300 zndraw-0.1.5/zndraw/io.py
+-rw-r--r--   0        0        0      880 2023-04-21 17:52:18.319756 zndraw-0.1.5/zndraw/main.py
+-rw-r--r--   0        0        0     9533 2023-04-17 10:14:40.724969 zndraw-0.1.5/zndraw/static/favion-192x192.png
+-rw-r--r--   0        0        0     3521 2023-04-23 21:22:34.290009 zndraw-0.1.5/zndraw/static/main.css
+-rw-r--r--   0        0        0    20035 2023-04-25 09:20:10.132886 zndraw-0.1.5/zndraw/static/main.js
+-rw-r--r--   0        0        0     2633 2023-04-25 09:20:10.132886 zndraw-0.1.5/zndraw/static/modules/data.js
+-rw-r--r--   0        0        0     2893 2023-04-24 08:50:45.112660 zndraw-0.1.5/zndraw/static/modules/draw.js
+-rw-r--r--   0        0        0     1009 2023-04-24 16:48:30.446942 zndraw-0.1.5/zndraw/static/modules/keypress.js
+-rw-r--r--   0        0        0    11582 2023-04-25 09:20:10.132886 zndraw-0.1.5/zndraw/static/modules/particles.js
+-rw-r--r--   0        0        0    15833 2023-04-25 09:20:10.142886 zndraw-0.1.5/zndraw/templates/index.html
+-rw-r--r--   0        0        0     2991 1970-01-01 00:00:00.000000 zndraw-0.1.5/PKG-INFO
```

### Comparing `zndraw-0.1.4/LICENSE` & `zndraw-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.4/README.md` & `zndraw-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.4/pyproject.toml` & `zndraw-0.1.5/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "zndraw"
-version = "0.1.4"
+version = "0.1.5"
 description = ""
 authors = ["zincwarecode <zincwarecode@gmail.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
@@ -12,14 +12,16 @@
 networkx = "^3.1"
 typer = {extras = ["all"], version = "^0.7.0"}
 flask = "^2.2.3"
 tqdm = "^4.65.0"
 pywebview = {version = "^4.0.2", optional = true}
 znh5md = "^0.1.6"
 pydantic = "^1.10.7"
+plotly = "^5.14.1"
+pandas = "^2.0.1"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 ruff = "^0.0.261"
 pytest = "^7.3.0"
 
 [build-system]
```

### Comparing `zndraw-0.1.4/zndraw/app.py` & `zndraw-0.1.5/zndraw/app.py`

 * *Files 12% similar despite different names*

```diff
@@ -35,27 +35,34 @@
     step = request.json
     try:
         atoms = globals.config.get_atoms(step=int(step))
         graph = io.get_graph(atoms)
         return {
             "nodes": [{**graph.nodes[idx], "id": idx} for idx in graph.nodes],
             "edges": list(graph.edges),
+            "box": atoms.get_cell().diagonal().tolist(),
         }
     except KeyError:
         return {}
 
 
-@app.route("/positions", methods=["POST"])
+@app.route("/data", methods=["POST"])
 def positions_step():
     params = request.json
-    result = []
+    result = {"position": [], "force": [], "box": []}
     try:
         for step in range(params["start"], params["stop"]):
             atoms = globals.config.get_atoms(step=int(step))
-            result.append(atoms.get_positions().tolist())
+            result["position"].append(atoms.get_positions().tolist())
+            result["box"].append(atoms.get_cell().diagonal().tolist())
+            # TODO MAKE THIS OPTIONAL!!, also energy, etc.
+            # try:
+            #     result["force"].append(atoms.get_forces().tolist())
+            # except:
+            #     result["force"].append(np.zeros_like(atoms.get_positions()).tolist())
         return result
     except KeyError:
         return result
 
 
 @app.route("/select", methods=["POST"])
 def select() -> list[int]:
@@ -123,12 +130,22 @@
     selected_ids = list(sorted(request.json["selected_ids"]))
     step = request.json["step"]
     points = np.array([[x["x"], x["y"], x["z"]] for x in request.json["points"]])
     globals.config.apply_update_function(selected_ids, step, points=points)
     return {}
 
 
+@app.route("/analyse", methods=["POST"])
+def analyse():
+    selected_ids = list(sorted(request.json["selected_ids"]))
+    step = request.json["step"]
+    from zndraw.analyse import get_distance_plot
+
+    fig = get_distance_plot(step, selected_ids)
+    return fig.to_json()
+
+
 @app.route("/load")
 def load():
     """Function to call asynchronously to load atoms in the background."""
     globals.config.load_atoms()
     return {}
```

### Comparing `zndraw-0.1.4/zndraw/cli.py` & `zndraw-0.1.5/zndraw/cli.py`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.4/zndraw/examples/__init__.py` & `zndraw-0.1.5/zndraw/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.4/zndraw/globals.py` & `zndraw-0.1.5/zndraw/globals.py`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.4/zndraw/io.py` & `zndraw-0.1.5/zndraw/io.py`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.4/zndraw/main.py` & `zndraw-0.1.5/zndraw/main.py`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.4/zndraw/static/favion-192x192.png` & `zndraw-0.1.5/zndraw/static/favion-192x192.png`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.4/zndraw/static/main.css` & `zndraw-0.1.5/zndraw/static/main.css`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.4/zndraw/static/main.js` & `zndraw-0.1.5/zndraw/static/main.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -1,38 +1,27 @@
 import * as THREE from 'three';
 import {
     OrbitControls
 } from 'three/addons/controls/OrbitControls.js';
 import * as PARTICLES from './modules/particles.js';
 import * as DRAW from './modules/draw.js';
+import * as DATA from './modules/data.js';
 import {
-    keydown
+    keydown,
+    keyconfig
 } from './modules/keypress.js';
 // THREE.Cache.enabled = true;
 
 
-/**
- * Three JS Setup
- */
-
-/**
- * ThreeJS variables
- */
-
-let config = {};
-
-
 // some global variables
-let frames = [];
 let selected_ids = [];
 let animation_frame = 0;
 let displayed_frame = 0;
 let scene_building = false;
 let animation_running = true;
-let data_loading = false;
 let fps = [];
 
 
 /**
  * DOM variables
  */
 
@@ -47,112 +36,88 @@
 const div_n_bonds = document.getElementById('n_bonds');
 
 const o_autoRestart = document.getElementById('autoRestart');
 const o_animate = document.getElementById('animate');
 const o_reset_selection = document.getElementById('reset_selection');
 const o_reset = document.getElementById('reset');
 const o_max_fps = document.getElementById('max_fps');
-const o_frames_per_post = document.getElementById('frames_per_post');
 const o_materialSelect = document.getElementById('materialSelect');
 const o_wireframe = document.getElementById('wireframe');
 const o_spotLightIntensity = document.getElementById('spotLightIntensity');
 const o_hemisphereLightIntensity = document.getElementById('hemisphereLightIntensity');
 
 const addModifierModal = new bootstrap.Modal(document.getElementById("addModifierModal"));
 const addSceneModifier = document.getElementById("addSceneModifier");
 
 
 // Helper Functions
 
-async function load_config() {
-    config = await (await fetch("config")).json();
-    console.log(config)
-}
-await load_config();
-
+await DATA.load_config();
 // THREE JS Setup
 const scene = new THREE.Scene();
 const camera = new THREE.PerspectiveCamera(75, window.innerWidth / window.innerHeight, 0.1, 1000);
 const renderer = new THREE.WebGLRenderer({
-    antialias: config["antialias"],
+    antialias: DATA.config["antialias"],
     alpha: true
 });
 
 const hemisphereLight = new THREE.HemisphereLight(0xffffff, 0x777777, 0.1);
-const spotLight = new THREE.SpotLight(0xffffff, 1, 0, Math.PI / 2);
+const spotLight = new THREE.SpotLight(0xffffff, 0, 0, Math.PI / 2);
+const cameraLight = new THREE.PointLight(0xffffff, 1.0);
+
+camera.add(cameraLight);
 
 renderer.setSize(window.innerWidth, window.innerHeight);
 document.body.appendChild(renderer.domElement);
 
 
 spotLight.position.set(0, 0, 100);
 scene.add(spotLight);
+scene.add(camera); // add the camera to the scene because of the cameraLight
 
 scene.add(hemisphereLight);
 
 async function update_materials() {
     for (const material in PARTICLES.materials) {
         const option = document.createElement("option");
         option.text = material;
         option.value = material;
         o_materialSelect.appendChild(option);
     }
-    o_materialSelect.value = config["material"];
+    o_materialSelect.value = DATA.config["material"];
 }
 
 update_materials();
 
 
 
 // Setup Scene
 
-let build_scene_cache = {};
 
 async function build_scene(step) {
     if (scene_building) {
         return;
     }
     console.log("Updating scene");
 
     div_loading.style.visibility = 'visible';
     div_greyOut.style.visibility = 'visible';
 
     animation_frame = step;
 
-    let arrayOfResponses = [];
-    if (build_scene_cache.hasOwnProperty(step)) {
-        console.log("Using cached scene");
-        arrayOfResponses = build_scene_cache[step];
-    } else {
-        // this is faster then doing it one by one
-
-        arrayOfResponses = await (await fetch("graph", {
-            "method": "POST",
-            "headers": {
-                "Content-Type": "application/json"
-            },
-            "body": JSON.stringify(step)
-        })).json();
-        console.log(arrayOfResponses);
-        build_scene_cache[step] = arrayOfResponses;
-    }
-
-    config = await (await fetch("config")).json();
-
-    PARTICLES.drawAtoms(arrayOfResponses["nodes"], arrayOfResponses["edges"], config, scene);
-    selected_ids = [];
-    await update_selection();
-    scene_building = false;
-
-    div_n_particles.innerHTML = PARTICLES.particleGroup.children.length;
-
-    div_n_bonds.innerHTML = PARTICLES.countBonds();
-
-    div_greyOut.style.visibility = 'hidden';
-    div_loading.style.visibility = 'hidden';
+    await DATA.getRebuildCache(step).then(function(arrayOfResponses) {
+        PARTICLES.drawAtoms(arrayOfResponses["nodes"], arrayOfResponses["edges"], DATA.config, scene);
+        selected_ids = [];
+    }).then(update_selection).then(function() {
+        scene_building = false;
+        div_n_particles.innerHTML = PARTICLES.particleGroup.children.length;
+        div_n_bonds.innerHTML = PARTICLES.countBonds();
+        div_greyOut.style.visibility = 'hidden';
+        div_loading.style.visibility = 'hidden';
+    });
 }
 
 build_scene(0);
 
 // interactions
 
 camera.position.z = 50;
@@ -188,15 +153,15 @@
 
     if (intersects.length == 0) {
         return;
     }
 
     // for (let i = 0; i < intersects.length; i++) {
     let mesh = intersects[0].object;
-    if (!keydown["shift"]) {
+    if (!keydown["shift"] && !keyconfig.multiselect) {
         if (selected_ids.includes(mesh.userData["id"])) {
             selected_ids = [];
         } else {
             selected_ids = [mesh.userData["id"]];
         }
     } else {
         if (!selected_ids.includes(mesh.userData["id"])) {
@@ -254,60 +219,20 @@
             selected_ids = response_json["selected_ids"];
         }
         div_lst_selected_ids.innerHTML = response_json["selected_ids"].join(", ");
     });
 
 }
 
-async function getAnimationFrames() {
-    if (data_loading) {
-        console.log("Animation read already in progress");
-        return;
-    }
-    console.log("Loading animation frames");
-
-    data_loading = true;
-    if (frames.length < 2) {
-        fetch("load");
-    }
-
-    let step = frames.length;
-    while (true) {
-
-        let obj = await fetch("positions", {
-            "method": "POST",
-            "headers": {
-                "Content-Type": "application/json"
-            },
-            "body": JSON.stringify({
-                "start": step,
-                "stop": parseInt(o_frames_per_post.value) + step
-            }),
-        }).then(response => response.json()).then(function(response_json) {
-            load_config();
-            return response_json;
-        });
-
-        console.log("Read " + step + "-" + (parseInt(o_frames_per_post.value) + step) + " frames");
-        if (Object.keys(obj).length === 0) {
-            console.log("Animation read finished");
-            break;
-        }
-        frames = frames.concat(obj);
-        step += parseInt(o_frames_per_post.value);
-    }
-    data_loading = false;
-}
-
 
-if (config["animate"] === true) {
+if (DATA.config["animate"] === true) {
     div_info.innerHTML = "Reading file...";
-    getAnimationFrames();
+    DATA.getAnimationFrames();
 }
-if (config["restart_animation"] === true) {
+if (DATA.config["restart_animation"] === true) {
     o_autoRestart.checked = true;
 }
 
 /**
  * Event listeners
  */
 
@@ -323,27 +248,27 @@
         window.addEventListener('pointerdown', onPointerDown, false);
     }
 
 }
 
 o_animate.onclick = function() {
     div_info.innerHTML = "Reading file...";
-    getAnimationFrames();
+    DATA.getAnimationFrames();
 }
 
 
 o_reset_selection.onclick = function() {
     selected_ids = [];
     update_color_of_ids(selected_ids);
     update_selection();
 }
 
 
 o_reset.onclick = function() {
-    load_config();
+    DATA.load_config();
     animation_frame = 0;
     build_scene(0);
     selected_ids = [];
     update_selection();
 }
 
 document.getElementById("sphereRadius").onchange = function() {
@@ -422,103 +347,77 @@
 
 o_hemisphereLightIntensity.oninput = function() {
     hemisphereLight.intensity = o_hemisphereLightIntensity.value;
     document.getElementById("hemisphereLightIntensityLabel").innerHTML = "Hemisphere light intensity: " + o_hemisphereLightIntensity.value;
 
 }
 
+document.getElementById("cameraLightIntensity").oninput = function() {
+    let intensity = parseFloat(document.getElementById("cameraLightIntensity").value);
+    cameraLight.intensity = intensity;
+    document.getElementById("cameraLightIntensityLabel").innerHTML = "Camera light intensity: " + intensity;
+}
+
 
 /**
  * Helper function, move later
  * @param {} name 
  * @param {*} checked 
  * @returns 
  */
 function createRadioElement(id, properties) {
 
-    var radioFragment = document.createElement('div');
-    radioFragment.classList.add("mb-3");
-    radioFragment.classList.add("collapse", "show", "scene-modifier");
-    radioFragment.id = "sceneModifier_" + id;
-
-    let function_container = document.createElement('div');
-    function_container.classList.add("container-fluid", "bg-light", "rounded", "border", "border-primary");
-
-    let function_container_label = document.createElement('h5');
-    function_container_label.innerHTML = id;
-
-    function_container.appendChild(function_container_label);
-
-    let function_container_col = document.createElement('div');
-    function_container_col.classList.add("row");
-
-    let descriptions = document.createElement('div');
-    descriptions.classList.add("col-sm-2");
-
-    let values = document.createElement('div');
-    values.classList.add("col-sm-1");
-
-    let controllers = document.createElement('div');
-    controllers.classList.add("col-sm-8");
-
-    function_container_col.appendChild(descriptions);
-    function_container_col.appendChild(values);
-    function_container_col.appendChild(controllers);
+    let modifierCanvas = document.createElement('div');
+    // modifierCanvas.classList.add("mb-3");
+    modifierCanvas.classList.add("collapse", "show", "scene-modifier", "border", "border-primary", "rounded", "p-3");
+    modifierCanvas.id = "sceneModifier_" + id;
 
     console.log(properties);
 
     Object.values(properties).forEach((item) => {
-        console.log(item);
-        let label = document.createElement('div');
-        label.innerHTML = item["title"];
-        let label_row = document.createElement('div');
-        label_row.classList.add("row-sm");
-        label_row.appendChild(label);
-
-        let value = document.createElement('div');
-        value.innerHTML = item["default"];
-        let value_row = document.createElement('div');
-        value_row.classList.add("row-sm");
-        value_row.appendChild(value);
-
-        descriptions.appendChild(label_row);
-        values.appendChild(value_row);
-
         let controller = document.createElement('input');
         if (item["type"] == "integer") {
             controller.type = "range";
+            controller.classList.add("form-range");
             controller.step = 1;
         } else if (item["type"] == "number") {
             controller.type = "range";
+            controller.classList.add("form-range");
             controller.step = 0.1;
         } else if (item["type"] == "text") {
             controller.type = "text";
+            controller.classList.add("form-control");
         } else {
             console.log("Unknown type: " + item["type"]);
         }
         controller.value = item["default"];
         controller.id = id + "_" + item["title"];
 
         if ("minimum" in item) {
             controller.min = item["minimum"];
         }
         if ("maximum" in item) {
             controller.max = item["maximum"];
         }
 
-        let controller_row = document.createElement('div');
-        controller_row.classList.add("row-sm");
-        controller_row.appendChild(controller);
+        let controller_label = document.createElement('label');
+        controller_label.classList.add("form-label");
+        controller_label.setAttribute("for", controller.id);
+        controller_label.innerHTML = item["title"] + ": " + controller.value;
+
+        let function_container = document.createElement('div');
+        // function_container.classList.add("mb-1");
+        function_container.appendChild(controller_label);
+        function_container.appendChild(controller);
 
-        controllers.appendChild(controller_row);
+        modifierCanvas.appendChild(function_container);
 
         controller.oninput = function() {
-            value.innerHTML = controller.value;
+            controller_label.innerHTML = item["title"] + ": " + controller.value;
         }
-
         controller.onchange = function() {
             // fetch with post 
             fetch("set_update_function_parameter", {
                 "method": "POST",
                 "headers": {
                     "Content-Type": "application/json"
                 },
@@ -526,18 +425,16 @@
                     "function_id": id,
                     "property": item["title"],
                     "value": controller.value
                 })
             });
         }
     });
-    function_container.appendChild(function_container_col);
-    radioFragment.appendChild(function_container);
 
-    return radioFragment;
+    return modifierCanvas;
 }
 
 addSceneModifier.onchange = function() {
     console.log(this.value);
     if (this.value == "add") {
         addModifierModal.show();
     } else {
@@ -577,15 +474,15 @@
                 alert("Function already loaded");
                 stepError("Function already loaded");
             };
 
             addModifierModal.hide();
 
             console.log(response_json);
-            load_config();
+            DATA.load_config();
         }
         return response_json;
     }).then(function(response_json) {
         console.log(response_json);
         let modifier = document.createElement("option");
         modifier.value = response_json["title"];
         modifier.innerHTML = response_json["title"];
@@ -601,51 +498,53 @@
 }
 
 
 
 window.addEventListener("keydown", (event) => {
     if (event.isComposing || event.key === " ") {
         event.preventDefault();
-        if (animation_running && animation_frame == frames.length - 1) {
+        if (animation_running && animation_frame == DATA.frames.length - 1) {
             animation_frame = 0;
         } else {
             animation_running = !animation_running;
         }
     }
     if (event.isComposing || event.key === "ArrowLeft") {
         event.preventDefault();
         animation_frame = Math.max(0, animation_frame - 1);
     }
     if (event.isComposing || event.key === "ArrowRight") {
         event.preventDefault();
-        animation_frame = Math.min(frames.length - 1, animation_frame + 1);
+        animation_frame = Math.min(DATA.frames.length - 1, animation_frame + 1);
     }
     if (event.isComposing || event.key === "ArrowUp") {
-        animation_frame = parseInt(Math.min(frames.length - 1, animation_frame + (frames.length / 10)));
+        animation_frame = parseInt(Math.min(DATA.frames.length - 1, animation_frame + (DATA.frames.length / 10)));
     }
     if (event.isComposing || event.key === "ArrowDown") {
-        animation_frame = parseInt(Math.max(0, animation_frame - (frames.length / 10)));
+        animation_frame = parseInt(Math.max(0, animation_frame - (DATA.frames.length / 10)));
     }
     if (event.isComposing || event.key === "q") {
-        getAnimationFrames();
+        DATA.getAnimationFrames();
     }
     if (event.isComposing || event.key === "i") {
         PARTICLES.printIndices(camera);
     };
 });
 
+
 window.addEventListener("keyup", (event) => {
     if (event.isComposing || event.key === "i") {
         let ids = document.getElementsByClassName("particle-id")
         while (ids.length > 0) {
             ids[0].parentNode.removeChild(ids[0]);
         }
     }
 });
 
+
 window.addEventListener("keydown", (event) => {
     if (event.isComposing || event.key === "Enter") {
         div_info.innerHTML = "Processing...";
 
         fetch("update", {
             "method": "POST",
             "headers": {
@@ -653,18 +552,18 @@
             },
             "body": JSON.stringify({
                 "selected_ids": selected_ids,
                 "step": animation_frame,
                 "points": DRAW.positions
             }),
         }).then((response) => {
-            if (frames.length > 0) {
-                frames.length = animation_frame + 1;
+            if (DATA.frames.length > 0) {
+                DATA.spliceFrames(animation_frame + 1);
             }
-            getAnimationFrames();
+            DATA.getAnimationFrames();
         });
     }
 });
 
 // Drawing
 
 DRAW.init(camera, renderer, scene, controls)
@@ -676,70 +575,96 @@
     DRAW.createAnchorPoint(position);
 };
 
 document.getElementById("drawRemoveLine").onclick = function() {
     DRAW.reset();
 };
 
+document.getElementById("analyseDistanceBtn").onclick = function() {
+    fetch("analyse", {
+        "method": "POST",
+        "headers": {
+            "Content-Type": "application/json"
+        },
+        "body": JSON.stringify({
+            "selected_ids": selected_ids,
+            "step": animation_frame,
+            "points": DRAW.positions
+        }),
+    }).then((response) => response.json()).then(function(response_json) {
+        Plotly.newPlot('analysePlot', response_json);
+    });
+};
 
+document.getElementById("showBox").onclick = function() {
+    if (this.checked) {
+        scene.add(PARTICLES.createBox(DATA.frames.box[animation_frame]));
+    } else {
+        scene.remove(PARTICLES.box);
+    }
+};
 
 
 let move_atoms_clock = new THREE.Clock();
 
 
 function move_atoms() {
-    if (frames.length === 0) {
+    if (DATA.frames.length === 0) {
         return;
     }
     if (move_atoms_clock.getElapsedTime() < (1 / o_max_fps.value)) {
         return;
     }
     if (scene_building === true) {
         return;
     }
     div_progressBar.style.visibility = "hidden";
 
     if (animation_running === true) {
-        if (animation_frame < frames.length - 1) {
+        if (animation_frame < DATA.frames.length - 1) {
             animation_frame += 1;
         } else if (o_autoRestart.checked === true) {
             animation_frame = 0;
         }
     }
-    if (frames.length < animation_frame) {
+    if (DATA.frames.length < animation_frame) {
         // waiting for async call to finish
         return;
     }
-    if (config["total_frames"] > 0) {
+    if (DATA.config["total_frames"] > 0) {
         div_progressBar.style.visibility = "visible";
-        div_progressBar.style.width = ((animation_frame / config["total_frames"]) * 100).toFixed(2) + "%";
-        div_bufferBar.style.width = (((frames.length - 1) / config["total_frames"]) * 100).toFixed(2) + "%";
+        div_progressBar.style.width = ((animation_frame / DATA.config["total_frames"]) * 100).toFixed(2) + "%";
+        div_bufferBar.style.width = (((DATA.frames.length - 1) / DATA.config["total_frames"]) * 100).toFixed(2) + "%";
     }
-    if (frames[animation_frame].length != PARTICLES.particleGroup.children.length) {
+    if (DATA.frames.position[animation_frame].length != PARTICLES.particleGroup.children.length) {
         // we need to update the scene
         build_scene(animation_frame);
         scene_building = true;
         return; // we need to wait for the scene to be updated
     }
 
-    div_info.innerHTML = "Frame (" + animation_frame + "/" + (frames.length - 1) + ")";
+    div_info.innerHTML = "Frame (" + animation_frame + "/" + (DATA.frames.length - 1) + ")";
 
     if (animation_frame != displayed_frame) {
         displayed_frame = animation_frame;
-        PARTICLES.updateParticlePositions(frames[animation_frame]);
+        PARTICLES.updateParticlePositions(DATA.frames.position[animation_frame]);
+        // if (PARTICLES.boxGeometry !== undefined) {
+        // 	PARTICLES.updateBox(DATA.frames.box[animation_frame]);
+        // }
+        // PARTICLES.updateArrows(DATA.frames.force[animation_frame]);
     }
 
     fps.push(move_atoms_clock.getElapsedTime());
 
     if (fps.length > 10) {
         fps.shift();
     }
-    if (!data_loading) {
-        getAnimationFrames();
-    }
+    // if (!data_loading) {
+    // 	DATA.getAnimationFrames();
+    // }
 
     div_FPS.innerHTML = (1 / (fps.reduce((a, b) => a + b, 0) / fps.length)).toFixed(2);
     move_atoms_clock.start();
 }
 
 function centerCamera() {
     if (selected_ids.length === 0) {
@@ -750,21 +675,21 @@
 }
 
 /**
  * Dynamic indices
  * 
  */
 
-
+// scene.add(PARTICLES.arrowGroup);
 function animate() {
 
     renderer.render(scene, camera);
     controls.update();
 
-    if (frames.length > 0) {
+    if (DATA.frames.length > 0) {
         move_atoms();
     }
     if (keydown["c"]) {
         centerCamera();
     }
     if (keydown["l"]) {
         spotLight.position.x = camera.position.x;
```

### Comparing `zndraw-0.1.4/zndraw/static/modules/draw.js` & `zndraw-0.1.5/zndraw/static/modules/draw.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.4/zndraw/static/modules/keypress.js` & `zndraw-0.1.5/zndraw/static/modules/keypress.js`

 * *Files 12% similar despite different names*

#### js-beautify {}

```diff
@@ -1,14 +1,17 @@
 export const keydown = {
     "shift": false,
     "ctrl": false,
     "alt": false,
     "c": false,
     "l": false
 };
+export const keyconfig = {
+    "multiselect": false
+}
 
 
 
 window.addEventListener("keyup", (event) => {
     if (event.isComposing || !event.shiftKey) {
         keydown["shift"] = false;
     }
@@ -36,8 +39,12 @@
         keydown["alt"] = true;
     }
     for (let key in keydown) {
         if (event.isComposing || event.key === key) {
             keydown[key] = true;
         }
     }
-});
+});
+
+document.getElementById("multiselect").onchange = function() {
+    keyconfig.multiselect = this.checked;
+}
```

### Comparing `zndraw-0.1.4/zndraw/static/modules/particles.js` & `zndraw-0.1.5/zndraw/static/modules/particles.js`

 * *Files 11% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,12 @@
 import * as THREE from 'three';
 
 // each entry in the particleGroup again is a group of [particle, bond1, bond2, bond3, ...]
 export const particleGroup = new THREE.Group();
+export const arrowGroup = new THREE.Group();
 
 
 export const materials = {
     "MeshBasicMaterial": new THREE.MeshBasicMaterial({
         color: "#ffa500"
     }),
     "MeshLambertMaterial": new THREE.MeshLambertMaterial({
@@ -27,14 +28,16 @@
         color: "#ffa500"
     }),
 
 };
 
 let node1 = new THREE.Vector3();
 let node2 = new THREE.Vector3();
+export let box;
+export let boxGeometry;
 
 const direction = new THREE.Vector3();
 
 let sphereGeometryFactoryCache = {};
 let speciesMaterialFactoryCache = {};
 let halfCylinderGeometryFactoryCache = {};
 
@@ -211,36 +214,42 @@
     }
     center.divideScalar(count);
     return center;
 }
 
 // TODO rename clean AtomsBonds
 // this does not remove the scene!
+// TODO add setup function that loads the scene inside this module
 export function cleanScene(scene) {
     speciesMaterialFactoryCache = {};
     sphereGeometryFactoryCache = {};
     halfCylinderGeometryFactoryCache = {};
 
     while (particleGroup.children.length > 0) {
         scene.remove(particleGroup.children.shift());
     };
+
+    while (arrowGroup.children.length > 0) {
+        scene.remove(arrowGroup.children.shift());
+    };
 }
 
 export function drawAtoms(atoms, bonds, config, scene) {
     cleanScene(scene);
 
     atoms.forEach((item) => {
         addAtom(item, config)
     });
 
     if (config["bond_size"] > 0) {
         bonds.forEach((item) => {
             addBond(item, config)
         });
     }
+    createArrowPerParticle();
     scene.add(particleGroup);
 }
 
 
 /**
  * Update the positions of the particles
  * @param {Float32List} positions as (n_particles, 3)
@@ -322,8 +331,47 @@
         text2.style.fontSize = Math.max(15, parseInt(50 - 0.3 * (distances[index] * Math.max(...distances)))) + 'px';
         text2.style.backgroundColor = "#cccccc";
         text2.innerHTML = item[1];
         text2.style.top = item[0].y + 'px';
         text2.style.left = item[0].x + 'px';
         document.body.appendChild(text2);
     });
+}
+
+/**
+ * Draw an arrow on each particle with the given direction / magnitude
+ * @param {THREE.Vector3} vectors 
+ */
+export async function updateArrows(vectors) {
+
+    arrowGroup.children.forEach((item, index) => {
+        const vector = new THREE.Vector3(...vectors[index]);
+        item.setDirection(vector.clone().normalize());
+        item.setLength(vector.length()); // find a good factor here
+        item.position.copy(getAtomById(index).position);
+    });
+}
+
+export function createArrowPerParticle() {
+    particleGroup.children.forEach(function(atoms_grp) {
+        let item = atoms_grp.children[0];
+        let arrow = new THREE.ArrowHelper(new THREE.Vector3(1, 0, 0), item.position, 0, 0xff0000);
+        arrowGroup.add(arrow);
+    });
+    return arrowGroup;
+}
+
+export function createBox(size) {
+    const geometry = new THREE.BoxGeometry(1, 1, 1);
+    geometry.applyMatrix4(new THREE.Matrix4().makeTranslation(1 / 2, 1 / 2, 1 / 2));
+    boxGeometry = new THREE.EdgesGeometry(geometry);
+    const material = new THREE.LineBasicMaterial({
+        color: 0x000000
+    });
+    box = new THREE.LineSegments(boxGeometry, material);
+    boxGeometry.scale(...size);
+    return box;
+}
+
+export function updateBox(size) {
+    console.log("update box not implemented yet")
 }
```

### Comparing `zndraw-0.1.4/zndraw/templates/index.html` & `zndraw-0.1.5/zndraw/templates/index.html`

 * *Files 6% similar despite different names*

```diff
@@ -15,14 +15,17 @@
     "imports": {
       "three": "https://unpkg.com/three@0.151.3/build/three.module.js",
       "three/addons/": "https://unpkg.com/three@0.151.3/examples/jsm/",
       "./modules/": "{{ url_for('static', filename='/modules/') }}"
     }
   }
 </script>
+  <script src="https://cdnjs.cloudflare.com/ajax/libs/plotly.js/2.21.0/plotly.min.js"
+    integrity="sha512-oalOW03buJpcBKtaooDOM2XrfQXI4ifCNBaFgYfY6UCQBGCFPsiwsrQVdAnENOJwjwEwLiVAgy3Ljyt7cN2LJw=="
+    crossorigin="anonymous" referrerpolicy="no-referrer"></script>
 </head>
 
 <body>
   <script type="module" src="{{ url_for('static', filename='main.js') }}"></script>
 
   <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0-alpha3/dist/js/bootstrap.bundle.min.js"
     integrity="sha384-ENjdO4Dr2bkBIFxQpeoTz1HIcje39Wm4jDKdf19U8gI4ddQ3GYNS7NTKfAdVQSZe"
@@ -77,14 +80,20 @@
           </li>
           <li class="nav-item mx-1">
             <button class="btn btn-outline-secondary" type="button" data-bs-toggle="offcanvas"
               data-bs-target="#drawCanvas" aria-controls="drawCanvas">
               Draw
             </button>
           </li>
+          <li class="nav-item mx-1">
+            <button class="btn btn-outline-secondary" type="button" data-bs-toggle="offcanvas"
+              data-bs-target="#analyseCanvas" aria-controls="analyseCanvas">
+              Analyse
+            </button>
+          </li>
         </ul>
         <form class="d-flex">
           <button class="btn btn-outline-primary mx-1" type="button" data-bs-toggle="collapse"
             data-bs-target="#helpBoxCollapse" aria-expanded="false" aria-controls="helpBoxCollapse">
             Help
           </button>
           <button class="btn btn-outline-primary" type="button" data-bs-toggle="collapse"
@@ -140,15 +149,15 @@
   <!-- Interaction -->
   <div class="offcanvas offcanvas-start canvasControl" data-bs-scroll="true" data-bs-backdrop="false" tabindex="-1"
     id="interactionCanvas" aria-labelledby="interactioneCanvasLabel">
     <div class="offcanvas-header">
       <h5 class="offcanvas-title" id="interactionCanvasLabel">Interaction</h5>
       <button type="button" class="btn-close" data-bs-dismiss="offcanvas" aria-label="Close"></button>
     </div>
-    <div class="offcanvas-body">
+    <div class="offcanvas-body" id="interactionOffCanvasBody">
 
       <div class="mb-3">
         <label for="selection-method" class="form-label">Selection Method</label>
         <select class="form-select" aria-label="Default select example" id="selection-method">
           <option selected, value="particles">Particles</option>
           <option value="species">Species</option>
           <option value="connected">Connected Particles</option>
@@ -157,14 +166,18 @@
         <div id="selection-methodHelp" class="form-text">Select single particles, whole molecules or disable selection.
         </div>
       </div>
       <div class="mb-3">
         <button type="button" class="btn btn-secondary" id="reset_selection">Reset Selection</button>
       </div>
       <div class="mb-3">
+        <input class="form-check-input" type="checkbox" value="" id="multiselect">
+        <label for="multiselect" class="form-label">Select multiple particles</label>
+      </div>
+      <div class="mb-3">
         <label for="addSceneModifier" class="form-label">Select scene modifier</label>
         <select class="form-select" aria-label="Default select example" id="addSceneModifier">
           <option selected, value="none"> </option>
           <option value="add">Add New</option>
         </select>
         <div id="addSceneModifierHelp" class="form-text">Load a Python class to modify the scene
         </div>
@@ -177,19 +190,23 @@
   <div class="offcanvas offcanvas-start canvasControl" data-bs-scroll="true" data-bs-backdrop="false" tabindex="-1"
     id="sceneCanvas" aria-labelledby="sceneCanvasLabel">
     <div class="offcanvas-header">
       <h5 class="offcanvas-title" id="sceneCanvasLabel">Scene</h5>
       <button type="button" class="btn-close" data-bs-dismiss="offcanvas" aria-label="Close"></button>
     </div>
     <div class="offcanvas-body">
-
       <div class="mb-3">
-        <label for="spotLightIntensity" class="form-label" id="spotLightIntensityLabel">Spot light intensity:
+        <label for="cameraLightIntensity" class="form-label" id="cameraLightIntensityLabel">Camera light intensity:
           1.0</label>
-        <input type="range" class="form-range" min="0" max="1" step="0.01" id="spotLightIntensity" value="1">
+        <input type="range" class="form-range" min="0" max="1" step="0.01" id="cameraLightIntensity" value="1">
+      </div>
+      <div class="mb-3">
+        <label for="spotLightIntensity" class="form-label" id="spotLightIntensityLabel">Spot light intensity:
+          0.0</label>
+        <input type="range" class="form-range" min="0" max="1" step="0.01" id="spotLightIntensity" value="0">
       </div>
       <div class="mb-3">
         <label for="hemisphereLightIntensity" class="form-label" id="hemisphereLightIntensityLabel">Hemisphere light
           intensity: 1.0</label>
         <input type="range" class="form-range" min="0" max="1" step="0.01" id="hemisphereLightIntensity" value="0.1">
       </div>
       <div class="mb-3">
@@ -200,14 +217,18 @@
       <div class="mb-3">
         <input class="form-check-input" type="checkbox" value="" id="autoRestart">
         <label class="form-check-label" for="autoRestart">
           Auto Restart
         </label>
       </div>
       <div class="mb-3">
+        <input class="form-check-input" type="checkbox" value="" id="showBox">
+        <label for="showBox" class="form-label">Show Box (static)</label>
+      </div>
+      <div class="mb-3">
         <button type="button" class="btn btn-secondary" id="reset">Reset Scene</button>
         <button type="button" class="btn btn-secondary" id="animate" {% if config.update_function %} disabled {% endif
           %}>Load Animation</button>
       </div>
     </div>
   </div>
 
@@ -223,82 +244,31 @@
       <div class="mb-3">
         <button type="button" class="btn btn-secondary" id="drawAddAnchor">Add anchor point</button>
         <button type="button" class="btn btn-secondary" id="drawRemoveLine">Remove Line</button>
       </div>
     </div>
   </div>
 
-
-  <!-- TODOs -->
-  <div style="display: none;">
-    <div class="row">
-      <div class="col-sm">
-        <div class="form-check form-switch">
-        </div>
-
-
-      </div>
-      <div class="col-sm">
-        <div class="row">
-          <div class="col-sm-3">
-            <div class="row">Max FPS</div>
-            <div class="row">POST</div>
-
-            <div class="row">1. Light</div>
-            <div class="row">2. Light</div>
-          </div>
-          <div class="col-sm-2">
-            <div class="row"><output id="frames_per_post_output">{{ config.frames_per_post }}</output></div>
-
-          </div>
-          <div class="col-sm">
-            <div class="row">
-            </div>
-            <div class="row"><input type="range" class="form-range" min="1" max="500" id="frames_per_post"
-                value="{{ config.frames_per_post }}" , oninput="frames_per_post_output.value = this.value">
-            </div>
-
-            <div class="row"></div>
-            <div class="row"></div>
-          </div>
-          <div class="col-sm-1"><!-- Padding on the right --></div>
-
-        </div>
-      </div>
+  <!-- Analyse -->
+  <div class="offcanvas offcanvas-start canvasControl" data-bs-scroll="true" data-bs-backdrop="false" tabindex="-1"
+    id="analyseCanvas" aria-labelledby="analyseCanvasLabel">
+    <div class="offcanvas-header">
+      <h5 class="offcanvas-title" id="analyseCanvasLabel">Analyse</h5>
+      <button type="button" class="btn-close" data-bs-dismiss="offcanvas" aria-label="Close"></button>
     </div>
-    <div class="container">
-      <div class="row">
-        <div class="col-sm">
-
-          <div class="btn-group-vertical" role="group" aria-label="Basic example">
-            <button type="button" class="btn btn-secondary" id="hide_selection" disabled>Hide
-              Selection</button>
-          </div>
-        </div>
-        <div class="col-sm">
-          <div class="btn-group-vertical" role="group" aria-label="Basic example">
-            <button type="button" class="btn btn-outline-dark" id="sphere_plus">+</button>
-            <button type="button" class="btn btn-outline-dark" id="bond_plus">+</button>
-            <button type="button" class="btn btn-outline-dark" id="resolution_plus">+</button>
-          </div>
-          <div class="btn-group-vertical" role="group" aria-label="Basic example">
-            <button type="button" class="btn btn-outline-dark" disabled>Particles</button>
-            <button type="button" class="btn btn-outline-dark" disabled>Bonds</button>
-            <button type="button" class="btn btn-outline-dark" disabled>Resolution</button>
-          </div>
-          <div class="btn-group-vertical" role="group" aria-label="Basic example">
-            <button type="button" class="btn btn-outline-dark" id="sphere_minus">-</button>
-            <button type="button" class="btn btn-outline-dark" id="bond_minus">-</button>
-            <button type="button" class="btn btn-outline-dark" id="resolution_minus">-</button>
-          </div>
-        </div>
+    <div class="offcanvas-body">
+      <div class="mb-3">
+        <button type="button" class="btn btn-secondary" id="analyseDistanceBtn">Get distance</button>
+        <div id="analyseDistanceBtnHelp" class="form-text">Get the distance between two selected particles.</div>
       </div>
+      <div id="analysePlot"></div>
     </div>
   </div>
 
+
   <!-- Info Box -->
   <div class="collapse" id="infoBoxCollapse">
     <div class="container-fluid rounded border border-dark" id="infoBox">
       <dl class="row">
         <dt class="col-sm-3">File</dt>
         <dd class="col-sm-9"><code>{{ config.file }}</code></dd>
         <dt class="col-sm-3">FPS</dt>
@@ -355,15 +325,16 @@
           <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
         </div>
         <div class="modal-body">
           <div class="mb-3">
             <label for="addSceneModifierImport" class="form-label">Path to modifier <code>class</code></label>
             <input type="email" class="form-control" id="addSceneModifierImport"
               aria-describedby="addSceneModifierImportHelp">
-            <div id="addSceneModifierImportHelp" class="form-text">The input should be <code>module.cls</code> such that
+            <div id="addSceneModifierImportHelp" class="form-text">The input should be <code>module.cls</code> such
+              that
               <code> from module import cls</code> works.
             </div>
           </div>
         </div>
         <div class="modal-footer">
           <button type="button" class="btn btn-secondary" data-bs-dismiss="modal">Close</button>
           <button type="button" class="btn btn-primary" id="addSceneModifierImportBtn">Load</button>
```

#### html2text {}

```diff
@@ -5,14 +5,15 @@
 ●
 
  ZnDraw
     *  Particles
     *  Interaction
     *  Scene
     *  Draw
+    *  Analyse
  Help   Info
 
 ** Particles **
 Change the material of the particles and bonds..
 ⁰ Wireframe material
 Sphere radius: {{ config['sphere_size'] }} [Unknown INPUT type]
 Bond diameter: {{ config['bond_size'] }} [Unknown INPUT type]
@@ -20,37 +21,33 @@
 ** Interaction **
  value="particles">Particles
 Species
 Connected Particles
 None
 Select single particles, whole molecules or disable selection.
 Reset Selection
+⁰ Select multiple particles
  value="none">
 Add New
 Load a Python class to modify the scene
 ** Scene **
-Spot light intensity: 1.0 [Unknown INPUT type]
+Camera light intensity: 1.0 [Unknown INPUT type]
+Spot light intensity: 0.0 [Unknown INPUT type]
 Hemisphere light intensity: 1.0 [Unknown INPUT type]
 Max FPS: {{ config.max_fps }}
  oninput="max_fpsLabel.innerHTML = 'Max FPS: ' + this.value">
 ⁰  Auto Restart
+⁰ Show Box (static)
 Reset Scene
 % if config.update_function %} disabled {% endif %}>Load Animation
 ** Draw **
 Add anchor point Remove Line
-Max FPS
-POST
-1. Light
-2. Light
-{{ config.frames_per_post }}
- oninput="frames_per_post_output.value = this.value">
-Hide Selection
-+ + +
-Particles Bonds Resolution
-- - -
+** Analyse **
+Get distance
+Get the distance between two selected particles.
 ***** ZnDraw Help *****
   move light to camera position
       keypress L
   play / pause
       keypress space
   frame forwards / backwards
       keypress ▶\◀
```

### Comparing `zndraw-0.1.4/PKG-INFO` & `zndraw-0.1.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: zndraw
-Version: 0.1.4
+Version: 0.1.5
 Summary: 
 License: Apache-2.0
 Author: zincwarecode
 Author-email: zincwarecode@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: webview
 Requires-Dist: ase (>=3.22.1,<4.0.0)
 Requires-Dist: flask (>=2.2.3,<3.0.0)
 Requires-Dist: networkx (>=3.1,<4.0)
+Requires-Dist: pandas (>=2.0.1,<3.0.0)
+Requires-Dist: plotly (>=5.14.1,<6.0.0)
 Requires-Dist: pydantic (>=1.10.7,<2.0.0)
 Requires-Dist: pywebview (>=4.0.2,<5.0.0) ; extra == "webview"
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Requires-Dist: typer[all] (>=0.7.0,<0.8.0)
 Requires-Dist: znh5md (>=0.1.6,<0.2.0)
 Project-URL: repository, https://github.com/zincware/ZnDraw
 Description-Content-Type: text/markdown
```

