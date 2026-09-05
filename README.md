# 🎨 Getting Used to Three.js

> *From fundamental 3D concepts to advanced WebGL magic — my personal journey, step-by-step experimentations, and progress in Three.js.*

---

## 📌 Overview

**`get-use-to-three-js`** is a dedicated laboratory and learning roadmap designed to document my transition from WebGL beginners' concepts to building immersive 3D web experiences. Each directory in this repository represents a standalone milestone, code experiment, or mini-project reflecting a specific technique or concept.

---

## 🗺️ Recommended Three.js Learning Path

This repository is organized following an industry-recommended progression path:
┌─────────────────┐     ┌─────────────────┐     ┌─────────────────┐
│ 1. Foundations  │ ──> │ 2. Interaction  │ ──> │ 3. Realism &    │
│    & Geometry   │     │   & Movement    │     │    Lighting     │
└─────────────────┘     └─────────────────┘     └─────────────────┘
│
┌─────────────────┐     ┌─────────────────┐              │
│ 5. Advanced     │ <── │ 4. Shaders &    │ <────────────┘
│    Opt & Polish │     │    Particles    │
└─────────────────┘     └─────────────────┘

### **Phase 1: Fundamentals (The Big Three)**
*   [x] **The Scene Hierarchy:** Understanding `Scene`, `Camera` (Perspective vs. Orthographic), and `WebGLRenderer`.
*   [x] **Basic Geometries & Mesh:** Box, Sphere, Plane, Cylinder, and Transform properties (Position, Rotation, Scale).
*   [x] **Materials 101:** `MeshBasicMaterial`, `MeshNormalMaterial`, `MeshLambertMaterial`, and `MeshPhongMaterial`.
*   [x] **Animation Loop:** Implementing `requestAnimationFrame`, `Clock`, and delta-time normalization.

### **Phase 2: Lighting, Shadows & Textures**
*   [x] **Light Sources:** Ambient, Directional, Point, Spot, and Hemisphere lights.
*   [x] **Shadow Mapping:** Enabling shadow maps (`castShadow`, `receiveShadow`), adjusting shadow map resolution & bias.
*   [x] **Texture Mapping:** Diffuse/Albedo, Roughness, Metalness, Normal maps, Displacement/Height maps, and AO (Ambient Occlusion).
*   [x] **Environment Maps (HDRIs):** Skyboxes, CubeTextures, and `RGBELoader` for realistic reflections and PBR lighting.

### **Phase 3: Interactivity & Camera Controls**
*   [x] **OrbitControls & Camera Helpers:** Smooth navigation and debugging tools.
*   [x] **Raycasting & Object Selection:** Mouse picking, hovering effects, and click-to-interact events.
*   [x] **Physics Engine Integration:** Integrating Cannon.js / Rapier.js for gravity, collisions, and rigid bodies.
*   [x] **DOM Events & UI Controls:** Binding UI inputs using `dat.gui` / `lil-gui`.

### **Phase 4: Advanced Effects & Performance**
*   [x] **Particle Systems:** `Points`, `BufferGeometry`, custom particle shapes, and animated starfields.
*   [x] **Custom GLSL Shaders:** Writing custom Vertex and Fragment Shaders via `ShaderMaterial`.
*   [x] **3D Model Imports:** Loading `.gltf` / `.glb` models using `GLTFLoader` with animations (`AnimationMixer`).
*   [x] **Post-Processing Pipeline:** `EffectComposer`, Bloom, SSAO, Depth of Field, and Chromatic Aberration.
*   [x] **Performance Optimization:** Instanced Mesh (`InstancedMesh`), texture compression, geometry merging, and memory management (disposing materials/geometries).

---

## 📂 Repository Structure

```tree
get-use-to-three-js/
├── 01-foundations/
│   ├── 01-basic-scene/
│   ├── 02-transformations/
│   └── 03-materials-and-textures/
├── 02-lighting-and-shadows/
│   ├── 01-light-types/
│   └── 02-hdri-environment/
├── 03-interactivity-and-physics/
│   ├── 01-raycasting/
│   └── 02-cannon-physics/
├── 04-models-and-animation/
│   └── 01-gltf-character-loader/
├── 05-shaders-and-postprocessing/
│   ├── 01-first-custom-shader/
│   └── 02-bloom-effect/
└── README.md

this for testing pushing to main