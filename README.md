# 📚 In-Situ Monitoring and Adaptive Control in Laser-based Additive Manufacturing

Welcome to this curated repository of **research papers** on *in‑situ process monitoring* and *adaptive process control* in laser-based additive manufacturing (AM). The goal is to highlight state-of-the-art approaches for ensuring **zero-defect, autonomous AM** through real-time sensing, data analysis, and control. We focus primarily on **Laser Powder Bed Fusion (LPBF)** and **Laser Directed Energy Deposition (LDED)**, with selective inclusion of **Wire Arc AM (WAAM)** and other processes where relevant. Contributions are welcome – see the guidelines below! 😊

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

### Vision-Based Monitoring 📷

Optical monitoring uses cameras (visible or infrared) to observe the melt pool, spatter, and layer morphology in real-time. High-speed imaging and computer vision techniques can detect anomalies like pores or lack-of-fusion. Some works also release open datasets for benchmarking.

| Title (and Link) | Code 💻 | Dataset 📂 | Process | Tags | Year |
|------------------|---------|------------|---------|------|------|
| [RAISE-LPBF: Reference Dataset & Benchmark for Reconstructing Laser Parameters from On-Axis Video](https://arxiv.org/html/2409.12475v1) <br> *C. Blanc et al.* (Addit. Manuf. Lett.) | [GitHub](https://github.com/Flanders-Make-vzw/RAISE_LPBF_Laser_benchmark) | [Website](https://www.makebench.eu) | LPBF | `HighSpeedImaging` `LaserParameters` `Benchmark` | 2023 |
| [Dataset of In‑Situ Coaxial Monitoring and Print's Cross-Section Images](https://doi.org/10.1038/s41597-023-02672-4) <br> *J. Akhavan et al.* (Sci. Data) | *N/A* | [Data](https://doi.org/10.1038/s41597-023-02672-4) | LDED | `CoaxialVision` `CrossSection` `OpenAccess` | 2023 |
| [Real-Time Monitoring & Quality Assurance for L-DED via Coaxial Imaging + Self-Supervised Learning](https://link.springer.com/article/10.1007/s10845-023-02279-x) <br> *V. Pandiyan et al.* (J. Intell. Manuf.) | [GitHub](https://github.com/vigneashpandiyan/Additive-Manufacturing-Self-Supervised-Learning-Coaxial-DED-Process-Zone-Imaging) | *Available on request* | LDED | `SelfSupervised` `CoaxialImaging` `QualityAssurance` | 2023 |
| [Deep DIC: Deep Learning-Based Digital Image Correlation for End-to-End Displacement and Strain Measurement](https://www.sciencedirect.com/science/article/abs/pii/S0924013621004349) <br> *R. Yang et al.* (J. Mat. Proc. Tech.) | [GitHub](https://github.com/RuYangNU/Deep-Dic-deep-learning-based-digital-image-correlation) | [Drive](https://drive.google.com/drive/folders/1n2axHsJ3flHxk_edceY6eOfiX7GjW_d6) | Various | `DIC` `DeepLearning` `StrainMeasurement` | 2022 |

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

## Adaptive Process Control 🕹️

Adaptive control closes the loop by adjusting process parameters in real-time based on sensor feedback. The aim is to correct defects on-the-fly – for example, modulating laser power or scan speed to maintain a stable melt pool and avoid flaws, driving AM toward autonomous operation.

| Title (and Link) | Code 💻 | Dataset 📂 | Process | Tags | Year |
|------------------|---------|------------|---------|------|------|
| [CladPlus: Closed-Loop Control for Laser Cladding](https://openlmd.github.io/cladplus.html) <br> *AIMEN OpenLMD Toolkit* (Open-Source Project) | [GitHub](https://github.com/openlmd/cladplus) | *N/A* | LDED | `ClosedLoop` `LaserCladding` `InfraredControl` | 2017 |


## Simulation for Process Optimization 🖥️

Physics-based simulations (thermal, mechanical, microstructural) help predict outcomes of process parameters and optimize them without costly trial-and-error. Open-source tools and multi-physics models are enabling **"digital twins"** of AM processes.

| Title (and Link) | Code 💻 | Dataset 📂 | Process | Tags | Year |
|------------------|---------|------------|---------|------|------|
| [JAX-AM: Differentiable Simulation Toolkit for Additive Manufacturing](https://github.com/tianjuxue/jax-am) <br> *T. Xue et al.* (Open-Source Project) | [GitHub](https://github.com/tianjuxue/jax-am) | *N/A* | *Multi (LPBF/DED)* | `Differentiable` `GPU-Accelerated` `JAX` | 2023 |



## Hybrid Additive-Subtractive Manufacturing ⚙️

Hybrid processes combine **additive** (build-up) and **subtractive** (machining) steps in the same workflow or machine. This addresses limitations of AM (e.g., surface finish, accuracy) by machining critical surfaces or features either intermittently during the build or post-build. Research in this area includes machine tool integration and strategic toolpath planning for when to print vs. mill.

| Title (and Link) | Code 💻 | Dataset 📂 | Process | Tags | Year |
|------------------|---------|------------|---------|------|------|
| [Hybrid Additive-Subtractive Manufacturing Using Pulsed Arc Plasma](https://www.mdpi.com/1996-1944/16/13/4809) <br> *X. Duan et al.* (Materials) | *N/A* | *N/A* | PAP (Arc DED) | `HybridManufacturing` `PulsedArc` `Milling` | 2023 |



## Physics-Informed Machine Learning 🧠

Physics-informed ML integrates fundamental physics (conservation laws, constitutive models, etc.) into data-driven models. In AM, this can mean using simulation data to train ML models, constraining neural nets with physical laws, or creating surrogate models that are faster than physics simulators but more accurate than black-box ML alone.

| Title (and Link) | Code 💻 | Dataset 📂 | Process | Tags | Year |
|------------------|---------|------------|---------|------|------|
| [Physics-Embedded Graph Network for Accelerating Metal Microstructure Simulation](https://github.com/tianjuxue/jax-am) <br> *T. Xue et al.* (NPJ Comput. Mater.) | [GitHub](https://github.com/tianjuxue/jax-am) | *Synthetic* | LPBF (Ti64) | `GraphNetwork` `PhaseField` `Microstructure` | 2022 |
| [A Physics-Informed CNN with Custom Loss Functions for Porosity Prediction in LMD](https://doi.org/10.3390/s22020494) <br> *P. Hagqvist et al.* (Sensors) | *N/A* | [Harvard Dataverse](https://dataverse.harvard.edu/dataset.xhtml?persistentId=doi:10.7910/DVN/AHYXL9) | LMD | `CustomLoss` `CNN` `Porosity` | 2022 |
| [Generic Physics-Based ML Model for Geometry-Invariant Thermal History Prediction in AM](https://www.sciencedirect.com/science/article/pii/S0924013621004325) <br> *K. Nygård et al.* (J. Mat. Proc. Tech.) | [GitHub](https://github.com/kariln/Predictions-of-thermal-fields-in-additive-manufacturing) | [Dataset](https://cutt.ly/QnqXV9Z) | Various | `GeometryInvariant` `ThermalHistory` `FEM` | 2022 |
| [Physics-Driven Deep Learning Model for Process-Porosity Causal Relationship in LMD](https://www.sciencedirect.com/science/article/pii/S0007850620300718) <br> *X. Xie et al.* (CIRP Annals) | *N/A* | [Harvard Dataverse](https://dataverse.harvard.edu/dataset.xhtml?persistentId=doi:10.7910/DVN/AHYXL9) | LMD | `Interpretability` `Causality` `Porosity` | 2021 |
| [ML for Metal AM: Predicting Temperature and Melt Pool Dynamics using Physics-Informed Neural Networks](https://www.sciencedirect.com/science/article/pii/S0924013621004325) <br> *Y. Yang et al.* (Computational Mechanics) | [Website](https://yan.cee.illinois.edu/) | ✅ | Various | `PINN` `MultiphaseFlow` `ThermalModeling` | 2021 |



## AM Robotic Path Planning 🤖

Path planning is crucial for directed-energy AM processes (LDED, WAAM, etc.), especially with multi-axis robots. Efficient algorithms are needed to determine the deposition toolpath that ensures uniform material deposition, avoids collisions, and can handle complex geometries or repairs.

| Title (and Link) | Code 💻 | Dataset 📂 | Process | Tags | Year |
|------------------|---------|------------|---------|------|------|
| [RobPath: Off‑Line Path Planning Tool for LMD Automation](https://github.com/openlmd/robpath) <br> *AIMEN OpenLMD Toolkit* (Open-Source Project) | [GitHub](https://github.com/openlmd/robpath) | *N/A* | LMD | `ToolpathGeneration` `Robotics` `CAD-Based` | 2020 |


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
