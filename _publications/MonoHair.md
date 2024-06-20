---
title: "MonoHair: High-Fidelity Hair Modeling from a Monocular Video"
collection: publications
permalink: /publication/MonoHair
excerpt: '[Keyu Wu](https://keyuwu-cs.github.io/), [Lingchen Yang](https://lingchen-chen.github.io/), **Zhiyi Kuang**, Yao Feng, Xutao Han, [Yuefan Shen](https://yuefanshen.net/), [Hongbo Fu](http://sweb.cityu.edu.hk/hongbofu/), [Kun Zhou](http://kunzhou.net/), Youyi Zheng'
date: 2024-05-27
venue: 'CVPR 2024'
paperurl: 'https://arxiv.org/abs/2403.18356'
---

**Abstract**

Undoubtedly, high-fidelity 3D hair is crucial for achieving realism, artistic expression, and immersion in computer graphics. While existing 3D hair modeling methods have achieved impressive performance, the challenge of achieving high-quality hair reconstruction persists: they either require strict capture conditions, making practical applications difficult, or heavily rely on learned prior data, obscuring fine-grained details in images. To address these challenges, we propose MonoHair,a generic framework to achieve high-fidelity hair reconstruction from a monocular video, without specific requirements for environments. Our approach bifurcates the hair modeling process into two main stages: precise exterior reconstruction and interior structure inference. The exterior is meticulously crafted using our Patch-based Multi-View Optimization (PMVO). This method strategically collects and integrates hair information from multiple views, independent of prior data, to produce a high-fidelity exterior 3D line map. This map not only captures intricate details but also facilitates the inference of the hair's inner structure. For the interior, we employ a data-driven, multi-view 3D hair reconstruction method. This method utilizes 2D structural renderings derived from the reconstructed exterior, mirroring the synthetic 2D inputs used during training. This alignment effectively bridges the domain gap between our training data and real-world data, thereby enhancing the accuracy and reliability of our interior structure inference. Lastly, we generate a strand model and resolve the directional ambiguity by our hair growth algorithm. Our experiments demonstrate that our method exhibits robustness across diverse hairstyles and achieves state-of-the-art performance.

[Download Paper](https://arxiv.org/abs/2403.18356)

Recommended citation:

```
@inproceedings{wu2024monohair,
  title={MonoHair: High-Fidelity Hair Modeling from a Monocular Video},
  author={Wu, Keyu and Yang, Lingchen and Kuang, Zhiyi and Feng, Yao and Han, Xutao and Shen, Yuefan and Fu, Hongbo and Zhou, Kun and Zheng, Youyi},
  booktitle={Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition},
  pages={24164--24173},
  year={2024}
}
```
