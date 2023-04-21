# Comparing `tmp/zndraw-0.1.2.tar.gz` & `tmp/zndraw-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zndraw-0.1.2.tar", max compression
+gzip compressed data, was "zndraw-0.1.3.tar", max compression
```

## Comparing `zndraw-0.1.2.tar` & `zndraw-0.1.3.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0    13576 2023-04-12 16:10:14.508402 zndraw-0.1.2/LICENSE
--rw-r--r--   0        0        0     1087 2023-04-16 21:37:27.597455 zndraw-0.1.2/README.md
--rw-r--r--   0        0        0      663 2023-04-16 22:45:01.403863 zndraw-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      125 2023-04-15 20:56:00.080869 zndraw-0.1.2/zndraw/__init__.py
--rw-r--r--   0        0        0     2123 2023-04-16 23:24:29.648456 zndraw-0.1.2/zndraw/app.py
--rw-r--r--   0        0        0     2121 2023-04-16 23:27:51.346288 zndraw-0.1.2/zndraw/cli.py
--rw-r--r--   0        0        0     1377 2023-04-16 23:24:33.028420 zndraw-0.1.2/zndraw/globals.py
--rw-r--r--   0        0        0     1074 2023-04-15 22:53:05.753961 zndraw-0.1.2/zndraw/io.py
--rw-r--r--   0        0        0     9533 2023-04-16 19:41:04.734213 zndraw-0.1.2/zndraw/static/favion-192x192.png
--rw-r--r--   0        0        0     4541 2023-04-16 21:05:21.578456 zndraw-0.1.2/zndraw/static/main.css
--rw-r--r--   0        0        0    18045 2023-04-16 23:24:48.368255 zndraw-0.1.2/zndraw/static/main.js
--rw-r--r--   0        0        0    11491 2023-04-16 22:23:39.187556 zndraw-0.1.2/zndraw/templates/index.html
--rw-r--r--   0        0        0     1762 1970-01-01 00:00:00.000000 zndraw-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    13576 2023-04-12 16:10:14.508402 zndraw-0.1.3/LICENSE
+-rw-r--r--   0        0        0     1734 2023-04-21 13:19:36.154627 zndraw-0.1.3/README.md
+-rw-r--r--   0        0        0      797 2023-04-21 13:19:36.154627 zndraw-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      125 2023-04-15 20:56:00.080869 zndraw-0.1.3/zndraw/__init__.py
+-rw-r--r--   0        0        0     3475 2023-04-21 13:19:36.154627 zndraw-0.1.3/zndraw/app.py
+-rw-r--r--   0        0        0     2613 2023-04-19 19:55:37.727848 zndraw-0.1.3/zndraw/cli.py
+-rw-r--r--   0        0        0     2356 2023-04-21 13:19:36.164627 zndraw-0.1.3/zndraw/examples/__init__.py
+-rw-r--r--   0        0        0     3491 2023-04-21 13:19:36.164627 zndraw-0.1.3/zndraw/globals.py
+-rw-r--r--   0        0        0     1208 2023-04-18 14:25:10.131721 zndraw-0.1.3/zndraw/io.py
+-rw-r--r--   0        0        0     9533 2023-04-17 10:14:40.724969 zndraw-0.1.3/zndraw/static/favion-192x192.png
+-rw-r--r--   0        0        0     4714 2023-04-21 13:19:36.164627 zndraw-0.1.3/zndraw/static/main.css
+-rw-r--r--   0        0        0    24146 2023-04-21 13:19:36.164627 zndraw-0.1.3/zndraw/static/main.js
+-rw-r--r--   0        0        0    12956 2023-04-21 13:19:36.164627 zndraw-0.1.3/zndraw/templates/index.html
+-rw-r--r--   0        0        0     2626 1970-01-01 00:00:00.000000 zndraw-0.1.3/PKG-INFO
```

### Comparing `zndraw-0.1.2/LICENSE` & `zndraw-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.2/pyproject.toml` & `zndraw-0.1.3/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,35 +1,41 @@
 [tool.poetry]
 name = "zndraw"
