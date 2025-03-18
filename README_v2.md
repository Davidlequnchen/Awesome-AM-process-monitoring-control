
# 📚 In-Situ Monitoring and Adaptive Control in Laser-based Additive Manufacturing

Welcome to this curated repository of **research papers** on *in‑situ process monitoring* and *adaptive process control* in laser-based additive manufacturing (AM). The goal is to highlight state-of-the-art approaches for ensuring **zero-defect, autonomous AM** through real-time sensing, data analysis, and contro ([[2404.13673] In-situ process monitoring and adaptive quality enhancement in laser additive manufacturing: a critical review](https://ar5iv.org/pdf/2404.13673#:~:text=This%20paper%20provides%20a%20comprehensive,remediation%20strategies%20that%20advance%20LAM)) ([[2404.13673] In-situ process monitoring and adaptive quality enhancement in laser additive manufacturing: a critical review](https://ar5iv.org/pdf/2404.13673#:~:text=also%20discusses%20in,making))】. We focus primarily on **Laser Powder Bed Fusion (LPBF)** and **Laser Directed Energy Deposition (LDED)**, with selective inclusion of **Wire Arc AM (WAAM)** and other processes where relevant. Contributions are welcome – see the guidelines below! 😊

## Contents

- **In-Situ Process Monitoring** 🔎  
  *Techniques for real-time sensing of the AM process.* Subcategories:
  - Acoustic Signal-Based Monitoring  
  - Vision (Optical/Camera-Based) Monitoring  
  - Thermal (Infrared) Monitoring  
  - Point Cloud / Surface Topography Monitoring  
  - Multisensor Data Fusion Monitoring  
- **Adaptive Process Control** 🕹️  
  *Closed-loop control strategies to adjust process parameters on the fly.*  
- **Simulation for Process Optimization** 🖥️  
  *FEM, multi-scale modeling, and simulations to optimize AM processes.*  
- **Hybrid Additive-Subtractive Manufacturing** ⚙️  
  *Integration of printing and machining for improved accuracy and finish.*  
- **Physics-Informed Machine Learning for AM** 🧠  
  *AI/ML techniques that embed physics knowledge of AM processes.*  
- **Robotic Path Planning for AM** 🤖  
  *Tool-path planning for multi-axis AM systems (especially DED/WAAM).*  

Each paper is listed in a table with **Title (linked to paper)**, **Year**, and quick info on **Code** 💻 (open-source code availability), **Dataset** 📂 (public dataset, if any), **Process** (LPBF, LDED, WAAM, etc.), and key **Tags**. We use emojis and tags (like #OpenSource, #Dataset) to highlight community resources. 

---

## In-Situ Process Monitoring 🔎

Real-time monitoring is crucial for defect detection and quality assurance ([[2404.13673] In-situ process monitoring and adaptive quality enhancement in laser additive manufacturing: a critical review](https://ar5iv.org/pdf/2404.13673#:~:text=This%20paper%20provides%20a%20comprehensive,remediation%20strategies%20that%20advance%20LAM))4†L68-L76】. Below, we categorize monitoring approaches by the primary sensing modality:

### Acoustic Signal-Based Monitoring 📢

High-frequency acoustic emissions can reveal melt pool instabilities and defect formation. Researchers are using microphones or piezoelectric sensors to capture sound from the process and applying ML for anomaly detection.

| Title (and Link)                                                                    | Year | Code 💻            | Dataset 📂        | Process    | Tags                                   |
|-------------------------------------------------------------------------------------|------|--------------------|-------------------|-----------|----------------------------------------|
| **Optimizing In‑Situ Monitoring for LPBF: Deciphering Acoustic Emission and Sensor Sensitivity with Exp ([GitHub - vigneashpandiyan/Additive-Manufacturing-Sensor-Selection-Acoustic-Emission: Sensor selection for process monitoring based on deciphering acoustic emissions from different dynamics of the Laser Powder Bed Fusion process using Empirical Mode Decompositions and Interpretable Machine Learning](https://github.com/vigneashpandiyan/Additive-Manufacturing-Sensor-Selection-Acoustic-Emission#:~:text=Optimizing%20In,Sensitivity%20with%20Explainable%20Machine%20Learning)) ([GitHub - vigneashpandiyan/Additive-Manufacturing-Sensor-Selection-Acoustic-Emission: Sensor selection for process monitoring based on deciphering acoustic emissions from different dynamics of the Laser Powder Bed Fusion process using Empirical Mode Decompositions and Interpretable Machine Learning](https://github.com/vigneashpandiyan/Additive-Manufacturing-Sensor-Selection-Acoustic-Emission#:~:text=Machine%20Learning%20%28ML%29%20techniques,Frequency%20domain%20analysis%20revealed%20statistically))14†L250-L258】 <br> *V. Pandiyan et al.* (J. Mat. Proc. Tech.) | 2023 | [GitHub](https://github.com/vigneashpandiyan/Additive-Manufacturing-Sensor-Selection-Acoustic-Emission) | *N/A*            | LPBF      | #OpenSource #Acoustic #ExplainableML   |

### Vision-Based Monitoring 📷

Optical monitoring uses cameras (visible or infrared) to observe the melt pool, spatter, and layer morpholog ([[2404.13673] In-situ process monitoring and adaptive quality enhancement in laser additive manufacturing: a critical review](https://ar5iv.org/pdf/2404.13673#:~:text=This%20paper%20provides%20a%20comprehensive,situ%20defect%20detection.%20The%20paper))ime. High-speed imaging and computer vision techniques can detect anomalies like pores or lack-of-fusion. Some works also release open datasets for benchmarking.

| Title (and Link)                                                                    | Year | Code 💻          | Dataset 📂             | Process | Tags                                      |
|-------------------------------------------------------------------------------------|------|------------------|------------------------|---------|-------------------------------------------|
| **RAISE-LPBF: Reference Dataset & Benchmark for Reconstructing Laser Parameters from ([Reference dataset and benchmark for reconstructing laser parameters from on-axis video in powder bed fusion of bulk stainless steel](https://arxiv.org/html/2409.12475v1#:~:text=We%20present%20raise,benchmark%20to%20evaluate%20predictive%20models))eo** <br> *C. Blanc et al.* (Addit. Manuf. Lett.) | 2023 | [GitHub](https://github.com/Flanders-Make-vzw/RAISE_LPBF_Laser_benchmark) | [Website](https://www.makebench.eu)       | LPBF    | #OpenSource #Dataset #HighSpeedImaging    |
| **Dataset of In‑Situ Coaxial Monitoring and Print’s Cross-Section Images (DED)** <br> *J. Akhavan et al.* (Sci. Data)                                            | 2023 | *N/A*           | [Data](https://doi.org/10.1038/s41597-023-02672-4) | LDED    | #OpenAccess #Dataset #CoaxialVision       |
| **Real-Time Monitoring & Quality Assurance for L-DED via Coaxial Imaging + Self ([Real-time monitoring and quality assurance for laser-based directed energy deposition: integrating co-axial imaging and self-supervised deep learning framework | Journal of Intelligent Manufacturing
        ](https://link.springer.com/article/10.1007/s10845-023-02279-x#:~:text=monitoring%20of%20the%20quality%20of,sampled%20representations%20of%20process%20zone)) ([Real-time monitoring and quality assurance for laser-based directed energy deposition: integrating co-axial imaging and self-supervised deep learning framework | Journal of Intelligent Manufacturing
        ](https://link.springer.com/article/10.1007/s10845-023-02279-x#:~:text=monitoring,ensuring%20part%20quality%20during%20fabrication))L73】 <br> *V. Pandiyan et al.* (J. Intell. Manuf.) | 2023 | [GitHub](https://github.com/vigneashpandiyan/Additive-Manufacturing-Self-Supervised-Learning-Coaxial-DED-Process-Zone-Imaging) | *Available on request* | LDED    | #OpenSource #Vision #SelfSupervised      |

### Thermal/Infrared Monitoring 🌡️

Infrared cameras and pyrometers capture thermal signatures (melt pool temperature, cooling rates, etc.) for  ([](http://arxiv.org/pdf/2407.12682#:~:text=introduce%20several%20new%20IR%20features,parts%20are%20printed%2C%20monitored%2C%20and)) ([](http://arxiv.org/pdf/2407.12682#:~:text=characterized%20to%20provide%20evidence%20of,situ%20monitoring))-L30】. Thermal monitoring can reveal anomalies like overheating, lack of fusion, or excessive cooling that correlate with defects.

| Title (and Link)                                                                    | Year | Code 💻          | Dataset 📂  | Process | Tags                                |
|-------------------------------------------------------------------------------------|------|------------------|------------|---------|-------------------------------------|
| **In‑Situ Infrared Camera Monitoring for Defect & Anomaly  ([](http://arxiv.org/pdf/2407.12682#:~:text=introduce%20several%20new%20IR%20features,parts%20are%20printed%2C%20monitored%2C%20and)) ([](http://arxiv.org/pdf/2407.12682#:~:text=instabilities%2C%20spattering%2C%20temperature%20increase%2C%20and,of%20this%20work%20is%20to))21-L30】 <br> *S. Hinnebusch et al.* (arXiv preprint) | 2024 | *Python snippets* | *N/A*     | LPBF    | #OpenAccess #Thermal #FeatureExtraction |

### Surface Topography / Point Cloud Monitoring 🛰️

Structured-light scanning, fringe projection, and 3D reconstruction techniques monitor the geometry of each layer. These produce **point clouds** or height maps to detect warping, recoater interference, or surface roughness issues.

| Title (and Link)                                                                    | Year | Code 💻       | Dataset 📂 | Process | Tags                                   |
|-------------------------------------------------------------------------------------|------|---------------|-----------|---------|----------------------------------------|
| **In‑Situ Surface Topography of LPBF Usi ([[PDF] In-situ fringe projection profilometry and spatter monitoring ... - euspen](http://www.euspen.eu/knowledge-base/AM23134.pdf#:~:text=euspen%20www.euspen.eu%20%20Davies%2C%20,107%2C%202016%2C%20doi%3A%2010.1016%2Fj))ojection** <br> *B. Zhang et al.* (Addit. Manuf.)                                             | 2016 | *N/A*        | *N/A*     | LPBF    | #FringeProjection #SurfaceMonitoring   |
| **Etna: On-line 3D Monitoring for Robotized LMD** <br> *AIMEN OpenLMD Toolkit* (Open-Source Project)                                                          | 2017 | [GitHub](https://github.com/openlmd/etna) | *N/A*     | LMD     | #OpenSource #3DScan #LMD               |

### Multisensor & Data Fusion 🧩

Combining multiple sensors (e.g., optical, acoustic, thermal) can provide a richer ([[2404.13673] In-situ process monitoring and adaptive quality enhancement in laser additive manufacturing: a critical review](https://ar5iv.org/pdf/2404.13673#:~:text=defects%20within%20Laser%20Powder%20Bed,situ%20defect%20detection.%20The%20paper)) the process. Multisensor approaches often leverage machine learning to fuse data and detect defects more reliably, sometimes using ground truth from X-ray or CT for validation.

| Title (and Link)                                                                    | Year | Code 💻         | Dataset 📂              | Process | Tags                                    |
|-------------------------------------------------------------------------------------|------|-----------------|-------------------------|---------|-----------------------------------------|
| **Deep Learning Monitoring of LPBF with Heterogeneous S ([Deep learning-based monitoring of laser powder bed fusion process on variable time-scales using heterogeneous sensing and operando X-ray radiography guidance](https://infoscience.epfl.ch/entities/publication/2ce72bb3-eeca-4099-9325-ce061bfa2e55#:~:text=,signals%20of%20fixed%20length%20in)) ([Deep learning-based monitoring of laser powder bed fusion process on variable time-scales using heterogeneous sensing and operando X-ray radiography guidance](https://infoscience.epfl.ch/entities/publication/2ce72bb3-eeca-4099-9325-ce061bfa2e55#:~:text=this%20work%2C%20we%20try%20to,cubes%20out%20of%20austenitic%20Stainless))* <br> *V. Pandiyan et al.* (Addit. Manuf.)                 | 2022 | [GitHub](https://github.com/vigneashpandiyan/Additive-Manufacturing-Variable-Time-Scales) | [Zenodo](https://doi.org/10.5281/zenodo.6339430) | LPBF    | #OpenSource #Multisensor #XRay           |

## Adaptive Process Control 🕹️

Adaptive control closes the loop by adjusting process parameters in real tim ([[2404.13673] In-situ process monitoring and adaptive quality enhancement in laser additive manufacturing: a critical review](https://ar5iv.org/pdf/2404.13673#:~:text=also%20discusses%20in,making)) sensor feedback. The aim is to correct defects on-the-fly – for example, modulating laser power or scan speed to maintain a stable melt pool and avoid flaws, driving AM t ([[2404.13673] In-situ process monitoring and adaptive quality enhancement in laser additive manufacturing: a critical review](https://ar5iv.org/pdf/2404.13673#:~:text=also%20discusses%20in,making))nomous operation.

| Title (and Link)                                                                    | Year | Code 💻       | Dataset 📂 | Process | Tags                               |
|-------------------------------------------------------------------------------------|------|---------------|-----------|---------|------------------------------------|
| **CladPlus: Closed-Loop  ([OpenLMD by AIMEN Technology Center](https://openlmd.github.io/cladplus.html#:~:text=This%20closed,from%201um%20to%205%20um)) ([OpenLMD by AIMEN Technology Center](https://openlmd.github.io/cladplus.html#:~:text=OpenLMD%20enables%20closed,of%20laser%20cladding))ng** <br> *AIMEN OpenLMD Toolkit* (Open-Source Project) | 2017 | [GitHub](https://github.com/openlmd/cladplus) | *N/A*     | LDED    | #OpenSource #ClosedLoop #LaserCladding |

*Examples:* In **CladPlus**, an infrared camera measures melt pool size and a controller adjusts laser power in real-tim ([OpenLMD by AIMEN Technology Center](https://openlmd.github.io/cladplus.html#:~:text=This%20closed,from%201um%20to%205%20um)) ([OpenLMD by AIMEN Technology Center](https://openlmd.github.io/cladplus.html#:~:text=OpenLMD%20enables%20closed,of%20laser%20cladding))pool. Emerging research also explores layerwise **iterative learning control** and even reinforcement learning to refine process parameters each layer, aiming for consistent part quality.

## Simulation for Process Optimization 🖥️

Physics-based simulations (thermal, mechanical, microstructural) help predict outcomes of process parameters and optimize them without costly trial-and-error. Open-source tools and multi-physics models are enabling **“digital twins”** of AM processes.

| Title (and Link)                                                                    | Year | Code 💻       | Dataset 📂 | Process        | Tags                                       |
|-------------------------------------------------------------------------------------|------|---------------|-----------|----------------|--------------------------------------------|
| **JAX-AM: Differentiable Simulation Toolb ([GitHub - tianjuxue/jax-am: Additive manufacturing simulation with JAX.](https://github.com/tianjuxue/jax-am#:~:text=A%20GPU,AM%29%20based%20on%20JAX)) ([GitHub - tianjuxue/jax-am: Additive manufacturing simulation with JAX.](https://github.com/tianjuxue/jax-am#:~:text=JAX,Property%20relationship%20in%20AM))g** <br> *T. Xue et al.* (Open-Source Project)            | 2023 | [GitHub](https://github.com/tianjuxue/jax-am) | *N/A*     | *Multi (LPBF/DED)* | #OpenSource #Simulation #Differentiable    |

*Notes:* **JAX-AM** is a GPU-accelerated simulation suite covering powder dynamics, fluid flow, thermal FEM, and phase-field mo ([GitHub - tianjuxue/jax-am: Additive manufacturing simulation with JAX.](https://github.com/tianjuxue/jax-am#:~:text=Image%3A%20Doc%20Image%3A%20PyPI%20Image%3A,Image%3A%20Github%20Fork%20Image%3A%20License))ilt in Python JAX. It enables fast experimentation and even AI integration (e.g. automatic differentiation for optimization). Such tools are pushing the envelope in process modeling and **inverse design** (finding optimal parameters for target outcomes).

## Hybrid Additive-Subtractive Manufacturing ⚙️

Hybrid processes combine **additive** (build-up) and **subtractive** (machining) s ([Hybrid additive and subtractive manufacturing - ScienceDirect.com](https://www.sciencedirect.com/science/article/pii/S2212827123003542#:~:text=ScienceDirect,limitations%20of%20both%20types))e workflow or machine. This addresses limitations of AM (e.g., surface finish, accuracy) by machining critical surfaces or features either intermittently during the build or post-build. Research in this area includes machine tool integration and strategic toolpath planning for when to print vs. mill.

| Title (and Link)                                                                    | Year | Code 💻 | Dataset 📂 | Process      | Tags                                |
|-------------------------------------------------------------------------------------|------|---------|-----------|--------------|-------------------------------------|
| **Hybrid Additive-Subtractive Manufacturing Using Pulsed Arc Plasma** <br> *X. Duan et al.* (Materials) | 2023 | *N/A*   | *N/A*     | PAP (Arc DED) | #OpenAccess #HybridManufacturing    |

*Example:* The above study demonstrates a hybrid setup where a **pulsed arc plasma** deposition is alternated with milling to achieve better precision. On the commercial side, machine tools that incorporate a laser or wire DED head alongside CNC milling heads are increasingly used. Research challenges include registration of the part between processes and optimizing **build-mill sequences**.

## Physics-Informed Machine Learning 🧠

Physics-informed ML integrates fundamental physics (conservation laws, constitutive models, etc.) into data-driven models. In AM, this can mean using simulation data to train ML models, constraining neural nets with physical laws, or creating surrogate models that are faster than physics simulators but mor ([GitHub - tianjuxue/jax-am: Additive manufacturing simulation with JAX.](https://github.com/tianjuxue/jax-am#:~:text=%40article%7Bxue2022physics%2C%20title%3D%7BPhysics,2022))n black-box ML alone.

| Title (and Link)                                                                    | Year | Code 💻 | Dataset 📂 | Process    | Tags                                       |
|-------------------------------------------------------------------------------------|------|---------|-----------|------------|--------------------------------------------|
| **Physics-Embedded Graph Network for Acce ([GitHub - tianjuxue/jax-am: Additive manufacturing simulation with JAX.](https://github.com/tianjuxue/jax-am#:~:text=%40article%7Bxue2022physics%2C%20title%3D%7BPhysics,2022))structure Simulation** <br> *T. Xue et al.* (NPJ Comput. Mater.) | 2022 | [GitHub](https://github.com/tianjuxue/jax-am) | *Synthetic* | LPBF (Ti64) | #OpenAccess #PhysicsInformed #Microstructure |

*Insight:* Xue et al. train a graph neural network to mimic a **phase-field** microstructure simulation, dramatically speeding up predictions of grain growth in LPB ([GitHub - tianjuxue/jax-am: Additive manufacturing simulation with JAX.](https://github.com/tianjuxue/jax-am#:~:text=%40article%7Bxue2022physics%2C%20title%3D%7BPhysics,2022))ting physical dynamics. Other work in this realm includes physics-informed neur ([Physics-Informed Machine Learning for Smart Additive Manufacturing](https://arxiv.org/abs/2407.10761#:~:text=Manufacturing%20arxiv,neural%20networks%20and%20physical%20laws))r thermal field prediction and defect propagation modeling, as well as Bayesian approaches that update physics models with in-situ sensor data. By fusing physics and ML, these approaches aim for models that require less training data and offer better extrapolation to new conditions.

## AM Robotic Path Planning 🤖

Path planning is crucial for directed-energy AM processes (LDED, WAAM, etc.), especially with multi-axis robots. Efficient algorithms are needed to determine the deposition toolpath that ensures uniform material deposition, avoids collisions, and can handle complex geometries or repairs.

| Title (and Link)                                                                    | Year | Code 💻       | Dataset 📂 | Process | Tags                           |
|-------------------------------------------------------------------------------------|------|---------------|-----------|---------|--------------------------------|
| **RobPath: Off‑Line Path Planning Tool for LMD Automation** <br> *AIMEN OpenLMD Toolkit* (Open-Source Project) | 2020 | [GitHub](https://github.com/openlmd/robpath) | *N/A*     | LMD     | #OpenSource #PathPlanning #LMD |

*Example:* **RobPath** provides a simple off-line planner for robotic LMD, allowing users to generate deposition toolpaths from a CAD model. In research, advanced planners consider multi-axis orientations to minimize support structures, or adaptive path planning to repair worn parts (e.g., vision-guided path correction in the PROPER project). Continued development in this area helps AM move beyond planar layers to true free-form 3D printing. 

---

## 🤝 Contributing

We welcome contributions from the community! Please feel free to **suggest a paper** or **add a new entry** via Pull Request. To maintain consistency, please follow these guidelines:

- **Scope**: Ensure the paper is relevant to *in-situ monitoring or adaptive control* in AM (or closely related, like simulation or hybrid processes). Laser-based metal AM is the focus, but notable work in other AM or sensing modalities can be included if it fits a category.
- **Table Format**: Use the same table structure: Title (with link to paper), Year, Code (link if available), Dataset (link if available), Process type, and Tags. Indicate *N/A* if code or data are not available. 
- **Tags**: Use brief tags prefixed with `#`. Examples: `#OpenSource` (if code available), `#Dataset` (open data), `#Vision`, `#Acoustic`, `#ML`, `#HybridManufacturing`, etc. Aim for 2-4 tags that capture the work’s key aspects.
- **Style**: Keep descriptions concise. You can add a short note below a table if needed to explain context or significance (as done above). Use present tense and clear language.
- **Attribution**: Include the first author’s last name or an obvious short reference in the Title field for clarity. If the paper is open access, you can note that in tags or the title (e.g., via journal or a 🔓 emoji).

By contributing, you agree to abide by the repo’s [Code of Conduct](CODE_OF_CONDUCT.md) and ensure information is accurate. Let's build a comprehensive knowledge base for the AM community! 🤖🔥

## 📜 License

All content in this repository is released under the [MIT License](LICENSE), and the respective papers are copyright their publishers/authors. This list is for educational and research purposes, inspired by open-source community efforts.

<hr>

*Happy Printing & Processing!* 🚀 Feel free to open an issue for any questions or discussions.

