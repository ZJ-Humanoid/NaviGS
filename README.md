# NaviGS: 3D Gaussian Splatting Dataset of Real-World Scenes

<p align="center">
  <a href="https://zj-humanoid.github.io/NaviGS/"><img src="https://img.shields.io/badge/%F0%9F%8C%90%20Project%20Page-0066FF?style=for-the-badge" alt="Project Page"></a>
  <a href="https://huggingface.co/datasets/zj-humanoid/NaviGS"><img src="https://img.shields.io/badge/%F0%9F%A4%97%20Dataset-FFD21E?style=for-the-badge" alt="Hugging Face"></a>
  <a href="https://creativecommons.org/licenses/by-nc-sa/4.0/"><img src="https://img.shields.io/badge/License-CC%20BY--NC--SA%204.0-lightgrey?style=for-the-badge" alt="License: CC BY-NC-SA 4.0"></a>
</p>

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

## License

NaviGS is released under the [Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License (CC BY-NC-SA 4.0)](https://creativecommons.org/licenses/by-nc-sa/4.0/).

You are free to share and adapt the dataset for non-commercial purposes, provided that you give appropriate credit, indicate any changes, and distribute adaptations under the same license.

For details, please refer to the [full license terms](https://creativecommons.org/licenses/by-nc-sa/4.0/legalcode).

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