-version = "0.1.2"
+version = "0.1.3"
 description = ""
 authors = ["zincwarecode <zincwarecode@gmail.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = "^3.10"
+python = "^3.9"
 ase = "^3.22.1"
 networkx = "^3.1"
 typer = {extras = ["all"], version = "^0.7.0"}
 flask = "^2.2.3"
 tqdm = "^4.65.0"
+pywebview = {version = "^4.0.2", optional = true}
+znh5md = "^0.1.6"
+pydantic = "^1.10.7"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 ruff = "^0.0.261"
 pytest = "^7.3.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 zndraw = 'zndraw.cli:cli'
 
+[tool.poetry.extras]
+webview = ["pywebview"]
+
 [tool.poetry.urls]
 repository = "https://github.com/zincware/ZnDraw"
 
 [tool.ruff]
 line-length = 90
 
 select = ["I"]
```

### Comparing `zndraw-0.1.2/zndraw/static/favion-192x192.png` & `zndraw-0.1.3/zndraw/static/favion-192x192.png`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.2/zndraw/static/main.css` & `zndraw-0.1.3/zndraw/static/main.css`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+:root {
+    --spinner-size: 60px;
+}
+
+
 body {
     margin: 0;
     /* overflow: hidden;  don't show scrolling bars */
 }
 
 canvas {
     position: absolute;
@@ -26,60 +31,66 @@
     position: absolute;
     bottom: 50%;
     left: 50%;
     z-index: 100;
     display: block;
 }
 
-#help_btn {
+#right_btn_group {
     position: absolute;
     top: 5px;
     right: 10px;
     width: 30px;
     z-index: 100;
     display: block;
     opacity: 0.5;
 }
 
+#add_class {
+    z-index: 2000;
+    display: none;
+
+}
+
 .atom-spinner,
 .atom-spinner * {
     box-sizing: border-box;
 }
 
 .atom-spinner {
-    height: 150px;
-    width: 150px;
+    height: var(--spinner-size);
+    width: var(--spinner-size);
     overflow: hidden;
 }
 
 .atom-spinner .spinner-inner {
     position: relative;
     display: block;
     height: 100%;
     width: 100%;
 }
 
 .atom-spinner .spinner-circle {
     display: block;
     position: absolute;
     color: #ffa500;
-    font-size: calc(60px * 0.24);
+    font-size: calc(var(--spinner-size) * 0.24);
     top: 50%;
     left: 50%;
     transform: translate(-50%, -50%);
 }
 
 .atom-spinner .spinner-line {
     position: absolute;
     width: 100%;
     height: 100%;
     border-radius: 50%;
-    animation-duration: 2s;
-    border-left-width: calc(60px / 25);
-    border-top-width: calc(60px / 25);
+    animation-duration: 1s;
+    border-left-width: calc(var(--spinner-size) / 25);
+    border-top-width: calc(var(--spinner-size) / 25);
     border-left-color: #ffa500;
     border-left-style: solid;
     border-top-style: solid;
     border-top-color: transparent;
 }
 
 .atom-spinner .spinner-line:nth-child(1) {
```

### Comparing `zndraw-0.1.2/zndraw/static/main.js` & `zndraw-0.1.3/zndraw/static/main.js`

 * *Files 25% similar despite different names*

#### js-beautify {}

```diff
@@ -23,33 +23,27 @@
 
     return undefined;
 
 }
 
 // THREE.Cache.enabled = true;
 
-let config = {};
+/**
+ * ThreeJS variables
+ */
 
 const scene = new THREE.Scene();
 const camera = new THREE.PerspectiveCamera(75, window.innerWidth / window.innerHeight, 0.1, 1000);
-
 const renderer = new THREE.WebGLRenderer({
     antialias: true,
     alpha: true
 });
-renderer.setSize(window.innerWidth, window.innerHeight);
-document.body.appendChild(renderer.domElement);
 
 const hemisphereLight = new THREE.HemisphereLight(0xffffff, 0x777777, 0.1);
-const spotLight = new THREE.SpotLight(0xffffff, 1);
-spotLight.position.set(0, 0, 100);
-scene.add(spotLight);
-
-scene.add(hemisphereLight);
-
+const spotLight = new THREE.SpotLight(0xffffff, 1, 0, Math.PI / 2);
 
 const atomsGroup = new THREE.Group();
 
 const bondsGroup = new THREE.Group();
 const bondsGroup_1 = new THREE.Group();
 const bondsGroup_2 = new THREE.Group();
 
@@ -77,33 +71,62 @@
     }),
     "MeshToonMaterial": new THREE.MeshToonMaterial({
         color: "#ffa500"
     }),
 
 };
 
+/**
+ * Three JS Setup
+ */
+
+renderer.setSize(window.innerWidth, window.innerHeight);
+document.body.appendChild(renderer.domElement);
+
+
+spotLight.position.set(0, 0, 100);
+scene.add(spotLight);
+
+scene.add(hemisphereLight);
+
+let config = {};
+
+
 // some global variables
 let frames = [];
 let selected_ids = [];
 let animation_frame = 0;
 let scene_building = false;
 let animation_running = true;
 let data_loading = false;
 let fps = [];
 
+let keydown = {
+    "shift": false,
+    "ctrl": false,
+    "alt": false,
+    "c": false,
+    "l": false
+};
+
+/**
+ * DOM variables
+ */
+
 const div_info = document.getElementById('info');
 const div_loading = document.getElementById('loading');
 const div_progressBar = document.getElementById('progressBar');
 const div_bufferBar = document.getElementById('bufferBar');
 const div_greyOut = document.getElementById('greyOut');
 const div_lst_selected_ids = document.getElementById('lst_selected_ids');
 const div_FPS = document.getElementById('FPS');
 const div_n_particles = document.getElementById('n_particles');
 const div_n_bonds = document.getElementById('n_bonds');
 const div_help_container = document.getElementById('help_container');
+const div_python_class_control = document.getElementById('python_class_control');
 
 const o_selectAtoms = document.getElementById('selectAtoms');
 const o_autoRestart = document.getElementById('autoRestart');
 const o_animate = document.getElementById('animate');
 const o_reset_selection = document.getElementById('reset_selection');
 const o_hide_selection = document.getElementById('hide_selection');
 const o_reset = document.getElementById('reset');
@@ -116,14 +139,16 @@
 const o_resolution_plus = document.getElementById('resolution_plus');
 const o_resolution_minus = document.getElementById('resolution_minus');
 const o_materialSelect = document.getElementById('materialSelect');
 const o_wireframe = document.getElementById('wireframe');
 const o_spotLightIntensity = document.getElementById('spotLightIntensity');
 const o_hemisphereLightIntensity = document.getElementById('hemisphereLightIntensity');
 const o_help_btn = document.getElementById('help_btn');
+const o_add_btn = document.getElementById('add_btn');
+const o_newPythonClassBtn = document.getElementById('newPythonClassBtn');
 
 
 // Helper Functions
 
 async function load_config() {
     config = await (await fetch("config")).json();
     console.log(config)
@@ -135,45 +160,14 @@
         option.text = material;
         option.value = material;
         o_materialSelect.appendChild(option);
     }
     o_materialSelect.value = "MeshPhongMaterial";
 }
 
