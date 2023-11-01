# Awesome Gaussian Splatting 

A curated list of awesome Gaussian Splatting resources, inspired by awesome-computer-vision.

## Table of Contents

- [Introduction](#introduction)
- [Quick Links](#quick-links)
- [Updates](#updates)
- [Papers](#papers)
- [Implementations](#implementations)
- [Tools](#rendering-and-visualisation-tools)
- [Training](#training)
- [Colabs](#colabs)
- [Explanations](#explanations)
  - [Blog Posts](#blog-posts)
  - [Tutorial Videos](#tutorial-videos)
- [Community](#community)

- [FAQs](#faqs)
- [License](#license)


## Introduction

Gaussian Splatting is a revolutionary technique that combines the advantages of both explicit 3D scene representations like meshes and points, and continuous representations like Neural Radiance Fields (NeRF). It introduces 3D Gaussians as a flexible and expressive scene representation that allows for high-quality, real-time rendering at 1080p resolution. The technique is also optimized for fast training times, making it a highly efficient solution for real-time rendering of complex scenes captured from multiple photos.

## Quick Links

- **Must-Read Paper**: [3D Gaussian Splatting for Real-Time Radiance Field Rendering](https://repo-sam.inria.fr/fungraph/3d-gaussian-splatting/)
- **Must-See Video**: [Short Presentation on 3D Gaussian Splatting](https://youtu.be/T_kXY43VZnk?si=DrkbDFxQAv5scQNT)
- **Implementation**: [3D Gaussian Splatting, reimagined: Unleashing unmatched speed with C++ and CUDA from the ground up!](https://github.com/MrNeRF/gaussian-splatting-cuda)
- **Beginner friendly Introduction**: [Blog: Introduction to 3D Gaussian Splatting](https://huggingface.co/blog/gaussian-splatting)
- **Beginner friendly 2 minute Video**: [3D Gaussian Splatting - Why Graphics Will Never Be The Same](https://www.youtube.com/watch?v=HVv_IQKlafQ)

## Updates

- **1 November 2023**: Added beginner friendly content introducing GS
- **31 October 2023**: Added the paper: 4D Gaussian Splatting for Real-Time Dynamic Scene Rendering
- **30 October 2023**: Added a FAQ section.


## Papers
### Seminal Paper introducing 3D Gaussian Splatting:
#### [3D Gaussian Splatting for Real-Time Radiance Field Rendering](https://repo-sam.inria.fr/fungraph/3d-gaussian-splatting/)
**Authors**: Bernhard Kerbl, Georgios Kopanas, Thomas Leimkühler3, George Drettakis  
**About**: The paper introduces a method using 3D Gaussians and a fast rendering algorithm for high-quality, real-time novel-view synthesis of scenes at 1080p resolution.  
- [📄 Paper (Low Resolution)](https://repo-sam.inria.fr/fungraph/3d-gaussian-splatting/3d_gaussian_splatting_low.pdf) 
- [📄 Paper (High Resolution)](https://repo-sam.inria.fr/fungraph/3d-gaussian-splatting/3d_gaussian_splatting_high.pdf) 
- [🌐 Project Page](https://repo-sam.inria.fr/fungraph/3d-gaussian-splatting/) 
- [💻 Code](https://github.com/graphdeco-inria/gaussian-splatting) 
- [🎥 Short Presentation](https://youtu.be/T_kXY43VZnk?si=DrkbDFxQAv5scQNT) 
- [🎥 Explanation Video](https://www.youtube.com/live/xgwvU7S0K-k?si=edF8NkYtsRbgTbKi)

### Dynamic 3D Gaussian Splatting:
#### [Dynamic 3D Gaussians: Tracking by Persistent Dynamic View Synthesis](https://dynamic3dgaussians.github.io/paper.pdf)
**Authors**: Jonathon Luiten, Georgios Kopanas, Bastian Leibe, Deva Ramanan  
**Aboutn**: This paper presents a method that simultaneously addresses dynamic scene novel-view synthesis and six degree-of-freedom (6-DOF) tracking of all dense scene elements through a collection of 3D Gaussians.
- [📄 Paper](https://dynamic3dgaussians.github.io/paper.pdf) 
- [🌐 Project Page](https://dynamic3dgaussians.github.io/) 
- [💻 Code](https://github.com/JonathonLuiten/Dynamic3DGaussians) 
- [🎥 Explanation Video](https://www.youtube.com/live/hDuy1TgD8I4?si=6oGN0IYnPRxOibpg)
  

### 4D Gaussian Splatting for Real-Time Dynamic Scene Rendering:
#### [4D Gaussian Splatting for Real-Time Dynamic Scene Rendering](https://arxiv.org/pdf/2310.08528.pdf)
**Authors**: Guanjun Wu, Taoran Yi, Jiemin Fang, Lingxi Xie, Xiaopeng Zhang, Wei Wei, Wenyu Liu, Qi Tian, Xinggang Wang  
**About**: The paper introduces 4D Gaussian Splatting (4D-GS) for real-time dynamic scene rendering. It efficiently models both Gaussian motions and shape deformations using a deformation field. The method achieves real-time rendering at high resolutions (70 FPS at 800*800 resolution on an RTX 3090 GPU) while maintaining high quality.
- [📄 Paper](https://arxiv.org/pdf/2310.08528.pdf) 
- [🌐 Project Page](https://guanjunwu.github.io/4dgs/) 
- [💻 Code](https://github.com/hustvl/4DGaussians) 

#### [Deformable 3D Gaussians for High-Fidelity Monocular Dynamic Scene Reconstruction](https://arxiv.org/pdf/2309.13101.pdf)
**Authors**: Ziyi Yang, Xinyu Gao, Wen Zhou, Shaohui Jiao, Yuqing Zhang, Xiaogang Jin  
**About**: The paper proposes a deformable 3D Gaussians Splatting method for dynamic scene reconstruction and real-time rendering, addressing issues faced by implicit methods in rendering dynamic scenes.
- [📄 Paper](https://arxiv.org/pdf/2309.13101.pdf) 
- [🌐 Project Page](https://ingra14m.github.io/Deformable-Gaussians/) 
- [💻 Code (to be released)](https://github.com/ingra14m/Deformable-3D-Gaussians)

### Diffusion 3D Gaussian Splatting:

#### [Text-to-3D using Gaussian Splatting](https://arxiv.org/pdf/2309.16585.pdf)
**Authors**: Zilong Chen, Feng Wang, Huaping Liu  
**About**: This paper presents a novel approach for generating high-quality 3D objects using Gaussian Splatting based text-to-3D generation (GSGEN).
- [📄 Paper](https://arxiv.org/pdf/2309.16585.pdf) 
- [🌐 Project Page](https://gsgen3d.github.io/) 
- [💻 Code](https://github.com/gsgen3d/gsgen) 
- [🎥 Short Presentation](https://streamable.com/28snte) 
- [🎥 Explanation Video](https://www.youtube.com/live/l956ye13F8M?si=ZkvFL_lsY5OQUB7e)

#### [DreamGaussian: Generative Gaussian Splatting for Efficient 3D Content Creation](https://dreamgaussian.github.io/)
**Authors**: Jiaxiang Tang, Jiawei Ren, Hang Zhou, Ziwei Liu, Gang Zeng  
**About**: DreamGaussian proposes a novel 3D content generation framework which leverages a generative 3D Gaussian Splatting model for efficient and quality 3D content creation.
- [📄 Paper](https://arxiv.org/pdf/2309.16653.pdf) 
- [🌐 Project Page](https://dreamgaussian.github.io/) 
- [💻 Code](https://github.com/dreamgaussian/dreamgaussian) 
- [🎥 Explanation Video](https://www.youtube.com/live/l956ye13F8M?si=ZkvFL_lsY5OQUB7e)

#### [GaussianDreamer: Fast Generation from Text to 3D Gaussian Splatting with Point Cloud Priors](https://arxiv.org/pdf/2310.08529.pdf)
**Authors**: Taoran Yi1, Jiemin Fang, Guanjun Wu1, Lingxi Xie, Xiaopeng Zhang, Wenyu Liu, Tian Qi, Xinggang Wang
**About**: GaussianDreamer proposes a fast 3D generation framework, where the 3D diffusion model provides point cloud priors for initialization and the 2D diffusion model enriches the geometry and appearance.
- [📄 Paper](https://arxiv.org/pdf/2310.08529.pdf) 
- [🌐 Project Page](https://taoranyi.com/gaussiandreamer/) 
- [💻 Code](https://github.com/hustvl/GaussianDreamer) 


## Implementations
[3D Gaussian Splatting for Real-Time Radiance Field Rendering](https://github.com/graphdeco-inria/gaussian-splatting)

[GSGEN: Text-to-3D using Gaussian Splatting](https://github.com/gsgen3d/gsgen)

[DreamGaussian: Generative Gaussian Splatting for Efficient 3D Content Creation](https://github.com/dreamgaussian/dreamgaussian)

[3D Gaussian Splatting, reimagined: Unleashing unmatched speed with C++ and CUDA from the ground up!](https://github.com/MrNeRF/gaussian-splatting-cuda)



## Rendering and Visualisation Tools

#### [Three.js-based implementation of the 3D Gaussian splat viewer](https://github.com/mkkellogg/GaussianSplats3D)
A Three.js implementation that demonstrates 3D Gaussian splatting. This project showcases a viewer for visualizing 3D Gaussian splats in a web-based application.

#### [WebRTC viewer](https://github.com/dylanebert/gaussian-viewer)
This project is a WebRTC implementation for viewing Gaussian splatting in real-time, allowing for interactive viewing experiences over the web.

#### [WebGL implementation of a real-time renderer](https://huggingface.co/spaces/cakewalk/splat)
A real-time renderer implemented in WebGL for viewing Gaussian splatting. This project aims to provide a high-performance rendering experience on the web.

#### [WebGPU viewer](https://github.com/cvlab-epfl/gaussian-splatting-web)
A WebGPU-based viewer for Gaussian splatting, showcasing real-time rendering capabilities and leveraging the power of WebGPU for enhanced performance.

#### [AR Gaussian Splatting for iOS & Metal](https://github.com/laanlabs/metal-splats)
A toy project on GitHub showcasing an iOS and Metal AR Gaussian Splat Renderer. This viewer is designed for rendering Gaussian splatting in an AR environment on iOS devices using Metal.

#### [Gaussian Splatting visualization in Unity](https://github.com/aras-p/UnityGaussianSplatting)
This project demonstrates Gaussian splatting visualization within the Unity game engine. It provides a Unity-based implementation for rendering and viewing Gaussian splats.

#### [CUDA accelerated rasterization of Gaussians with python bindings](https://github.com/nerfstudio-project/gsplat)
A project that showcases CUDA accelerated rasterization of Gaussians with Python bindings. This viewer leverages CUDA for high-performance rendering and rasterization of Gaussians.

## Training
- [fast: C++/CUDA](https://github.com/MrNeRF/gaussian-splatting-cuda)
- [nerfstudio: python/CUDA](https://github.com/nerfstudio-project/gsplat)

## Colabs 
- [Clip Guided Gaussian Splatting Colab](https://colab.research.google.com/drive/1YniEH63VfZPuRGTddviUvNH48cDaLqtg)
- [Gaussian splitting viewer colab](https://colab.research.google.com/github/camenduru/gaussian-splatting-colab/blob/main/gaussian_splatting_viewer_colab.ipynb)




  
## Explanations

### Blog Posts

#### Gaussian Splatting is pretty cool
**Summary**: This blog post discusses the essence and benefits of Gaussian Splatting in rendering, shedding light on how it's a game changer for real-time, high-quality rendering, and how it could be applied in game development.
- [Read more](https://aras-p.info/blog/2023/09/05/Gaussian-Splatting-is-pretty-cool/)

#### Making Gaussian Splats smaller
**Summary**:The author explores techniques and shares insights on how to make Gaussian splats smaller to optimize performance without compromising the quality of rendering.
- [Read more](https://aras-p.info/blog/2023/09/13/Making-Gaussian-Splats-smaller/)

#### Making Gaussian Splats more smaller
**Summary**: A continuation of exploring ways to optimize the size of Gaussian Splats for better performance in rendering tasks.
- [Read more](https://aras-p.info/blog/2023/09/27/Making-Gaussian-Splats-more-smaller/)

#### Introduction to 3D Gaussian Splatting
**Summary**: The post breaks down the rasterization technique of 3D Gaussian Splatting, elaborating on how it enables real-time rendering of photorealistic scenes from small image samples, its process, and its potential impact on the future of graphics.
- [Read more](https://huggingface.co/blog/gaussian-splatting)
  

### Tutorial Videos

#### Getting Started with 3DGS
**Summary**: A tutorial video guiding viewers on how to get started with 3D Gaussian Splatting, covering the basics and essential steps to utilize this rendering technique.
  [Watch here](https://youtu.be/UXtuigy_wYc?si=j1vfORNspcocSH-b)

#### How to view 3DGS Scenes in Unity
**Summary**: This tutorial demonstrates how to view 3D Gaussian Splatting scenes in Unity, providing a practical guide for developers interested in integrating this technique in their projects.
  [Watch here](https://youtu.be/5_GaPYBHqOo?si=6u9j1HqXwF_5WSUL)
  
#### Gaussian Splatting explorations
 **Summary**:Dive into Gaussian Splatting: what is it, how are scenes represented, and what fun things can we do with it?
  [Watch here](https://www.youtube.com/watch?v=jV1g5OY0L5s)



## Community
- [Reddit GaussianSplatting Subreddit](https://www.reddit.com/r/GaussianSplatting)


## FAQs

### What is 3D Gaussian Splatting?

- **A**: 3D Gaussian Splatting is a novel technique introduced for real-time, high-quality rendering of 3D scenes. It uses 3D Gaussians as a flexible and expressive scene representation, optimized for both visual quality and computational efficiency.

### How does 3D Gaussian Splatting differ from traditional 3D scene representations like meshes and points?

- **A**: Traditional 3D scene representations like meshes and points are explicit and well-suited for fast GPU/CUDA-based rasterization. However, they lack the continuous nature that some other methods like Neural Radiance Fields (NeRF) offer. 3D Gaussian Splatting combines the best of both worlds, offering a continuous yet efficient representation.

### What are the advantages of using 3D Gaussian Splatting over Neural Radiance Fields (NeRF)?

- **A**: While NeRF methods offer high visual quality, they require costly stochastic sampling for rendering, which can result in noise. 3D Gaussian Splatting allows for state-of-the-art visual quality and competitive training times, without the need for costly sampling. It also ensures real-time rendering at high resolutions like 1080p.

### What are the core components of the 3D Gaussian Splatting method?

- **A**: The method has three main components:
  1. 3D Gaussians as a flexible and expressive scene representation.
  2. Optimization of the properties of these 3D Gaussians, including their 3D position, opacity, anisotropic covariance, and spherical harmonic coefficients.
  3. A real-time rendering solution that uses fast GPU sorting algorithms and is inspired by tile-based rasterization.

### How does 3D Gaussian Splatting achieve real-time rendering?

- **A**: The method employs a tile-based splatting solution for real-time rendering. It uses fast GPU sorting algorithms and is inspired by tile-based rasterization techniques. This allows for anisotropic splatting that respects visibility ordering and enables a fast and accurate backward pass.

### What kind of optimization times can one expect with 3D Gaussian Splatting?

- **A**: The method is optimized for fast training times, making it a highly efficient solution for real-time rendering of complex scenes. For example, it can achieve training speeds and quality similar to the fastest existing methods, and it provides the first real-time rendering solution with high quality for novel-view synthesis.

### Is 3D Gaussian Splatting suitable for dynamic scenes?

- **A**: The paper primarily focuses on real-time rendering for scenes captured with multiple photos. However, its flexible and expressive representation makes it a promising candidate for dynamic scenes as well.

  
## License 
MIT
