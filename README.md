# threejs-gltf-template
A simple Draco-capable GLTF/GLB Three JS template

Forked from the original to add basic DRACO compression support for a friend.

## Features

* Gradient background with texture noise
* Orbit controller
* Draco compression support

<img src="image.jpg" />

## Usage

Replace the models with your own files

```javascript
loader.load('<my_model.glb>', handle_load);
```

Adjust the camera field of view (FOV) to see more of less of your model in the screen. To change the FOV update the number 24 in the code below.

```javascript
var camera = new THREE.PerspectiveCamera(24,window.innerWidth / window.innerHeight,1,1000);
```

Adjust the ambient light in the scene but changing the color or intensity. To change the color update the hex value 0xffffff and to change the intensity change the number 3.

```javascript
var light = new THREE.AmbientLight(0xffffff, 3);
```