-function center_camera() {
-    // try to move the camera such that all atoms are in view
-
-    let trials = 0;
-
-    const frustum = new THREE.Frustum()
-
-    camera.position.x = 0;
-    camera.position.y = 0;
-    camera.position.z = 0;
-
-    atomsGroup.children.forEach((atom) => {
-
-        while (true) {
-            const matrix = new THREE.Matrix4().multiplyMatrices(camera.projectionMatrix, camera.matrixWorldInverse)
-            frustum.setFromProjectionMatrix(matrix)
-            camera.updateMatrix();
-            camera.updateMatrixWorld();
-            if (frustum.containsPoint(atom.position)) {
-                break;
-            }
-            console.log('Atom out of view');
-            camera.position.z += 1;
-            trials += 1;
-            if (trials > 100) {
-                break;
-            }
-        }
-    });
-}
-
 update_materials();
 
 function halfCylinderGeometry(pointX, pointY) {
     // Make the geometry (of "direction" length)
     var direction = new THREE.Vector3().subVectors(pointY, pointX);
 
     var geometry = new THREE.CylinderGeometry(0.15 * config["bond_size"], 0.15 * config["bond_size"], direction.length() / 2, config["resolution"] * 2);
@@ -275,29 +269,36 @@
 
 }
 
 async function build_scene(step) {
     if (scene_building) {
         return;
     }
-    const urls = ["atoms/" + step, "bonds/" + step];
+    const urls = ["atoms", "bonds"];
     animation_frame = step;
     console.log("Updating scene");
 
     div_loading.style.visibility = 'visible';
     div_greyOut.style.visibility = 'visible';
 
     // this is faster then doing it one by one
     const arrayOfResponses = await Promise.all(
         urls.map((url) =>
-            fetch(url)
+            fetch(url, {
+                "method": "POST",
+                "headers": {
+                    "Content-Type": "application/json"
+                },
+                "body": JSON.stringify(step)
+            })
             .then((res) => res.json())
         )
     );
 
+
     drawAtoms(arrayOfResponses[0], arrayOfResponses[1]);
     selected_ids = [];
     await update_selection();
     scene_building = false;
 
     div_n_particles.innerHTML = atomsGroup.children.length;
     div_n_bonds.innerHTML = bondsGroup_1.children.length;
@@ -338,44 +339,74 @@
 
     // update the picking ray with the camera and pointer position
     raycaster.setFromCamera(pointer, camera);
 
     // calculate objects intersecting the picking ray
     const intersects = raycaster.intersectObjects(atomsGroup.children);
 
-    for (let i = 0; i < intersects.length; i++) {
-
-        let mesh = intersects[i].object;
-
-        // mesh.callback();
+    if (intersects.length == 0) {
+        return;
+    }
 
-        if (selected_ids.includes(mesh.userData["id"])) {
-            mesh.material.color.set(mesh.userData["color"]);
-            let index = selected_ids.indexOf(mesh.userData["id"]);
-            if (index !== -1) {
-                selected_ids.splice(index, 1);
-            }
+    // for (let i = 0; i < intersects.length; i++) {
+    let mesh = intersects[0].object;
+    if (!keydown["shift"]) {
+        selected_ids = [mesh.userData["id"]];
+        mesh.material.color.set(0xffa500);
+    } else {
+        if (!selected_ids.includes(mesh.userData["id"])) {
+            mesh.material.color.set(0xffa500);
+            selected_ids.push(mesh.userData["id"]);
         } else {
-            intersects[i].object.material.color.set(0xffa500);
-            selected_ids.push(intersects[i].object.userData["id"]);
-        };
+            mesh.material.color.set(mesh.userData["color"]);
+            selected_ids.splice(selected_ids.indexOf(mesh.userData["id"]), 1);
+        }
     }
+    // update colors here for better performance
+    update_color_of_ids(selected_ids);
     await update_selection();
 }
 
+/**
+ * We update the color of every atom in the scene
+ * @param {list[int]} ids, the selected ids
+ * @returns 
+ */
+
+async function update_color_of_ids(ids) {
+    atomsGroup.children.forEach(function(mesh) {
+        if (ids.includes(mesh.userData["id"])) {
+            mesh.material.color.set(0xffa500);
+        } else {
+            mesh.material.color.set(mesh.userData["color"]);
+        }
+    });
+    return ids;
+}
+
 async function update_selection() {
-    fetch("select", {
+    console.log("Updating selection");
+    div_lst_selected_ids.innerHTML = selected_ids.join(", ");
+    await fetch("select", {
         "method": "POST",
         "headers": {
             "Content-Type": "application/json"
         },
-        "body": JSON.stringify(selected_ids),
-    })
+        "body": JSON.stringify({
+            "selected_ids": selected_ids,
+            "step": animation_frame
+        }),
+    }).then(response => response.json()).then(function(response_json) {
+        if (response_json["updated"]) {
+            update_color_of_ids(response_json["selected_ids"]);
+            selected_ids = response_json["selected_ids"];
+        }
+        div_lst_selected_ids.innerHTML = response_json["selected_ids"].join(", ");
+    });
 
-    div_lst_selected_ids.innerHTML = selected_ids.join(", ");
 }
 
 async function getAnimationFrames() {
     if (data_loading) {
         console.log("Animation read already in progress");
         return;
     }
@@ -384,36 +415,53 @@
     data_loading = true;
     if (frames.length < 2) {
         fetch("load");
     }
 
     let step = frames.length;
     while (true) {
-        let obj = await (await fetch("positions/" + step + "&" + (parseInt(o_frames_per_post.value) + step))).json();
+
+        let obj = await fetch("positions", {
+            "method": "POST",
+            "headers": {
+                "Content-Type": "application/json"
+            },
+            "body": JSON.stringify({
+                "start": step,
+                "stop": parseInt(o_frames_per_post.value) + step
+            }),
+        }).then(response => response.json()).then(function(response_json) {
+            load_config();
+            return response_json;
+        });
+
         console.log("Read " + step + "-" + (parseInt(o_frames_per_post.value) + step) + " frames");
         if (Object.keys(obj).length === 0) {
             console.log("Animation read finished");
             break;
         }
         frames = frames.concat(obj);
         step += parseInt(o_frames_per_post.value);
-        await fetch("atoms/1").then(load_config());
     }
     data_loading = false;
 }
 
 
 if (config["animate"] === true) {
     div_info.innerHTML = "Reading file...";
     getAnimationFrames();
 }
 if (config["restart_animation"] === true) {
     o_autoRestart.checked = true;
 }
 
+/**
+ * Event listeners
+ */
+
 window.addEventListener('pointerdown', onPointerDown, false);
 window.addEventListener('resize', onWindowResize, false);
 
 o_selectAtoms.onclick = function() {
     if (o_selectAtoms.checked) {
         console.log("Selecting atoms");
         window.addEventListener('pointerdown', onPointerDown, false);
@@ -423,23 +471,21 @@
     }
 }
 o_animate.onclick = function() {
     div_info.innerHTML = "Reading file...";
     getAnimationFrames();
 }
 
+
 o_reset_selection.onclick = function() {
-    selected_ids.forEach(function(item, index) {
-        let mesh = atomsGroup.getObjectByUserDataProperty("id", item);
-        mesh.material.color.set(mesh.userData["color"]);
-    });
     selected_ids = [];
     update_selection();
 }
 
+
 o_hide_selection.onclick = function() {
     selected_ids.forEach(function(item, index) {
         let mesh = atomsGroup.getObjectByUserDataProperty("id", item);
         mesh.visible = false;
 
         mesh.userData["bond_ids"].forEach(function(item, index) {
             bondsGroup_1.getObjectById(item).visible = false;
@@ -450,15 +496,14 @@
 
 o_reset.onclick = function() {
     load_config();
     animation_frame = 0;
     build_scene(0);
     selected_ids = [];
     update_selection();
-    center_camera();
 }
 
 o_sphere_plus.onclick = function() {
     config["sphere_size"] += 0.1;
     build_scene(animation_frame);
 }
 
@@ -509,14 +554,168 @@
     div_help_container.style.display = "block";
 }
 
 o_help_btn.onmouseout = function() {
     div_help_container.style.display = "none";
 }
 
+o_add_btn.onclick = function() {
+    document.getElementById("add_class").style.display = "block";
+}
+
+
+/**
+ * Helper function, move later
+ * @param {} name 
+ * @param {*} checked 
+ * @returns 
+ */
+function createRadioElement(name, checked, id, properties) {
+    var radioHtml = '<input class="form-check-input" type="radio" name="' + name + '"  id="' + id + '"';
+    if (checked) {
+        radioHtml += ' checked="checked"';
+    }
+    radioHtml += '/>';
+
+    var radioFragment = document.createElement('div');
+    radioFragment.classList.add("form-check");
+    radioFragment.innerHTML = radioHtml;
+
+
+
+    let function_container = document.createElement('div');
+    function_container.classList.add("container-fluid", "bg-light", "rounded", "border", "border-primary");
+
+    let function_container_label = document.createElement('h5');
+    function_container_label.innerHTML = id;
+
+    function_container.appendChild(function_container_label);
+
+    let function_container_col = document.createElement('div');
+    function_container_col.classList.add("row");
+
+    let descriptions = document.createElement('div');
+    descriptions.classList.add("col-sm-2");
+
+    let values = document.createElement('div');
+    values.classList.add("col-sm-1");
+
+    let controllers = document.createElement('div');
+    controllers.classList.add("col-sm-8");
+
+    function_container_col.appendChild(descriptions);
+    function_container_col.appendChild(values);
+    function_container_col.appendChild(controllers);
+
+    console.log(properties);
+
+    Object.values(properties).forEach((item) => {
+        console.log(item);
+        let label = document.createElement('div');
+        label.innerHTML = item["title"];
+        let label_row = document.createElement('div');
+        label_row.classList.add("row-sm");
+        label_row.appendChild(label);
+
+        let value = document.createElement('div');
+        value.innerHTML = item["default"];
+        let value_row = document.createElement('div');
+        value_row.classList.add("row-sm");
+        value_row.appendChild(value);
+
+        descriptions.appendChild(label_row);
+        values.appendChild(value_row);
+
+        let controller = document.createElement('input');
+        if (item["type"] == "integer") {
+            controller.type = "range";
+            controller.step = 1;
+        } else if (item["type"] == "number") {
+            controller.type = "range";
+            controller.step = 0.1;
+        } else if (item["type"] == "text") {
+            controller.type = "text";
+        } else {
+            console.log("Unknown type: " + item["type"]);
+        }
+        controller.value = item["default"];
+        controller.id = id + "_" + item["title"];
+
+        if ("minimum" in item) {
+            controller.min = item["minimum"];
+        }
+        if ("maximum" in item) {
+            controller.max = item["maximum"];
+        }
+
+        let controller_row = document.createElement('div');
+        controller_row.classList.add("row-sm");
+        controller_row.appendChild(controller);
+
+        controllers.appendChild(controller_row);
+
+        controller.oninput = function() {
+            value.innerHTML = controller.value;
+        }
+
+        controller.onchange = function() {
+            // fetch with post 
+            fetch("update_function_values", {
+                "method": "POST",
+                "headers": {
+                    "Content-Type": "application/json"
+                },
+                "body": JSON.stringify({
+                    "function_id": id,
+                    "property": item["title"],
+                    "value": controller.value
+                })
+            });
+        }
+    });
+    function_container.appendChild(function_container_col);
+    radioFragment.appendChild(function_container);
+
+    return radioFragment;
+}
+
+o_newPythonClassBtn.onclick = function() {
+    document.getElementById("add_class").style.display = "none";
+
+    fetch("add_update_function", {
+        "method": "POST",
+        "headers": {
+            "Content-Type": "application/json"
+        },
+        "body": JSON.stringify(document.getElementById("newPythonClass").value),
+    }).then(response => response.json()).then(function(response_json) {
+        // if not null alert
+        if ("error" in response_json) {
+            alert(response_json["error"]);
+            stepError(response_json["error"]);
+        } else {
+            console.log(response_json);
+            load_config();
+        }
+        return response_json;
+    }).then(function(response_json) {
+        console.log(response_json);
+        div_python_class_control.appendChild(createRadioElement("flexRadioUpdateFunction", true, response_json["title"], response_json["properties"]));
+
+        document.getElementById(response_json["title"]).onclick = function() {
+            console.log("clicked");
+            console.log(document.querySelector('input[name="flexRadioUpdateFunction"]:checked').id);
+            fetch("/select_update_function/" + document.querySelector('input[name="flexRadioUpdateFunction"]:checked').id)
+        };
+
+    });
+
+
+}
+
 window.addEventListener("keydown", (event) => {
     if (event.isComposing || event.key === " ") {
         event.preventDefault();
         if (animation_running && animation_frame == frames.length - 1) {
             animation_frame = 0;
         } else {
             animation_running = !animation_running;
@@ -532,38 +731,71 @@
     }
     if (event.isComposing || event.key === "ArrowUp") {
         animation_frame = parseInt(Math.min(frames.length - 1, animation_frame + (frames.length / 10)));
     }
     if (event.isComposing || event.key === "ArrowDown") {
         animation_frame = parseInt(Math.max(0, animation_frame - (frames.length / 10)));
     }
-    if (event.isComposing || event.key === "l") {
-        spotLight.position.x = camera.position.x;
-        spotLight.position.y = camera.position.y;
-        spotLight.position.z = camera.position.z;
-    }
-    if (event.isComposing || event.key === "r") {
-        center_camera();
-    }
     if (event.isComposing || event.key === "q") {
         getAnimationFrames();
     }
+    if (event.isComposing || event.shiftKey) {
+        keydown["shift"] = true;
+    }
+    if (event.isComposing || event.ctrlKey) {
+        keydown["strg"] = true;
+    }
+    if (event.isComposing || event.altKey) {
+        keydown["alt"] = true;
+    }
+    for (let key in keydown) {
+        if (event.isComposing || event.key === key) {
+            keydown[key] = true;
+        }
+    }
 });
 
-if (config["update_function"] !== null) {
-    window.addEventListener("keydown", (event) => {
-        if (event.isComposing || event.key === "Enter") {
-            div_info.innerHTML = "Processing...";
-            fetch("update/" + animation_frame).then((response) => getAnimationFrames());
-            if (!data_loading) {
-                getAnimationFrames();
-            }
+window.addEventListener("keyup", (event) => {
+    if (event.isComposing || !event.shiftKey) {
+        keydown["shift"] = false;
+    }
+    if (event.isComposing || !event.ctrlKey) {
+        keydown["ctrl"] = false;
+    }
+    if (event.isComposing || !event.altKey) {
+        keydown["alt"] = false;
+    }
+    for (let key in keydown) {
+        if (event.isComposing || event.key === key) {
+            keydown[key] = false;
         }
-    });
-}
+    }
+});
+
+window.addEventListener("keydown", (event) => {
+    if (event.isComposing || event.key === "Enter") {
+        div_info.innerHTML = "Processing...";
+
+        fetch("update", {
+            "method": "POST",
+            "headers": {
+                "Content-Type": "application/json"
+            },
+            "body": JSON.stringify({
+                "selected_ids": selected_ids,
+                "step": animation_frame
+            }),
+        }).then((response) => getAnimationFrames());
+
+        if (!data_loading) {
+            getAnimationFrames();
+        }
+    }
+});
+
 
 
 
 let move_atoms_clock = new THREE.Clock();
 
 
 function move_atoms() {
@@ -599,15 +831,14 @@
         // we need to update the scene
         build_scene(animation_frame);
         scene_building = true;
         return; // we need to wait for the scene to be updated
     }
 
 
-
     frames[animation_frame].forEach(function(item, index) {
         atomsGroup.getObjectByUserDataProperty("id", index).position.set(...item);
     });
 
     div_info.innerHTML = "Frame (" + animation_frame + "/" + (frames.length - 1) + ")";
 
     if (config["bond_size"] > 0) {
@@ -648,22 +879,38 @@
         getAnimationFrames();
     }
 
     div_FPS.innerHTML = (1 / (fps.reduce((a, b) => a + b, 0) / fps.length)).toFixed(2);
     move_atoms_clock.start();
 }
 
+function centerCamera() {
+    if (selected_ids.length === 0) {
+        controls.target = new THREE.Vector3(0, 0, 0);
+    } else {
+        controls.target = atomsGroup.getObjectByUserDataProperty("id", selected_ids[0]).position.clone();
+    }
+}
+
 function animate() {
 
     renderer.render(scene, camera);
     controls.update();
 
     if (frames.length > 0) {
         move_atoms();
     }
+    if (keydown["c"]) {
+        centerCamera();
+    }
+    if (keydown["l"]) {
+        spotLight.position.x = camera.position.x;
+        spotLight.position.y = camera.position.y;
+        spotLight.position.z = camera.position.z;
+    }
 
     // animation loop
 
     requestAnimationFrame(animate);
 }
 
 animate();
```

### Comparing `zndraw-0.1.2/zndraw/templates/index.html` & `zndraw-0.1.3/zndraw/templates/index.html`

 * *Files 16% similar despite different names*

```diff
@@ -185,14 +185,29 @@
                 <dt class="col-sm-3">Function</dt>
                 <dd class="col-sm-9" id="lst_selected_ids"><code>{{ config.update_function }}</code></dd>
                 {% endif %}
               </dl>
             </div>
           </div>
         </div>
+        <div class="accordion-item">
+          <h2 class="accordion-header" id="panelsStayOpen-headingFour">
+            <button class="accordion-button collapsed" type="button" data-bs-toggle="collapse"
+              data-bs-target="#panelsStayOpen-collapseFour" aria-expanded="false"
+              aria-controls="panelsStayOpen-collapseFour">
+              Manipulate Particles
+            </button>
+          </h2>
+          <div id="panelsStayOpen-collapseFour" class="accordion-collapse collapse"
+            aria-labelledby="panelsStayOpen-headingFour">
+            <div class="accordion-body">
+              <div id="python_class_control"></div>
+            </div>
+          </div>
+        </div>
       </div>
     </ul>
   </div>
 
   <div id="loading">
     <div class="atom-spinner">
       <div class="spinner-inner">
@@ -206,15 +221,19 @@
       </div>
     </div>
   </div>
   <div id="info"></div>
   <div id="progressBar"></div>
   <div id="bufferBar"></div>
   <div id="greyOut"></div>
-  <img id="help_btn" src="https://openmoji.org/data/color/svg/2139.svg" />
+  <div id="right_btn_group">
+    <img id="help_btn" src="https://openmoji.org/data/color/svg/2139.svg" />
+    <img id="add_btn" src="https://openmoji.org/data/color/svg/2795.svg" />
+  </div>
+
 
   <div class="container py-4" id="help_container" style="display: none; opacity: 0.9;">
     <div class="h-100 p-5 bg-light rounded-3 border border-primary">
       <h2>ZnDraw Help</h2>
       <br>
       <div class="rounded-3 bg-white" , style="padding-left: 10px;">
         <dl class="row">
@@ -224,22 +243,37 @@
           <dd class="col-sm-9"><code>keypress space</code></dd>
           <dt class="col-sm-3">frame forwards / backwards</dt>
           <dd class="col-sm-9"><code>keypress &#9654;\&#9664; </code></dd>
           <dt class="col-sm-3">jump forwards / backwards</dt>
           <dd class="col-sm-9"><code>keypress &#9650;\&#9660; </code></dd>
           <dt class="col-sm-3">run update function</dt>
           <dd class="col-sm-9"><code>keypress enter</code></dd>
-          <dt class="col-sm-3">reset camera position</dt>
-          <dd class="col-sm-9"><code>keypress R</code></dd>
+          <dt class="col-sm-3">center camera around selected particle</dt>
+          <dd class="col-sm-9"><code>keypress C</code></dd>
           <dt class="col-sm-3">reload animation</dt>
           <dd class="col-sm-9"><code>keypress Q</code></dd>
+          <dt class="col-sm-3">select multiple particles</dt>
+          <dd class="col-sm-9"><code>keydown shift</code></dd>
 
         </dl>
       </div>
     </div>
   </div>
 
+  <div id="add_class">
+    <div class="container py-4" id="help_container">
+      <div class="h-100 p-5 bg-light rounded-3 border border-primary">
+        <div class="form-group">
+          <label for="newPythonClass">Add path to python module</label>
+          <input class="form-control" id="newPythonClass" placeholder="zndraw.examples.Duplicate">
+          <br>
+          <button id="newPythonClassBtn" class="btn btn-primary">Add to Scene</button>
+        </div>
+      </div>
+    </div>
+  </div>
+
 
 
 </body>
 
 </html>
```

#### html2text {}

```diff
@@ -22,26 +22,32 @@
 *****  Controls  *****
 % if config.update_function %} disabled {% endif %}>Load Animation Reset
 Selection Hide Selection Reset Scene
 + + +
 Particles Bonds Resolution
 - - -
 *****  Info  *****
+*****  Manipulate Particles  *****
 ●
-[https://openmoji.org/data/color/svg/2139.svg]
+[https://openmoji.org/data/color/svg/2139.svg] [https://openmoji.org/data/
+color/svg/2795.svg]
 ***** ZnDraw Help *****
 
  style="padding-left: 10px;">
   move light to camera position
       keypress L
   play / pause
       keypress space
   frame forwards / backwards
       keypress ▶\◀
   jump forwards / backwards
       keypress ▲\▼
   run update function
       keypress enter
-  reset camera position
-      keypress R
+  center camera around selected particle
+      keypress C
   reload animation
       keypress Q
+  select multiple particles
+      keydown shift
+Add path to python module [                    ]
+Add to Scene
```

