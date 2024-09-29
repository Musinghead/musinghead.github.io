---
title: "OLAT Gaussians for Generic Relightable Appearance Acquisition"
collection: publications
permalink: /publication/OLAT_Gaussians
excerpt: '**Zhiyi Kuang**, [Yanchao Yang](https://yanchaoyang.github.io/), [Siyan Dong](https://siyandong.github.io/), Jiayue Ma, [Hongbo Fu](https://hongbofu.people.ust.hk/), Youyi Zheng'
date: 2024-11-19
venue: 'SIGGRAPH Asia 2024 Conference'
paperurl: ''
---

**Abstract**

One-light-at-a-time (OLAT) images sample a broader range of object appearance changes than images captured under constant lighting and are superior as input to object relighting. Although existing methods have produced reasonable relighting quality using OLAT images, they utilize surface-like representations, limiting their capacity to model volumetric objects, such as furs. Besides, their rendering process is time-consuming and still far from being used in real-time applications. To address these issues, we propose OLAT Gaussians to build relightable representations of objects from multi-view OLAT images. We build our pipeline on 3D Gaussian Splatting (3DGS), which achieves real-time high-quality rendering. To augment 3DGS with relighting capability, we assign each Gaussian a learnable feature vector, serving as an index to query the objects’ appearance field. Specifically, we decompose the appearance field into an incident illumination function and a scattering function. The former accounts for light transmittance and foreshortening effects, while the latter represents the object’s material properties to scatter light. Rather than using an off-the-shelf physically-based parametric rendering formulation, we model both functions using multi-layer perceptrons (MLPs). This makes our method suitable for various objects, e.g., opaque surfaces, semi-transparent volumes, furs, fabrics, etc. Given a camera view and a point light position, we compute each Gaussian’s color as the product of the light intensity, the incident illumination value, and the scattering value, and then render the target image through the 3DGS rasterizer. To enhance rendering quality, we further utilize a proxy mesh to provide OLAT Gaussians with normals to improve highlights and visi- bility cues to improve shadows. Extensive experiments demonstrate that our method produces state-of-the-art rendering quality with significantly more details in texture-rich areas than previous methods. Our method also achieves real-time rendering, allowing users to interactively modify camera views and point light positions to get immediate rendering results, which are not available from the offline rendering of previous methods.

[Download Paper](https://musinghead.github.io/publication/OLAT_Gaussians)

Recommended citation:

```
@inproceedings{kuang2024OLAT,
  title={OLAT Gaussians for Generic Relightable Appearance Acquisition},
  author={Kuang, Zhiyi and Yang, Yanchao and Dong, Siyan and Ma, Jiayue and Fu, Hongbo and Zheng, Youyi},
  booktitle={SIGGRAPH Asia 2024 Conference Papers},
  pages={1--8},
  year={2024}
}
```
