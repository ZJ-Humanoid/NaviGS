# NaviGS

> ✅ **First Release · v1.0 is out**, with subsequent versions coming soon.

NaviGS is a real-world 3D Gaussian Splatting (3DGS) dataset comprising **120 high-fidelity indoor and outdoor scenes**, covering **over 50,000 m²** across **10 diverse scene categories**. The dataset provides RGB images, depth observations, LiDAR data, camera poses, 3D Gaussian Splatting (3DGS) representations, reconstructed meshes, and hierarchical scene graphs.

The first phase of the dataset includes **5 RGB scenes and 5 semantic scenes**.

## Dataset Structure

```text
NaviGS/
├── RGB_scene/
│   ├── scene_0/
│   │   ├── RGB/
│   │   ├── depth/
│   │   ├── lidar/
│   │   ├── pose/
│   │   ├── 3dgs/
│   │   └── mesh/
│   ├── scene_1/
│   ├── scene_2/
│   ├── scene_3/
│   └── scene_4/
│
└── semantic_scene/
    ├── apartment0/
    │   ├── RGB/
    │   ├── depth/
    │   ├── lidar/
    │   ├── pose/
    │   ├── 3dgs/
    │   ├── mesh/
    │   └── scenegraph/
    ├── apartment1/
    ├── apartment2/
    ├── resthome0/
    └── meetingroom0/
```

## Data Organization

### RGB Scenes

The `RGB_scene` directory contains five scenes. Each scene includes:

* `RGB/` — RGB images
* `depth/` — Depth observations
* `lidar/` — LiDAR point cloud
* `pose/` — Camera poses and trajectories
* `3dgs/` — 3D Gaussian Splatting representations
* `mesh/` — Reconstructed meshes

### Semantic Scenes

The `semantic_scene` directory contains five scenes with semantic and hierarchical scene understanding annotations.

Each semantic scene includes:

* `RGB/` — RGB images
* `depth/` — Depth observations
* `lidar/` — LiDAR point cloud
* `pose/` — Camera poses and trajectories
* `3dgs/` — 3D Gaussian Splatting representations
* `mesh/` — Reconstructed meshes
* `scenegraph/` — Hierarchical 3D scene graphs

The scene graphs follow the hierarchical **floor–room–stuff–object** organization and provide semantic and spatial relationships between scene elements.

## Scenes

### RGB Scenes

* `scene_0`
* `scene_1`
* `scene_2`
* `scene_3`
* `scene_4`

### Semantic Scenes

* `apartment0`
* `apartment1`
* `apartment2`
* `resthome0`
* `meetingroom0`

## Release

**First Release · v1.0 is out!** The initial release includes **5 RGB scenes and 5 semantic scenes**.

The dataset is now available for download on [Hugging Face](https://huggingface.co/datasets/zj-humanoid/NaviGS).

More documentation, usage instructions, and updates will be provided in subsequent releases.

## Citation

If you use NaviGS in your research, please cite:

```bibtex
@misc{navigs2026,
  title        = {NaviGS: 3D Gaussian Splatting Dataset of Real-World Scenes},
  author       = {Zhejiang Humanoid Robot Innovation Center},
  year         = {2026},
  howpublished = {\url{https://github.com/zj-humanoid/NaviGS}}
}
```
