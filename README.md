# 📚 In-Situ Monitoring and Adaptive Control in Laser-based Additive Manufacturing [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

Welcome to this curated repository of **research papers with open-source codes/dataset** on *in‑situ process monitoring* and *adaptive process control* in laser-based additive manufacturing (AM). The goal is to highlight state-of-the-art approaches for ensuring **zero-defect, autonomous AM** through real-time sensing, data analysis, and control. We focus primarily on **Laser Powder Bed Fusion (LPBF)** and **Laser Directed Energy Deposition (LDED)**, with selective inclusion of **Wire Arc AM (WAAM)** and other processes where relevant. Contributions are welcome – see the guidelines below! 😊

Details of our comprehensive review paper published in 2024:
[In-situ process monitoring and adaptive quality enhancement in laser additive manufacturing: a critical review (2024)](https://ar5iv.org/pdf/2404.13673#:~:text=This%20paper%20provides%20a%20comprehensive,remediation%20strategies%20that%20advance%20LAM)

## Table of Contents

- [In-Situ Process Monitoring](#in-situ-process-monitoring-) 🔎
  - [Acoustic Signal-Based Monitoring](#acoustic-signal-based-monitoring-) 📢
  - [Vision-Based Monitoring](#vision-based-monitoring-) 📷
  - [Thermal/Infrared Monitoring](#thermalinfrared-monitoring-) 🌡️
  - [Surface Topography / Point Cloud Monitoring](#surface-topography--point-cloud-monitoring-) 🛰️
  - [Multisensor & Data Fusion](#multisensor--data-fusion-) 🧩
- [Adaptive Process Control](#adaptive-process-control-) 🕹️
- [Simulation for Process Optimization](#simulation-for-process-optimization-) 🖥️
- [Hybrid Additive-Subtractive Manufacturing](#hybrid-additive-subtractive-manufacturing-) ⚙️
- [Physics-Informed Machine Learning for AM](#physics-informed-machine-learning-) 🧠
- [AM Robotic Path Planning](#am-robotic-path-planning-) 🤖
- [Contributing](#-contributing)
- [License](#-license)

---

## In-Situ Process Monitoring 🔎

Real-time monitoring is crucial for defect detection and quality assurance. Below, we categorize monitoring approaches by the primary sensing modality:

### Acoustic Signal-Based Monitoring 📢

High-frequency acoustic emissions can reveal melt pool instabilities and defect formation. Researchers are using microphones or piezoelectric sensors to capture sound from the process and applying ML for anomaly detection.

| Title (and Link) | Code 💻 | Dataset 📂 | Process | Tags | Year |
|------------------|---------|------------|---------|------|------|
| [Optimizing In‑Situ Monitoring for LPBF: Deciphering Acoustic Emission and Sensor Sensitivity with Explainable ML](https://github.com/vigneashpandiyan/Additive-Manufacturing-Sensor-Selection-Acoustic-Emission) <br> *V. Pandiyan et al.* (J. Mat. Proc. Tech.) | [GitHub](https://github.com/vigneashpandiyan/Additive-Manufacturing-Sensor-Selection-Acoustic-Emission) | *N/A* | LPBF | `ExplainableML` `EMD` `FrequencyAnalysis` | 2023 |
| [Deep Transfer Learning of AM Mechanisms Across Materials in LPBF](https://www.sciencedirect.com/science/article/pii/S0924013622000437) <br> *V. Pandiyan et al.* (J. Mat. Proc. Tech.) | [GitHub](https://c4science.ch/diffusion/11778/) | ✅ | LPBF | `TransferLearning` `PyTorch` `CrossMaterial` | 2022 |
| [Semi-supervised Monitoring of LPBF Based on Acoustic Emissions](https://www.tandfonline.com/doi/abs/10.1080/17452759.2021.1966166) <br> *V. Pandiyan et al.* (Virtual Phys. Prototyp.) | [GitHub](https://c4science.ch/diffusion/11519/) | *N/A* | LPBF | `SemiSupervised` `PyTorch` `AnomalyDetection` | 2021 |
| [In-Situ Alloying of Titanium-Fe: Acoustic Dynamics and Process Signatures](https://www.sciencedirect.com/science/article/pii/S0264127522009790) <br> *V. Pandiyan et al.* | [GitHub](https://github.com/vigneashpandiyan/Additive-Manufacturing-Acoustic-Dynamics-of-in-situ-alloying-of-Titanium-Fe) | *N/A* | LPBF | `In-situAlloying` `AcousticFingerprinting` `Ti-Fe` | 2023 |
| [Feature Engineering for AM Acoustic Emission Monitoring](https://www.sciencedirect.com/science/article/pii/S2212827120313408) <br> *V. Pandiyan et al.* (Procedia CIRP) | [GitHub](https://github.com/vigneashpandiyan/Additive-Manufacturing-Feature-Engineering-Acoustic-Emission) | *N/A* | LPBF | `FeatureEngineering` `WaveletTransform` `RealTime` | 2021 |
| [Linking Acoustic Emission Signatures to Material Properties in AM](https://www.tandfonline.com/doi/full/10.1080/17452759.2022.2028380) <br> *V. Pandiyan et al.* (Virtual Phys. Prototyp.) | [GitHub](https://github.com/vigneashpandiyan/Additive-Manufacturing-Feature-Engineering-Acoustic-Emission) | *N/A* | LPBF | `MaterialFingerprinting` `FeatureSelection` | 2022 |
| [Self-Supervised Bayesian Representation Learning for Acoustic Monitoring in AM](https://www.sciencedirect.com/science/article/pii/S0959652622041081) <br> *V. Pandiyan et al.* | [GitHub](https://github.com/vigneashpandiyan/Additive-Manufacturing-Self-Supervised-Bayesian-Representation-Learning-Acoustic-Emission) | *N/A* | LPBF | `SelfSupervised` `BayesianLearning` `Representation` | 2022 |
| [Domain Adaptation for Bridging Dissimilar Process Maps Using Acoustic Signals](https://www.sciencedirect.com/science/article/pii/S0924013622000322) <br> *V. Pandiyan et al.* | [GitHub](https://github.com/vigneashpandiyan/Additive-Manufacturing-Domain-adaptation-for-Bridging-Dissimilar-Process-Maps-Acoustic-Emission) | *N/A* | LPBF | `DomainAdaptation` `ProcessMaps` `CrossMaterial` | 2022 |
| [Semi-Supervised Acoustic Monitoring for LPBF](https://www.sciencedirect.com/science/article/pii/S2214860421005108) <br> *V. Pandiyan et al.* | [GitHub](https://github.com/vigneashpandiyan/Additive-Manufacturing-Acoustics-Semisupervised-Learning) | *N/A* | LPBF | `SemiSupervised` `AnomalyDetection` `RealTime` | 2021 |

### Vision-Based Monitoring 📷

Optical monitoring uses cameras (visible or infrared) to observe the melt pool, spatter, and layer morphology in real-time. High-speed imaging and computer vision techniques can detect anomalies like pores or lack-of-fusion. Some works also release open datasets for benchmarking.

| Title (and Link) | Code 💻 | Dataset 📂 | Process | Tags | Year |
|------------------|---------|------------|---------|------|------|
| [RAISE-LPBF: Reference Dataset & Benchmark for Reconstructing Laser Parameters from On-Axis Video](https://arxiv.org/html/2409.12475v1) <br> *C. Blanc et al.* (Addit. Manuf. Lett.) | [GitHub](https://github.com/Flanders-Make-vzw/RAISE_LPBF_Laser_benchmark) | [Website](https://www.makebench.eu) | LPBF | `HighSpeedImaging` `LaserParameters` `Benchmark` | 2023 |
| [Dataset of In‑Situ Coaxial Monitoring and Print's Cross-Section Images](https://doi.org/10.1038/s41597-023-02672-4) <br> *J. Akhavan et al.* (Sci. Data) | *N/A* | [Data](https://doi.org/10.1038/s41597-023-02672-4) | LDED | `CoaxialVision` `CrossSection` `OpenAccess` | 2023 |
| [Real-Time Monitoring & Quality Assurance for L-DED via Coaxial Imaging + Self-Supervised Learning](https://link.springer.com/article/10.1007/s10845-023-02279-x) <br> *V. Pandiyan et al.* (J. Intell. Manuf.) | [GitHub](https://github.com/vigneashpandiyan/Additive-Manufacturing-Self-Supervised-Learning-Coaxial-DED-Process-Zone-Imaging) | *Available on request* | LDED | `SelfSupervised` `CoaxialImaging` `QualityAssurance` | 2023 |
| [Deep DIC: Deep Learning-Based Digital Image Correlation for End-to-End Displacement and Strain Measurement](https://www.sciencedirect.com/science/article/abs/pii/S0924013621004349) <br> *R. Yang et al.* (J. Mat. Proc. Tech.) | [GitHub](https://github.com/RuYangNU/Deep-Dic-deep-learning-based-digital-image-correlation) | [Drive](https://drive.google.com/drive/folders/1n2axHsJ3flHxk_edceY6eOfiX7GjW_d6) | Various | `DIC` `DeepLearning` `StrainMeasurement` | 2022 |
| [Surface Defect Detection in AM Using Deep Learning](https://www.tandfonline.com/doi/full/10.1080/17452759.2020.1832695) <br> *D. Chen et al.* (Virtual and Physical Prototyping) | [GitHub](https://github.com/Davidlequnchen/AM_Surface_Defect) | *N/A* | Various | `SurfaceDefect` `ComputerVision` `DeepLearning` | 2020 |
| [Manifold Learning for Process Zone Characterization in DED](https://www.sciencedirect.com/science/article/pii/S0890695523001645) <br> *V. Pandiyan et al.* | [GitHub](https://github.com/vigneashpandiyan/Additive-Manufacturing-DED-Manifold-Learning) | *N/A* | DED | `ManifoldLearning` `Dimensionality` `ProcessZone` | 2023 |
| [Contrastive Learning for DED Process Monitoring](https://www.sciencedirect.com/science/article/pii/S2214860422003530) <br> *V. Pandiyan et al.* | [GitHub](https://github.com/vigneashpandiyan/Additive-Manufacturing-DED-Contrastive-Learners) | *N/A* | DED | `ContrastiveLearning` `SelfSupervised` `ProcessAnalysis` | 2022 |


### Thermal/Infrared Monitoring 🌡️

Infrared cameras and pyrometers capture thermal signatures (melt pool temperature, cooling rates, etc.) for defect detection. Thermal monitoring can reveal anomalies like overheating, lack of fusion, or excessive cooling that correlate with defects.

| Title (and Link) | Code 💻 | Dataset 📂 | Process | Tags | Year |
|------------------|---------|------------|---------|------|------|
| [In‑Situ Infrared Camera Monitoring for Defect & Anomaly Detection](http://arxiv.org/pdf/2407.12682) <br> *S. Hinnebusch et al.* (arXiv preprint) | *Python snippets* | *N/A* | LPBF | `FeatureExtraction` `AnomalyDetection` `ThermalSignatures` | 2024 |
| [Mechanistic Data-Driven Prediction of As-Built Mechanical Properties in Metal AM](https://www.nature.com/articles/s41524-021-00555-z) <br> *X. Xie et al.* (Npj Comput. Mater.) | [GitHub](https://github.com/xiaoyuxie-vico/DL-AM) | [GitHub](https://github.com/xiaoyuxie-vico/DL_AM_Data) | DED | `ThermalHistory` `CNN` `MechanicalProperties` | 2021 |

### Surface Topography / Point Cloud Monitoring 🛰️

Structured-light scanning, fringe projection, and 3D reconstruction techniques monitor the geometry of each layer. These produce **point clouds** or height maps to detect warping, recoater interference, or surface roughness issues.

| Title (and Link) | Code 💻 | Dataset 📂 | Process | Tags | Year |
|------------------|---------|------------|---------|------|------|
| [In‑Situ Surface Topography of LPBF Using Fringe Projection](http://www.euspen.eu/knowledge-base/AM23134.pdf) <br> *B. Zhang et al.* (Addit. Manuf.) | *N/A* | *N/A* | LPBF | `FringeProjection` `SurfaceMonitoring` `Topography` | 2016 |
| [Etna: On-line 3D Monitoring for Robotized LMD](https://github.com/openlmd/etna) <br> *AIMEN OpenLMD Toolkit* (Open-Source Project) | [GitHub](https://github.com/openlmd/etna) | *N/A* | LMD | `3DScan` `RealTime` `Robotized` | 2017 |

### Multisensor & Data Fusion 🧩

Combining multiple sensors (e.g., optical, acoustic, thermal) can provide a richer picture of the process. Multisensor approaches often leverage machine learning to fuse data and detect defects more reliably, sometimes using ground truth from X-ray or CT for validation.

| Title (and Link) | Code 💻 | Dataset 📂 | Process | Tags | Year |
|------------------|---------|------------|---------|------|------|
| [Deep Learning Monitoring of LPBF with Heterogeneous Sensing and X-Ray Guidance](https://infoscience.epfl.ch/entities/publication/2ce72bb3-eeca-4099-9325-ce061bfa2e55) <br> *V. Pandiyan et al.* (Addit. Manuf.) | [GitHub](https://github.com/vigneashpandiyan/Additive-Manufacturing-Variable-Time-Scales) | [Zenodo](https://doi.org/10.5281/zenodo.6339430) | LPBF | `Multisensor` `XRay` `VariableTimeScales` | 2022 |
| [Multi-Material Composition Monitoring Using Sensor Fusion in LPBF](https://www.sciencedirect.com/science/article/pii/S2214860421001718) <br> *V. Pandiyan et al.* | [GitHub](https://github.com/vigneashpandiyan/Additive-Manufacturing-Multi-Material-Composition-Monitoring-Using-Sensor-Fusion) | *N/A* | LPBF | `SensorFusion` `MultiMaterial` `CompositionMonitoring` | 2021 |
| [MultiSensor Fusion for ROS-Based AM Monitoring](https://www.sciencedirect.com/science/article/abs/pii/S0736584523000571) <br> *L. Chen et al.* (Robotics and CIM) | [GitHub](https://github.com/Davidlequnchen/MultiSensorFusion-ROS-AM-Monitoring) | *N/A* | Various | `ROS` `Robotics` `SensorFusion` | 2023 |
| [MultiSensor Monitoring for Laser Wire DED](https://github.com/Davidlequnchen/MultiSensor-Monitoring-LW-DED) <br> *L. Chen et al.* | [GitHub](https://github.com/Davidlequnchen/MultiSensor-Monitoring-LW-DED) | *N/A* | LW-DED | `MultiSensor` `WireFeed` `ProcessMonitoring` | 2023 |

## Adaptive Process Control 🕹️

Adaptive control closes the loop by adjusting process parameters in real-time based on sensor feedback. The aim is to correct defects on-the-fly – for example, modulating laser power or scan speed to maintain a stable melt pool and avoid flaws, driving AM toward autonomous operation.

| Title (and Link) | Code 💻 | Dataset 📂 | Process | Tags | Year |
|------------------|---------|------------|---------|------|------|
| [CladPlus: Closed-Loop Control for Laser Cladding](https://openlmd.github.io/cladplus.html) <br> *AIMEN OpenLMD Toolkit* (Open-Source Project) | [GitHub](https://github.com/openlmd/cladplus) | *N/A* | LDED | `ClosedLoop` `LaserCladding` `InfraredControl` | 2017 |


## Simulation for Design and Process Optimization 🖥️

Physics-based simulations (thermal, mechanical, microstructural) help predict outcomes of process parameters and optimize them without costly trial-and-error. Open-source tools and multi-physics models are enabling **"digital twins"** of AM processes.

| Title (and Link) | Code 💻 | Dataset 📂 | Process | Tags | Year |
|------------------|---------|------------|---------|------|------|
| [JAX-AM: Differentiable Simulation Toolkit for Additive Manufacturing](https://github.com/tianjuxue/jax-am) <br> *T. Xue et al.* (Open-Source Project) | [GitHub](https://github.com/tianjuxue/jax-am) | *N/A* | *Multi (LPBF/DED)* | `Differentiable` `GPU-Accelerated` `JAX` | 2023 |
| [Graph-Based Modeling for Additive Manufacturing](https://github.com/AMPL-NU/Graph_AM_Modeling) <br> *AMPL Research Group* | [GitHub](https://github.com/AMPL-NU/Graph_AM_Modeling) | *N/A* | Various | `GraphModels` `GNN` `ProcessModeling` | 2023 |


## Hybrid Additive-Subtractive Manufacturing ⚙️

Hybrid processes combine **additive** (build-up) and **subtractive** (machining) steps in the same workflow or machine. This addresses limitations of AM (e.g., surface finish, accuracy) by machining critical surfaces or features either intermittently during the build or post-build. Research in this area includes machine tool integration and strategic toolpath planning for when to print vs. mill.

| Title (and Link) | Code 💻 | Dataset 📂 | Process | Tags | Year |
|------------------|---------|------------|---------|------|------|
| [Hybrid Additive-Subtractive Manufacturing Using Pulsed Arc Plasma](https://www.mdpi.com/1996-1944/16/13/4809) <br> *X. Duan et al.* (Materials) | *N/A* | *N/A* | PAP (Arc DED) | `HybridManufacturing` `PulsedArc` `Milling` | 2023 |

## 4D Printing & Advanced Materials 🧪

4D printing adds the dimension of time to 3D printing, enabling printed parts to change shape, properties, or function in response to external stimuli. Research in this area combines advanced materials, simulation, and AI to design transformable structures.

| Title (and Link) | Code 💻 | Dataset 📂 | Process | Tags | Year |
|------------------|---------|------------|---------|------|------|
| [AI-Assisted Material Design for 4D Printing](https://www.sciencedirect.com/science/article/pii/S2667369722000103) <br> *L. Chen et al.* | [GitHub](https://github.com/Davidlequnchen/AI-assisted-material-design-for-4D-printing) | *N/A* | 4DP | `MaterialDesign` `AI` `ShapeMemory` | 2022 |


## Physics-Informed Machine Learning 🧠

Physics-informed ML integrates fundamental physics (conservation laws, constitutive models, etc.) into data-driven models. In AM, this can mean using simulation data to train ML models, constraining neural nets with physical laws, or creating surrogate models that are faster than physics simulators but more accurate than black-box ML alone.

| Title (and Link) | Code 💻 | Dataset 📂 | Process | Tags | Year |
|------------------|---------|------------|---------|------|------|
| [Physics-Embedded Graph Network for Accelerating Metal Microstructure Simulation](https://github.com/tianjuxue/jax-am) <br> *T. Xue et al.* (NPJ Comput. Mater.) | [GitHub](https://github.com/tianjuxue/jax-am) | *Synthetic* | LPBF (Ti64) | `GraphNetwork` `PhaseField` `Microstructure` | 2022 |
| [A Physics-Informed CNN with Custom Loss Functions for Porosity Prediction in LMD](https://doi.org/10.3390/s22020494) <br> *P. Hagqvist et al.* (Sensors) | *N/A* | [Harvard Dataverse](https://dataverse.harvard.edu/dataset.xhtml?persistentId=doi:10.7910/DVN/AHYXL9) | LMD | `CustomLoss` `CNN` `Porosity` | 2022 |
| [Generic Physics-Based ML Model for Geometry-Invariant Thermal History Prediction in AM](https://www.sciencedirect.com/science/article/pii/S0924013621004325) <br> *K. Nygård et al.* (J. Mat. Proc. Tech.) | [GitHub](https://github.com/kariln/Predictions-of-thermal-fields-in-additive-manufacturing) | [Dataset](https://cutt.ly/QnqXV9Z) | Various | `GeometryInvariant` `ThermalHistory` `FEM` | 2022 |
| [Physics-Driven Deep Learning Model for Process-Porosity Causal Relationship in LMD](https://www.sciencedirect.com/science/article/pii/S0007850620300718) <br> *X. Xie et al.* (CIRP Annals) | *N/A* | [Harvard Dataverse](https://dataverse.harvard.edu/dataset.xhtml?persistentId=doi:10.7910/DVN/AHYXL9) | LMD | `Interpretability` `Causality` `Porosity` | 2021 |
| [ML for Metal AM: Predicting Temperature and Melt Pool Dynamics using Physics-Informed Neural Networks](https://www.sciencedirect.com/science/article/pii/S0924013621004325) <br> *Y. Yang et al.* (Computational Mechanics) | [Website](https://yan.cee.illinois.edu/) | ✅ | Various | `PINN` `MultiphaseFlow` `ThermalModeling` | 2021 |
| [Physics-Informed Neural Network for AM Thermal-Mechanical Multi-Physics Process](https://link.springer.com/article/10.1007/s00466-022-02257-9) <br> *S. Liao et al.* (Computational Mechanics) | [GitHub](https://github.com/ShuhengLiao/Physics_informed_AM) | [Drive](https://drive.google.com/file/d/1P6RqrbRW3mptzKd4LDoUrHFopBp7AfzV/view) | Various | `PINN` `ThermalMechanical` `MultiPhysics` | 2022 |
| [Machine Learning for Iterative Prediction of Build Quality in Metal AM](https://www.mdpi.com/2075-4701/12/9/1441) <br> *Y. Hidaka et al.* (Metals) | [GitHub](https://github.com/NU-CUCIS/ml-iter-additive) | *N/A* | LPBF | `IterativePrediction` `BuildQuality` `XCT` | 2022 |
| [Differentiable Simulation for Additive Manufacturing](https://arxiv.org/abs/2211.12654) <br> *M. Mozaffar et al.* (arXiv) | [GitHub](https://github.com/mojtabamozaffar/differentiable-simulation-am) | *N/A* | Various | `DifferentiableSimulation` `AutoDiff` `Optimization` | 2022 |


## AM Robotic Path Planning 🤖

Path planning is crucial for directed-energy AM processes (LDED, WAAM, etc.), especially with multi-axis robots. Efficient algorithms are needed to determine the deposition toolpath that ensures uniform material deposition, avoids collisions, and can handle complex geometries or repairs.

| Title (and Link) | Code 💻 | Dataset 📂 | Process | Tags | Year |
|------------------|---------|------------|---------|------|------|
| [RobPath: Off‑Line Path Planning Tool for LMD Automation](https://github.com/openlmd/robpath) <br> *AIMEN OpenLMD Toolkit* (Open-Source Project) | [GitHub](https://github.com/openlmd/robpath) | *N/A* | LMD | `ToolpathGeneration` `Robotics` `CAD-Based` | 2020 |
| [KUKA-ROS Based Advanced Motion Planning for Additive Manufacturing](https://www.sciencedirect.com/science/article/abs/pii/S0924013622000565) <br> *D. Chen et al.* (J. Mat. Proc. Tech.) | [GitHub](https://github.com/Davidlequnchen/KUKA-ROS-AM-Advanced-Motion-Planning) | *N/A* | Various | `KUKA` `ROS` `MotionPlanning` | 2022 |
| [Toolpath Design for AM Using Reinforcement Learning](https://www.sciencedirect.com/science/article/pii/S2214860422000252) <br> *M. Mozaffar et al.* | [GitHub](https://github.com/mojtabamozaffar/toolpath-design-rl) | *N/A* | FDM/Various | `ReinforcementLearning` `ToolpathOptimization` | 2022 |

---

## 🤝 Contributing

We welcome contributions from the community! Please feel free to **suggest a paper** or **add a new entry** via Pull Request. To maintain consistency, please follow these guidelines:

- **Scope**: Ensure the paper is relevant to *in-situ monitoring or adaptive control* in AM (or closely related, like simulation or hybrid processes). Laser-based metal AM is the focus, but notable work in other AM or sensing modalities can be included if it fits a category.
- **Table Format**: Use the same table structure: Title (with link to paper), Code (link if available), Dataset (link if available), Process type, Tags, and Year. Indicate *N/A* if code or data are not available. 
- **Tags**: Use descriptive tags in backticks like `` `ExplainableML` ``. Aim for 2-4 tags that capture the work's key aspects, focusing on methods, algorithms, or specific techniques rather than general categories already covered by the section.
- **Style**: Keep descriptions concise. You can add a short note below a table if needed to explain context or significance (as done above). Use present tense and clear language.
- **Attribution**: Include the first author's last name or an obvious short reference in the Title field for clarity. If the paper is open access, you can note that in tags or the title (e.g., via journal or a 🔓 emoji).

By contributing, you agree to abide by the repo's [Code of Conduct](CODE_OF_CONDUCT.md) and ensure information is accurate. Let's build a comprehensive knowledge base for the AM community! 🤖🔥

## 📜 License

All content in this repository is released under the [MIT License](LICENSE), and the respective papers are copyright their publishers/authors. This list is for educational and research purposes, inspired by open-source community efforts.

<hr>

*Happy Printing & Processing!* 🚀 Feel free to open an issue for any questions or discussions.
