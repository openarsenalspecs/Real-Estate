# HelixPlan

**The geometry was always there.**

HelixPlan is an open-source spatial intelligence system that reconstructs complete architectural floorplans from simple walkthrough video and minimal dimensional inputs.

It converts motion into structure, generating accurate 2D and 3D representations of real-world interiors including walls, rooms, doors, windows, closets, and stairs.

---

## Overview

HelixPlan uses computer vision, SLAM, depth estimation, and structural reasoning to infer the hidden geometry of built environments.

Given:
- A walkthrough video
- Basic house dimensions (length × width)

It produces:
- Structured 2D floorplans
- Optional 3D spatial reconstructions
- Semantic labeling of interior spaces
- Exportable architectural formats

---

## Core Features

### Video-to-Structure Reconstruction
- Converts walkthrough video into spatial geometry
- Frame extraction and keyframe optimization
- Camera motion tracking and pose estimation

### 3D Spatial Reconstruction
- Structure-from-Motion (SfM) pipeline
- Sparse and dense point cloud generation
- Optional NeRF-based reconstruction support

### Semantic Interior Understanding
Detects and classifies:
- Walls
- Doors
- Windows
- Closets
- Stairs
- Room boundaries

### Floorplan Generation Engine
- Converts 3D geometry into structured 2D maps
- Room segmentation using graph-based clustering
- Wall extraction via planar detection
- Connectivity mapping (doors as graph edges)

### Structural Constraint Engine
Ensures architectural validity:
- Doors connect valid spaces
- Rooms maintain geometric enclosure
- Hallways respect minimum width constraints
- Stairs align across vertical transitions
- Prevents physically impossible layouts

### Temporal Consistency Model
Stabilizes video-based reconstruction:
- Reduces frame-to-frame flicker
- Prevents SLAM drift accumulation
- Maintains object identity consistency across frames
- Enforces geometric coherence over time

### Scale Alignment Engine
- Anchors reconstruction using user-provided dimensions
- Uses architectural priors (door height, stair geometry)
- Normalizes spatial scale across entire model

### Automated Measurement Verification Layer
- Validates generated geometry against real-world constraints
- Detects scale drift and structural inconsistencies
- Cross-checks door, stair, and room dimensions
- Produces confidence scores for spatial accuracy

### AI Refinement Layer
- Improves layout accuracy using learned priors
- Graph Neural Networks for room structure correction
- Transformer-based spatial refinement
- Dataset-trained correction models

### Dataset Generation Pipeline
- Converts real-world walkthroughs into training data
- Stores video, geometry, labels, and corrections
- Enables continuous model improvement
- Supports synthetic and real-world augmentation

---

## Output Formats

HelixPlan supports multiple export formats:

- SVG (vector floorplans)
- DXF (CAD-compatible)
- JSON (spatial graph representation)
- IFC (BIM-compatible models)
- Optional 3D mesh exports

---

## Technology Stack

- **Video Processing:** OpenCV, FFmpeg  
- **SLAM / SfM:** COLMAP, ORB-SLAM3, OpenVINS  
- **Depth Estimation:** MiDaS, DPT, NeRF variants  
- **Segmentation:** YOLOv8, SAM, Mask2Former  
- **Geometry Processing:** Open3D, Shapely, Trimesh  
- **Visualization:** Blender, Three.js  
- **ML Frameworks:** PyTorch, ONNX  

---

## Use Cases

- Real estate floorplan generation
- Architectural documentation
- Home renovation planning
- Insurance property mapping
- Construction verification
- Digital twin creation

---

## Project Vision

HelixPlan is built on a simple principle:

> The geometry was always there.

It does not invent space—it reconstructs it from observation, motion, and structure.

---

## Specification Branding License (SBL)

### Standard
- Fully AGPL-3.0+ compliant system
- Copyleft enforced for network deployments
- Required attribution:
  - Roxanne Ardary
  - https://www.roxanneardary.com/

### Optional

- **Specification Branding License (SBL)**
  - Attribution-free commercial deployment
  - Pricing based on scale, usage, and deployment scope
  - [https://roxanneardary.com/helixplan/](https://roxanneardary.com/helixplan/)  

---

## License & Notice Requirements

HelixPlan is released under the **GNU Affero General Public License v3.0 or later (AGPL-3.0+)**.   
By contributing to this project, you agree that your contributions will also be released under this license.

Please note the following:

- All contributions must comply with the **AGPL-3.0+** terms.  
- Under **Section 7** of the license, all redistributions, forks, and derivative works must preserve attribution to:  
  **Roxanne Ardary** and **[roxanneardary.com](https://www.roxanneardary.com/)**.
- The project's **notice.md** file tracks attribution requirements and contributor acknowledgments.   
  Any update that adds new contributors or modifies attribution should also update `notice.md`. 
- When submitting a pull request, ensure that any new files maintain the attribution headers where applicable.
- Network-deployed versions of this software must also remain fully AGPL-3.0+ compliant, including exposure of source code modifications when applicable under the license.

For full legal details, please refer to the AGPL-3.0+ license and the project's `notice.md` file.

---

## Closing Statement

HelixPlan is not just a mapping tool.

It is a system for recovering structure from reality itself.

**The geometry was always there.**
