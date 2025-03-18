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
- [Physics-Informed Machine Learning for AM](#physics-informed-machine-learning-) 🧠
- [AM Robotic Path Planning](#am-robotic-path-planning-) 🤖
- [AI-assisted Design of Advanced Materials](###advanced-materials-) 🧪
- [Contributing](#-contributing)
- [License](#-license)

---

## In-Situ Process Monitoring 🔎

Real-time monitoring is crucial for defect detection and quality assurance. Below, we categorize monitoring approaches by the primary sensing modality:

### Acoustic Signal-Based Monitoring 📢

High-frequency acoustic emissions can reveal melt pool instabilities and defect formation. Researchers are using microphones or piezoelectric sensors to capture sound from the process and applying ML for anomaly detection.

| Title (and Link) | Code 💻 | Dataset 📂 | Process | Tags | Year |
|------------------|---------|------------|---------|------|------|
| [Optimizing In‑Situ Monitoring for LPBF: Deciphering Acoustic Emission and Sensor Sensitivity with Explainable ML](https://www.sciencedirect.com/science/article/pii/S0924013623002893?via%3Dihub) <br> *V. Pandiyan et al.* (J. Mat. Proc. Tech.) | [GitHub](https://github.com/vigneashpandiyan/Additive-Manufacturing-Sensor-Selection-Acoustic-Emission) | [Dataset](https://github.com/vigneashpandiyan/Additive-Manufacturing-Sensor-Selection-Acoustic-Emission) | LPBF | `ExplainableML` `EMD` `FrequencyAnalysis` | 2023 |
| [In-Situ Alloying of Titanium-Fe: Acoustic Dynamics and Process Signatures](https://www.sciencedirect.com/science/article/pii/S0264127522009790) <br> *V. Pandiyan et al.* | [GitHub](https://github.com/vigneashpandiyan/Additive-Manufacturing-Acoustic-Dynamics-of-in-situ-alloying-of-Titanium-Fe) | *N/A* | LPBF | `In-situAlloying` `AcousticFingerprinting` `Ti-Fe` | 2023 |
| [Deep Transfer Learning of AM Mechanisms Across Materials in LPBF](https://www.sciencedirect.com/science/article/pii/S0924013622000437) <br> *V. Pandiyan et al.* (J. Mat. Proc. Tech.) | [GitHub](https://github.com/vigneashpandiyan/Additive-Manufacturing-Transfer-Learning) | N.A. | LPBF | `TransferLearning` `PyTorch` `CrossMaterial` | 2022 |
| [Linking Acoustic Emission Signatures to Material Properties in AM](https://www.tandfonline.com/doi/full/10.1080/17452759.2022.2028380) <br> *V. Pandiyan et al.* (Virtual Phys. Prototyp.) | [GitHub](https://github.com/vigneashpandiyan/Additive-Manufacturing-Feature-Engineering-Acoustic-Emission) | *N/A* | LPBF | `MaterialFingerprinting` `FeatureSelection` | 2022 |
| [Self-Supervised Bayesian Representation Learning for Acoustic Monitoring in AM](https://www.sciencedirect.com/science/article/pii/S0264127523008730?via%3Dihub) <br> *V. Pandiyan et al. (Materials & Design)* | [GitHub](https://github.com/vigneashpandiyan/Additive-Manufacturing-Self-Supervised-Bayesian-Representation-Learning-Acoustic-Emission) | *N/A* | LPBF | `SelfSupervised` `BayesianLearning` `Representation` | 2022 |
| [Domain Adaptation for Bridging Dissimilar Process Maps Using Acoustic Signals](https://www.sciencedirect.com/science/article/pii/S2214860424000204?via%3Dihub) <br> *V. Pandiyan et al. (Additive Manufacturing)* | [GitHub](https://github.com/vigneashpandiyan/Additive-Manufacturing-Domain-adaptation-for-Bridging-Dissimilar-Process-Maps-Acoustic-Emission) | *N/A* | LPBF | `DomainAdaptation` `ProcessMaps` `CrossMaterial` | 2022 |
| [Feature Engineering for AM Acoustic Emission Monitoring](https://www.sciencedirect.com/science/article/pii/S2212827120313408) <br> *V. Pandiyan et al.* (Procedia CIRP) | [GitHub](https://github.com/vigneashpandiyan/Additive-Manufacturing-Feature-Engineering-Acoustic-Emission) | *N/A* | LPBF | `FeatureEngineering` `WaveletTransform` `RealTime` | 2021 |
| [Semi-supervised Monitoring of LPBF Based on Acoustic Emissions](https://www.tandfonline.com/doi/abs/10.1080/17452759.2021.1966166) <br> *V. Pandiyan et al.* (Virtual Phys. Prototyp.) | [GitHub](https://github.com/vigneashpandiyan/Additive-Manufacturing-Acoustics-Semisupervised-Learning) | *N/A* | LPBF | `SemiSupervised` `PyTorch` `AnomalyDetection` | 2021 |

### Vision-Based Monitoring 📷

Optical monitoring uses cameras (visible or infrared) to observe the melt pool, spatter, and layer morphology in real-time. High-speed imaging and computer vision techniques can detect anomalies like pores or lack-of-fusion. Some works also release open datasets for benchmarking.

| Title (and Link) | Code 💻 | Dataset 📂 | Process | Tags | Year |
|------------------|---------|------------|---------|------|------|
| [RAISE-LPBF: Reference Dataset & Benchmark for Reconstructing Laser Parameters from On-Axis Video](https://arxiv.org/html/2409.12475v1) <br> *C. Blanc et al.* | [GitHub](https://github.com/Flanders-Make-vzw/RAISE_LPBF_Laser_benchmark) | [Website](https://www.makebench.eu) | LPBF | `HighSpeedImaging` `LaserParameters` `Benchmark` | 2023 |
| [Dataset of In‑Situ Coaxial Monitoring and Print's Cross-Section Images](https://doi.org/10.1038/s41597-023-02672-4) <br> *J. Akhavan et al.* (Sci. Data) | *N/A* | [Data](https://doi.org/10.1038/s41597-023-02672-4) | LDED | `CoaxialVision` `CrossSection` `OpenAccess` | 2023 |
| [Real-Time Monitoring & Quality Assurance for L-DED via Coaxial Imaging + Self-Supervised Learning](https://link.springer.com/article/10.1007/s10845-023-02279-x) <br> *V. Pandiyan et al.* (J. Intell. Manuf.) | [GitHub](https://github.com/vigneashpandiyan/Additive-Manufacturing-Self-Supervised-Learning-Coaxial-DED-Process-Zone-Imaging) | *N/A* | LDED | `SelfSupervised` `CoaxialImaging` `QualityAssurance` | 2023 |
| [Manifold Learning for Process Zone Characterization in DED](https://www.sciencedirect.com/science/article/pii/S2213846322001274?via%3Dihub) <br> *V. Pandiyan et al. (Manufacturing Letters)* | [GitHub](https://github.com/vigneashpandiyan/Additive-Manufacturing-DED-Manifold-Learning) | *N/A* | DED | `ManifoldLearning` `Dimensionality` `ProcessZone` | 2022 |
| [Contrastive Learning for DED Process Monitoring](https://www.sciencedirect.com/science/article/pii/S1526612522004996?via%3Dihub) <br> *V. Pandiyan et al. (Journal of Manufacturing Processes)* | [GitHub](https://github.com/vigneashpandiyan/Additive-Manufacturing-DED-Contrastive-Learners) | *N/A* | DED | `ContrastiveLearning` `SelfSupervised` `ProcessAnalysis` | 2022 |
| [Deep DIC: Deep Learning-Based Digital Image Correlation for End-to-End Displacement and Strain Measurement](https://www.sciencedirect.com/science/article/abs/pii/S0924013621004349) <br> *R. Yang et al.* (J. Mat. Proc. Tech.) | [GitHub](https://github.com/RuYangNU/Deep-Dic-deep-learning-based-digital-image-correlation) | [Drive](https://drive.google.com/drive/folders/1n2axHsJ3flHxk_edceY6eOfiX7GjW_d6) | Various | `DIC` `DeepLearning` `StrainMeasurement` | 2022 |



### Thermal/Infrared Monitoring 🌡️

Infrared cameras and pyrometers capture thermal signatures (melt pool temperature, cooling rates, etc.) for defect detection. Thermal monitoring can reveal anomalies like overheating, lack of fusion, or excessive cooling that correlate with defects.

| Title (and Link) | Code 💻 | Dataset 📂 | Process | Tags | Year |
|------------------|---------|------------|---------|------|------|
| [In‑Situ Infrared Camera Monitoring for Defect & Anomaly Detection](http://arxiv.org/pdf/2407.12682) <br> *S. Hinnebusch et al.* (arXiv preprint) | *Python snippets* | *N/A* | LPBF | `FeatureExtraction` `AnomalyDetection` `ThermalSignatures` | 2024 |


### Surface Topography / Point Cloud Monitoring 🛰️

Structured-light scanning, fringe projection, and 3D reconstruction techniques monitor the geometry of each layer. These produce **point clouds** or height maps to detect warping, recoater interference, or surface roughness issues.

| Title (and Link) | Code 💻 | Dataset 📂 | Process | Tags | Year |
|------------------|---------|------------|---------|------|------|
| [Surface Defect Detection in AM Using Deep Learning](https://www.tandfonline.com/doi/full/10.1080/17452759.2020.1832695) <br> *L. Chen et al.* (Virtual and Physical Prototyping) | [GitHub](https://github.com/Davidlequnchen/AM_Surface_Defect) | *N/A* | LDED | `SurfaceDefect` `ComputerVision` `DeepLearning` | 2020 |
| [Etna: On-line 3D Monitoring for Robotized LMD](https://github.com/openlmd/etna) <br> *AIMEN OpenLMD Toolkit* (Open-Source Project) | [GitHub](https://github.com/openlmd/etna) | *N/A* | LDED | `3DScan` `RealTime` `Robotized` | 2017 |

### Multisensor & Data Fusion 🧩

Combining multiple sensors (e.g., optical, acoustic, thermal) can provide a richer picture of the process. Multisensor approaches often leverage machine learning to fuse data and detect defects more reliably, sometimes using ground truth from X-ray or CT for validation.

| Title (and Link) | Code 💻 | Dataset 📂 | Process | Tags | Year |
|------------------|---------|------------|---------|------|------|
| [Audio-Visual Cross-Modality Knowledge Transfer for ML-Based In-Situ Monitoring in Laser AM](https://www.sciencedirect.com/science/article/abs/pii/S2214860425000569) <br> *V. Pandiyan et al.* (Additive Manufacturing) | *N/A* | [Zenodo](https://zenodo.org/records/12604782) | LDED | `CrossModality` `AudioVisual` `KnowledgeTransfer` | 2025 |
| [Deep Learning Monitoring of LPBF with Heterogeneous Sensing and X-Ray Guidance](https://www.sciencedirect.com/science/article/pii/S2214860422004006) <br> *V. Pandiyan et al.* (Addit. Manuf.) | [GitHub](https://github.com/vigneashpandiyan/Additive-Manufacturing-Variable-Time-Scales) | N.A. | LPBF | `Multisensor` `XRay` `VariableTimeScales` | 2022 |
| [Multi-Material Composition Monitoring Using Sensor Fusion in LPBF](https://www.tandfonline.com/doi/full/10.1080/17452759.2024.2356080) <br> *V. Pandiyan et al.* | [GitHub](https://github.com/vigneashpandiyan/Additive-Manufacturing-Multi-Material-Composition-Monitoring-Using-Sensor-Fusion) | *N/A* | LPBF | `SensorFusion` `MultiMaterial` `CompositionMonitoring` | 2021 |
| [MultiSensor Fusion for ROS-Based AM Monitoring](https://www.sciencedirect.com/science/article/abs/pii/S0736584523000571) <br> *L. Chen et al.* (Robotics and CIM) | [GitHub](https://github.com/Davidlequnchen/MultiSensorFusion-ROS-AM-Monitoring) | *N/A* | LDED | `ROS` `Robotics` `SensorFusion` | 2023 |
| [MultiSensor Monitoring for Laser Wire DED](https://github.com/Davidlequnchen/MultiSensor-Monitoring-LW-DED) <br> *L. Chen et al.* | [GitHub](https://github.com/Davidlequnchen/MultiSensor-Monitoring-LW-DED) | *N/A* | LW-DED | `MultiSensor` `WireFeed` `ProcessMonitoring` | 2023 |

## Adaptive Process Control 🕹️

Adaptive control closes the loop by adjusting process parameters in real-time based on sensor feedback. The aim is to correct defects on-the-fly – for example, modulating laser power or scan speed to maintain a stable melt pool and avoid flaws, driving AM toward autonomous operation.

| Title (and Link) | Code 💻 | Dataset 📂 | Process | Tags | Year |
|------------------|---------|------------|---------|------|------|
| [CladPlus: Closed-Loop Control for Laser Cladding](https://openlmd.github.io/cladplus.html) <br> *AIMEN OpenLMD Toolkit* (Open-Source Project), [OpenLMD, an open source middleware and toolkit](https://www.sciencedirect.com/science/article/abs/pii/S0736584517303770) (García-Díaz et al. RCIM) | [GitHub](https://github.com/openlmd/cladplus)  | *N/A* | LDED | `ClosedLoop` `LaserCladding` `InfraredControl` | 2017 |
| [Data-Driven Adaptive Control for Laser-Based AM with Automatic Controller Tuning](https://www.mdpi.com/2076-3417/10/22/7967) <br> *L. Chen et al.* (Applied Sciences) | [GitHub](https://github.com/Davidlequnchen/laam_control_ws) | *N/A* | LDED | `AdaptiveControl` `AutoTuning` `ClosedLoop` `RealTime` | 2020 |

## Simulation for Design and Process Optimization 🖥️

Physics-based simulations (thermal, mechanical, microstructural) help predict outcomes of process parameters and optimize them without costly trial-and-error. Open-source tools and multi-physics models are enabling **"digital twins"** of AM processes.

| Title (and Link) | Code 💻 | Dataset 📂 | Process | Tags | Year |
|------------------|---------|------------|---------|------|------|
| [JAX-AM: Differentiable Simulation Toolkit for Additive Manufacturing](https://github.com/tianjuxue/jax-am) <br> *T. Xue et al.* (Open-Source Project) | [GitHub](https://github.com/tianjuxue/jax-am) | *N/A* | *Multi (LPBF/DED)* | `Differentiable` `GPU-Accelerated` `JAX` | 2023 |
| [Efficient GPU-accelerated Thermomechanical Solver for Residual Stress Prediction in AM](https://link.springer.com/article/10.1007/s00466-023-02273-3) <br> *S. Liao et al.* (Computational Mechanics) | [GitHub](https://github.com/ShuhengLiao/AM_Thermomechanical_Solver) | *N/A* | LDED/LPBF | `GPU-Accelerated` `FEM` `ResidualStress` `CuPy` | 2023 |
| [Graph-Based Modeling for Additive Manufacturing](https://github.com/AMPL-NU/Graph_AM_Modeling) <br> *AMPL Research Group* | [GitHub](https://github.com/AMPL-NU/Graph_AM_Modeling) | *N/A* | LPBF, LDED | `GraphModels` `GNN` `ProcessModeling` | 2023 |
| [An iterative machine learning framework for predicting temperature profiles](https://arxiv.org/abs/1907.12953) <br> *Arindam Paul et al.* | [GitHub](https://github.com/NU-CUCIS/ml-iter-additive) | *N/A* | LPBF | `IterativePrediction` `BuildQuality` `XCT` | 2022 |
| [Mechanistic Data-Driven Prediction of As-Built Mechanical Properties in Metal Additive Manufacturing](https://www.nature.com/articles/s41524-021-00555-z) <br> *X. Xie et al.* (npj Computational Materials) | [GitHub](https://github.com/xiaoyuxie-vico/DL-AM) | [GitHub](https://github.com/xiaoyuxie-vico/DL_AM_Data) | DED | `ThermalHistory` `CNN` `MechanicalProperties` | 2021 |



## Physics-Informed Machine Learning 🧠

Physics-informed ML integrates fundamental physics (conservation laws, constitutive models, etc.) into data-driven models. In AM, this can mean using simulation data to train ML models, constraining neural nets with physical laws, or creating surrogate models that are faster than physics simulators but more accurate than black-box ML alone.



| Title (and Link) | Code 💻 | Dataset 📂 | Process | Tags | Year |
|------------------|---------|------------|---------|------|------|
| [A Physics-Informed CNN with Custom Loss Functions for Porosity Prediction in LMD](https://doi.org/10.3390/s22020494) <br> *Erin McGowan. et al* (Sensors) | *N/A* | [Harvard Dataverse](https://dataverse.harvard.edu/dataset.xhtml?persistentId=doi:10.7910/DVN/AHYXL9) | LMD | `CustomLoss` `CNN` `Porosity` | 2022 |
| [Differentiable Physics Simulation of Dynamics-aware Metal Powder-bed Fusion Additive Manufacturing Components](https://github.com/mojtabamozaffar/differentiable-simulation-am) <br> *M. Mozaffar et al.* | [GitHub](https://github.com/mojtabamozaffar/differentiable-simulation-am) | *N/A* | LPBF | `DifferentiableSimulation` `AutoDiff` `Optimization` | 2022 |
| [Physics-Informed Neural Networks for Multiphysics Data Assimilation with Application to AM](https://link.springer.com/article/10.1007/s00466-022-02257-9) <br> *S. Liao et al.* (Computational Mechanics) | [GitHub](https://github.com/ShuhengLiao/Physics_informed_AM) | [Drive](https://drive.google.com/file/d/1P6RqrbRW3mptzKd4LDoUrHFopBp7AfzV/view) | LDED/LPBF | `PINN` `ThermalMechanical` `DataAssimilation` | 2022 |

## AM Robotic Path Planning 🤖

Path planning is crucial for directed-energy AM processes (LDED, WAAM, etc.), especially with multi-axis robots. Efficient algorithms are needed to determine the deposition toolpath that ensures uniform material deposition, avoids collisions, and can handle complex geometries or repairs.

| Title (and Link) | Code 💻 | Dataset 📂 | Process | Tags | Year |
|------------------|---------|------------|---------|------|------|
| [RobPath: Off‑Line Path Planning Tool for LMD Automation](https://github.com/openlmd/robpath) <br> *AIMEN OpenLMD Toolkit* (Open-Source Project) | [GitHub](https://github.com/openlmd/robpath) | *N/A* | LMD | `ToolpathGeneration` `Robotics` `CAD-Based` | 2020 |
| [KUKA-ROS Based Advanced Motion Planning for Additive Manufacturing](https://www.sciencedirect.com/science/article/abs/pii/S0924013622000565) <br> *L. Chen et al.* (J. Mat. Proc. Tech.) | [GitHub](https://github.com/Davidlequnchen/KUKA-ROS-AM-Advanced-Motion-Planning) | *N/A* | LDED | `KUKA` `ROS` `MotionPlanning` | 2022 |
| [Toolpath Design for AM Using Reinforcement Learning](https://www.sciencedirect.com/science/article/pii/S2214860422000252) <br> *M. Mozaffar et al.* | [GitHub](https://github.com/mojtabamozaffar/toolpath-design-rl) | *N/A* | FDM | `ReinforcementLearning` `ToolpathOptimization` | 2022 |




## Advanced Materials 🧪

4D printing adds the dimension of time to 3D printing, enabling printed parts to change shape, properties, or function in response to external stimuli. Research in this area combines advanced materials, simulation, and AI to design transformable structures.

| Title (and Link) | Code 💻 | Dataset 📂 | Process | Tags | Year |
|------------------|---------|------------|---------|------|------|
| [AI-Assisted Material Design for 4D Printing](https://www.sciencedirect.com/science/article/pii/S2667369722000103) <br> *L. Chen et al.* | [GitHub](https://github.com/Davidlequnchen/AI-assisted-material-design-for-4D-printing) | *N/A* | 4DP | `MaterialDesign` `AI` `ShapeMemory` | 2022 |

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
