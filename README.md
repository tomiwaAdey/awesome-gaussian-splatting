# Awesome Gaussian Splatting 

A curated list of awesome Gaussian Splatting resources, inspired by awesome-computer-vision.

## Table of Contents

- [Papers](#papers)
- [Implementations](#implementations)
- [Tools](#tools)
- [Colabs](#colabs)
- [Explanations](#explanations)
- [Community](#community)


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



## Tools
[Three.js-based implementation of the 3D Gaussian splat viewer](https://github.com/mkkellogg/GaussianSplats3D)

[WebRTC viewer](https://github.com/dylanebert/gaussian-viewer)

[WebGL implementation of a real-time renderer](https://huggingface.co/spaces/cakewalk/splat)

[WebGPU viewer](https://github.com/cvlab-epfl/gaussian-splatting-web)

[AR Gaussian Splatting for iOS & Metal](https://github.com/laanlabs/metal-splats)

[Gaussian Splatting visualization in Unity](https://github.com/aras-p/UnityGaussianSplatting)

[CUDA accelerated rasterization of gaussians with python bindings](https://github.com/nerfstudio-project/gsplat)

## Colabs 
[Clip Guided Gaussian Splatting Colab](https://colab.research.google.com/drive/1YniEH63VfZPuRGTddviUvNH48cDaLqtg)

[Gaussian splitting viewer colab](https://colab.research.google.com/github/camenduru/gaussian-splatting-colab/blob/main/gaussian_splatting_viewer_colab.ipynb)

## Explanations
[Introduction to 3D Gaussian Splatting](https://huggingface.co/blog/gaussian-splatting)

[Gaussian Splatting explorations](https://www.youtube.com/watch?v=jV1g5OY0L5s&ab_channel=DataScienceCastnet)


## Community
- [Reddit GaussianSplatting Subreddit](https://www.reddit.com/r/GaussianSplatting)

## License 
MIT
