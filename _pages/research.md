---
layout: single
title: "Research"
permalink: /research/
author_profile: true
---

{% include base_path %}

<hr style="border-top: 2px solid #ccc; margin: 20px 0;">

**-Current-**

* **Neural Implicit Surface/Shape Reconstruction for 3D Ultrasound Imaging**, *Sep 2023 - present*

    *  Multi-view Shape Reconstruction using Signed Distance Function (In progress)

    *  Single-view Surface Reconstruction using Signed Distance Function: [arXiv preprint](https://arxiv.org/abs/2401.05915)

    *  Single-view Surface Reconstruction using Unsigned Distance Function: [2023 IEEE IUS Conference](https://ieeexplore.ieee.org/abstract/document/10307668)
    
    Currently, I mainly focus on the surface/shape reconstruction to improve the geometric quality and visualization appearance of the 3D ultrasound volume.
    Traditional methods, such as ISO-Surface and Poisson surface reconstruction, cannot produce a high-quality surface due to image noise. Despite improvements in smoothness, continuity, and resolution from deep learning approaches, research on surface reconstruction in freehand 3D ultrasound is still missing. However, deep learning-based approaches are challenging for 3D ultrasound due to difficult-to-extract boundaries and unavailable large-scale training data or templates.
    In this project, we propose a self-supervised neural implicit surface/shape reconstruction method to learn (un)signed distance functions (SDF, UDF) from ultrasound volumes. The proposed method demonstrates its adaptability to various anatomical structures and improved high-resolution visual quality. 

<div  align="center">    
 <img src="/images/NeuralSurface.png" width = "600"  alt="Framework" align=center />

</div>


**-Ongoing Projects-**
* **Development of Portable Freehand 3D Ultrasound Imaging Systems**, *Sep 2019 - Present*
    * 3D Spine Imaging System: [2020 EMBC Conference](https://ieeexplore.ieee.org/abstract/document/9176614)
    * 3D Photoacoustic Imaging System: [2022 Journal of Applied Physics](https://pubs.aip.org/aip/jap/article-abstract/132/7/074904/2837375/Hand-held-free-scan-3D-photoacoustic-tomography?redirectedFrom=fulltext)
    * 3D Carotid artery Imaging System: [2023 IEEE TUFFC Journal](https://ieeexplore.ieee.org/abstract/document/10368098)
    * 3D Intraoral Imaging System:, supervised by Dr. Lawrence H Le during my visiting in University of Alberta in 2023. [2023 IUS Conference](https://ieeexplore.ieee.org/abstract/document/10308083)

    This project aims to build portable freehand 3D ultrasound imaging systems for various applications. The development of a freehand 3D ultrasound imaging system a rapidly advancing technology to obtain the high-quality 3D volumes without the limitation of field-of-view. Such imaging system commonly compounds the collected 2D B-mode images from the transducer and the corresponding 3D poses from the tracking device into a volume to reconstruct the 3D internal structures of the human body. The system can be built following two main positioning strategies:
    1)	Electromagnetic tracking and 2) Optical tracking.
    The electromagnetic tracking method is simple to use, flexible to install, and low-cost, but it is limited by accuracy and magnetic field interference. 
    The optical tracking method has the advantages of high accuracy and stable positioning, but it is easily affected by occlusion.

    In this project, we design our systems according to different clinical scenarios. We customize a windows client for data collection, image processing and visualization. 

    1)	3D Spine imaging system. A wireless convex ultrasound scanner (5 MHz) and an EM tracking device are used to build this system.
    
    2)	3D Photoacoustic Imaging System. A linear array ultrasound scanner (7.5 MHz) and an EM tracking device are used to build this system.

    3)	3D Carotid artery imaging system. A linear array ultrasound scanner (10 MHz) and an EM tracking device are used to build this system.
    
    4)	3D Intraoral Imaging System. An in-house designed high-frequency ultrasound transducer (20 MHz) and an optical tracking device are combined to build this system. I finished this project in University of Alberta supervised by Dr.Lawrence H Le during my visiting in 2023.

<div  align="center">    
 <img src="/images/PortableSystem.png" width = "500"  alt="Framework" align=center />
</div>


<div  align="center">    
 <img src="/images/image1.gif" width = "500" alt="Framework" align=center />
</div>


<div  align="center">    
  A volunteer is being scanned using 3D spine imaging system
  
</div>

<div  align="center">      
  ——Customized Windows Client by Hongbo Chen

</div>

**-Past Projects-**

* **Automatic Assessment System for Spine Deformity using Freehand 3D Ultrasound Imager**, *Nov 2021 - Aug 2023*
    * Spine Detection using Transformer: [2022 IUS Conference](https://ieeexplore.ieee.org/abstract/document/9958621)
    * Framework Establishment: [2024 IEEE TUFFC Journal](https://ieeexplore.ieee.org/abstract/document/10385188) 

      
    This project aims to establish a general assessment framework to automatically estimate spinal deformity in ultrasound spine images. The proposed framework comprises four major components, a US spine image generator, a novel transformer-based lightweight spine detector network, an angle evaluator, and a 3-D modeler. This framework can be easily applied in the current large-scale scoliosis screening setup without radiation and demonstrate the potential of automatic 3-D parametric modeling for 3-D deformity visualization.

<div  align="center">    
 <img src="/images/AutoAsseesment.png" width = "400"  alt="Framework" align=center />
</div>



<!-- ![@Copyright Reserved IEEE Transactions on Ultrasonics, Ferroelectrics, and Frequency Control](/images/AutoAsseesment.png) -->





* **Fast Reconstruction of Freehand 3D Ultrasound Spine Imaging**, *2018 - 2021*
    * Fast-Dot Projection: [2019 IEEE IUS Conference](https://ieeexplore.ieee.org/abstract/document/8925758)
    * Improvement of Fast Reconstruction: [2021 IEEE TUFFC Journal](https://ieeexplore.ieee.org/abstract/document/9449836)

    This project is my first project at ShanghaiTech University. The purpose is to design a general accelerator that can accelerate existing traditional reconstruction algorithms.
    For large field-of-view 3-D ultrasound reconstruction such as spine imaging, 2-D transverse images and the corresponding spatial information are acquired by the ultrasound probe with a tracking sensor. In general, the number of 2-D images could be as high as 2000 depending on the scan length. Therefore, the process of fusing the data into a 3-D volume is time-consuming.
    To overcome this problem, we propose the Fast-Dot Projection (FDP) method, which simplifies the projection process in reconstruction by replacing a complex vector operation with numerical addition. The proposed method has the following advantages: (1) it can be adapted to various traditional reconstruction algorithms such as Voxel-based back mapping or Pixel-based forward mapping; (2) the fusion speed is fast, for example, the time of rebuilding a full spine image can drop to 26 sec when only using CPU; (3) the reduction (up to 5 times faster than conventional algorithms based on complex vector calculation) of computation cost permits real-time visualization during scanning, which enables clinical diagnosis and assessment possible at the point of care.


<div  align="center">    
 <img src="/images/FastRecons.png" width = "500"  alt="Pipeline" align=center />
</div>