# In-situ process monitoring and adaptive control for laser-based additive manufacturing [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)
A list of papers about in-situ process monitoring and closed-loop control for laser-based additive manufacturing (LAM) - DED/LPBF. (__continously updating__). The paper collection here focus only on highly cited/open-source/latest articles from __top tier__ journal/conferences.

Other research area including hybrid additive-subtractive manufacturing, physics-informed machine learning for AM, and AM robotic path planning are also briefly included. 

For anyone who wants to do research about AM process monitoring, control, and intelligent decision-making, hope this is helpful to you.   

If you find the paper/code/dataset or have some suggestions, please contact chen1189@e.ntu.edu.sg. Thanks for your valuable contribution to the research community. 


# Table of Contents
- [Latest review articles](#latest-review-articles)
- [In-situ process monitoring](#process-monitoring-for-lam)
    - [Acoustic signal-based monitoring](#acoustic-signal-based-monitoring)
    - [Vision-based monitoring](#vision-based-monitoring-and-inspections)
    - [Thermal-based monitoring](#thermal-based-monitoring-and-inspections)
    - [Point cloud-based surface monitoring](#point-cloud-based-surfacegeometric-monitoring)
- [Closed loop feedback control](#closed-loop-feedback-control)
- [Process planning and robotic path planning for AM and hybrid AM](#process-planning-and-path-planning-for-am-and-hybrid-am)
- [Multimodal process monitoring](#multimodal-process-monitoring) 
- [Hybrid AM - material, process, systems](#hybrid-am---material-process-systems)
- [Physics-informed machine learning for Additive Manufacturing](#physics-informed-machine-learning-for-additive-manufacturing)


<h3> Keywords </h3>

__`datset`__: dataset &emsp; | &emsp; __`code`__: open-soruce code repositories &emsp; | &emsp;
__`control`__: process control &emsp; | &emsp; __`acoustic`__: acoustic-based monitoring &emsp; | &emsp; __`thermal`__: thermal-based monitoring  &emsp; | &emsp;
__`vision`__: vision-based monitoring &emsp; | &emsp; __`PointCloud`__: point cloud &emsp; | &emsp;  __`multimodal`__: multimodal process monitoring &emsp; | &emsp; __`planning`__: AM/hybrid AM process planning &emsp; | &emsp; __`hybridAM`__: hybrid additive-subtractive manufacturing &emsp; | &emsp; __`toolpath`__: AM/SM/hybrid AM toolpath planning &emsp; | &emsp;
__`DED`__: Direct Energy Deposition &emsp; | &emsp; __`LPBF`__: Laser-based powder bed fusion &emsp; | &emsp;
__`AI`__: AI-assisted advanced monitoring approach &emsp; | &emsp;
__`oth.`__: other, including normal-related, correspondence, mapping, matching, alignment, compression, generative model...

Statistics: :fire: code is available  &emsp;|&emsp; :star: citation >= 20 &emsp;|&emsp; :+1: Really good paper that you should pay attention to 
---
## Latest review articles

- [[Additive Manufacturing (2022)](https://www.sciencedirect.com/science/article/abs/pii/S2214860422000963?via%3Dihub)] Research and Application of Machine Learning for Additive Manufacturing] [__`monitoring`__ __`ML`__] 

- [[IJMPT (2022))](https://www.sciencedirect.com/science/article/abs/pii/S0924013621004453)] Mechanistic artificial intelligence (mechanistic-AI) for modeling, design, and control of advanced manufacturing processes: Current state and perspectives.] [__`monitoring`__] 


- [[IEEE/ASME Transactions on Mechatronics (2021))](https://ieeexplore.ieee.org/document/9580759)] Metal-Based Additive Manufacturing Condition Monitoring: A Review on Machine Learning Based Approaches

---
## Process monitoring for LAM

---
### Acoustic signal-based monitoring


- [[JMPT (2022))](https://www.sciencedirect.com/science/article/pii/S0924013622000437)] Deep Transfer Learning of Additive Manufacturing Mechanisms Across Materials in Metal-Based Laser Powder Bed Fusion Process.] [__`monitoring`__ __`acoustic`__ __`SLM`__ __`transfer learning`__] [__code(pytorch), dataset__](https://c4science.ch/diffusion/11778/)  :fire:: :fire:: :+1:

- [[VPP (2021))](https://www.tandfonline.com/doi/abs/10.1080/17452759.2021.1966166)] Semi-supervised Monitoring of Laser powder bed fusion process based on acoustic emissions.] [__`monitoring`__ __`acoustic`__ __`SLM`__] [code(pytorch)](https://c4science.ch/diffusion/11519/) :star:: :fire:: :+1:

- [[Procedia CIRP (2020))](https://www.sciencedirect.com/science/article/pii/S2212827120313408)] Analysis of time, frequency and time-frequency domain features from acoustic emissions during Laser Powder-Bed fusion process.] [__`monitoring`__ __`acoustic`__ __`SLM`__] :+1:


- [[IEEE Transactions on Industrial Informatics (2019)](10.1109/TII.2019.2910524)] Deep Learning for In Situ and Real-Time Quality Monitoring in Additive Manufacturing Using Acoustic Emission [__`monitoring`__ __`acoustic`__ __`SLM`__] :star:: :+1:


- [[The Journal of the Acoustical Society of America (2019)](https://doi.org/10.1121/1.5136551)] Acoustic signals associated with laser-substrate interaction in powder bed fusion additive manufacturing process] [__`monitoring`__ __`acoustic`__ __`SLM`__] 

- [[ 2018 International Solid Freeform Fabrication Symposium (2018)](https://repositories.lib.utexas.edu/handle/2152/90284)] Development of an Acoustic Process Monitoring System for Selective Laser Melting (SLM)] [__`monitoring`__ __`acoustic`__, __`SLM`__] :star::

- [[ AIP Conference Proceedings (2018)](https://doi.org/10.1063/1.5031503)] In-situ acoustic signature monitoring in additive manufacturing processes [__`monitoring`__ __`acoustic`__, __`DED`__, __`in-situ`__] :star:: :+1:

- [[Additive Manufacturing (2017)](https://www.sciencedirect.com/science/article/abs/pii/S221486041730132X)] Acoustic emission for in situ quality monitoring in additive manufacturing using spectral convolutional neural networks.] [__`monitoring`__ __`acoustic`__ __`SLM`__] :star::


- [[Mechanics Research Communications (2017)](https://www.sciencedirect.com/science/article/abs/pii/S009364131630235X)] Acoustic emission monitoring of crack propagation in additively manufactured and conventional titanium components] [__`monitoring`__ __`acoustic`__, __`DED`__, __Offline inspection(not in-situ)__, first time that AE is applied in AM components under fatigue] :star::







---
### Vision-based monitoring and inspections
- [[JMPT (2022)](https://www.sciencedirect.com/science/article/abs/pii/S0924013621004349?dgcid=rss_sd_all)] Deep DIC: Deep learning-based digital image correlation for end-to-end
displacement and strain measurement] [__`monitoring`__ __`DIC`__ __`vision`__]  [__code (pytorch)__](https://github.com/RuYangNU/Deep-Dic-deep-learning-based-digital-image-correlation), [dataset](https://drive.google.com/drive/folders/1n2axHsJ3flHxk_edceY6eOfiX7GjW_d6) :fire::fire:

- [[Robotics and Computer Integrated Manufacturing (2018)](https://www.sciencedirect.com/science/article/abs/pii/S0736584517303770?via%3Dihub)] OpenLMD, an open source middleware and toolkit for laser-based additive
manufacturing of large metal parts] [__`monitoring`__ __`DED`__ __`vision`__ __`control`__]  [__code (OpenLMD, ROS)__](https://github.com/openlmd), [dataset](https://zenodo.org/record/45664#.YgW-f99BxPY) :fire: :+1:

- [[IEEE Access (2021)](https://ieeexplore.ieee.org/document/9381862)] Improving Build Quality in Laser Powder Bed Fusion Using High Dynamic Range Imaging and Model-Based Reinforcement Learning] [__`reinforcement learning`__ __`CNN`__ __`LPBF`__ __`vision`__ __`surface defect (roughness)`__ __`Fraunhofer-Institute for Laser Technology`__] :+1:



---
### Thermal-based monitoring and inspections
- [[JMPT (2022)](https://www.sciencedirect.com/science/article/abs/pii/S0924013621004337)] Local prediction of Laser Powder Bed Fusion porosity by short-wave infrared imaging thermal feature porosity probability maps] [__`LPBF`__ __`thermal history`__ __`porosity`__ __`Missouri University of Science and Technology`__]  :+1:

- [[Npj Computational Materials (2021)](https://www.nature.com/articles/s41524-021-00555-z)] Mechanistic data-driven prediction of as-built mechanical properties in metal additive manufacturing] [__`DED`__ __`thermal history`__ __`UTS`__]  [__code(pytorch, CNN)__]( https://github.com/xiaoyuxie-vico/DL-AM), [__dataset__](https://github.com/xiaoyuxie-vico/DL_AM_Data) :fire: :+1:


- [[ASME J. Manuf. Sci. Eng. (2016)](https://asmedigitalcollection.asme.org/manufacturingscience/article-abstract/138/11/111007/454591/Predicting-Microstructure-From-Thermal-History)] Predicting Microstructure From Thermal History During Additive Manufacturing for Ti-6Al-4V] [__`DED`__ __`thermal history`__ __`Modelling`__ __`Simulation`__]  





---
### Point Cloud-based surface/geometric monitoring
- [[JMPT (2022)](https://doi.org/10.1016/j.jmatprotec.2021.117457)] Beyond parabolic weld bead models: AI-based 3D reconstruction of weld beads under transient conditions in wire-arc additive manufacturing
displacement and strain measurement] [__`monitoring`__ __`surface`__ __`planning`__]


---	
## Multimodal process monitoring

---	
## Closed loop feedback control	
- [[Lasers in Manufacturing and Materials Processing (2022)](https://www.sciencedirect.com.remotexs.ntu.edu.sg/science/article/pii/S277236902200010X)] Fabrication of Thin Walls with and without Close Loop
Control as a Function of Scan Strategy Via DED.] [__`control`__ __`DED`__]	
 

---	
## Process planning and path planning for AM and hybrid AM


- [[AM Letters (2022)](https://www.sciencedirect.com.remotexs.ntu.edu.sg/science/article/pii/S277236902200010X)] Process planning for additive manufacturing of geometries with variable overhang angles using a robotic laser DED system.] [__`planning`__ __`DED`__ __'University of Waterloo'__]

- [[VPP (2022)](https://www.tandfonline.com/doi/full/10.1080/17452759.2022.2031232?src=)] A spiral laser scanning routine for powder bed fusion inspired by natural predator-prey behaviour.] [__`planning`__ __`SLM`__ __`MIT`__]	


## Hybrid AM - material, process, systems
- [[VPP (2022)](https://www.tandfonline.com/doi/abs/10.1080/17452759.2022.2034081?src=&journalCode=nvpp20)] High-speed machining of additively manufactured Inconel 718 using hybrid cryogenic cooling methods] [__`hybridAM`__ __`DED`__  __`milling`__ __`material`__ __`CNC`__]

- [[Additive Manufacturing (2022)](https://www.sciencedirect.com/science/article/abs/pii/S2214860422000549)] Hybrid additive manufacturing (__DED__ + __ultrasonic
micro-forging treatment (UMT)__) for performance
improvement of martensitic stainless steel] [__`hybridAM`__ __`DED`__ __`material`__]

- [[VPP (2022)](https://www.tandfonline.com/doi/abs/10.1080/17452759.2022.2029009?src=&journalCode=nvpp20)] Investigation on synergism between additive and subtractive manufacturing for curved thin-walled structure,  multiple-cycle hybrid manufacturing (MCHM) vs. one-cycle hybrid manufacturing (OCHM) ] [__`hybridAM`__  __`thin-wall`__ __`process`__] 
 


##  Physics-informed machine learning for Additive Manufacturing

Alternative to the timely and costly FEM simulations of the thermal history in additive manufacturing.

- [[JMPT (2022)](https://www.sciencedirect.com/science/article/pii/S0924013621004325)] A generic physics-based machine learning model for geometry invariant thermal history prediction in additive manufacturing [__`Physics informed AI`__ __`process`__ __`geometry`__] [__code__](https://github.com/kariln/Predictions-of-thermal-fields-in-additive-manufacturing) [dataset](https://cutt.ly/QnqXV9Z) :fire:

- [[Computational Mechanics (2021)](https://www.sciencedirect.com/science/article/pii/S0924013621004325)]Machine learning for metal additive manufacturing: predicting temperature and melt pool fluid dynamics using physics-informed
neural networks[__`Physics informed AI`__ __`Thermal multiphase flows`__] [code and dataset](https://yan.cee.illinois.edu/) :fire:

