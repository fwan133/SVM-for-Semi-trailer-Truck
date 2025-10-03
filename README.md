# Multi-Camera Surround View Monitoring (SVM) System for Semi-Trailer Trucks

A research project implementing a **multi-camera SVM framework** for semi-trailer trucks to support safe maneuvering of oversized goods in constrained urban environments.

This repository complements the paper:  
> *Title: Multi-Camera Surround View Monitoring for Semi-Trailer Trucks*  
> *(Currently under review)*

---

## 🚚 Project Overview
This project focuses on developing a **systematic and theoretically feasible framework** for SVM systems on semi-trailer trucks. The goal is to improve situational awareness and support safe operations such as transporting Modular Integrated Construction (MiC) modules in urban environments.

The framework includes:
- **Camera Placement Optimization (CPO):** Determines the optimal number and positions of fisheye cameras to maximize BEV image fidelity while minimizing hardware cost.
- **Spatial–Temporal Fusion Articulation-Angle Estimation (AAE):** A camera-only method that robustly estimates the articulation angle between the tractor and trailer, even under occlusions or disturbances.
- **Dynamic Image Concatenation (DIC):** Produces seamless BEV images by selecting the optimal image source for each pixel rather than relying on traditional seam-based stitching.

---

## ✨ Key Features
- 📷 **Optimized camera placement** for high coverage and clear BEV images.
- 🔗 **Robust articulation angle estimation** using spatial–temporal fusion and Kalman filtering.
- 🖼️ **High-fidelity BEV image generation** with reduced distortion for near-field 3D objects.
- ⚙️ Designed for **scalability** to various semi-trailer configurations.

---

## 🖥️ Simulation Platform
- **Operating System:** Ubuntu 20.04.6 LTS
- **CPU:** Intel® Core™ i9‑14900K ×32
- **GPU:** NVIDIA RTX 4090D
- **Memory:** 94 GB
- **Simulation Frame Rate:** 10 FPS (due to rendering constraints of the simulation environment)

---

## 📊 Evaluation
The evaluation focuses on:
- Accuracy of **articulation angle estimation**
- Overall **BEV image quality**
- **Computational efficiency** of the BEV pipeline

### Real-Time Performance
- Articulation angle estimation: **57.82 ms / frame**
- BEV image generation: **7.94 ms / frame**
- Achieved up to **17.3 FPS** in simulation

> Future work aims to integrate GPU acceleration and real-world testing to further enhance performance.

---

## 📈 Future Work
- Develop **fiducial‑marker‑based calibration** for real-world camera extrinsics.
- Integrate **roll and pitch modeling** to improve BEV accuracy on uneven terrain.
- Incorporate **height and depth estimation** (e.g., via stereo vision or LiDAR fusion).
- Extend functionalities for **3D object detection, obstacle warnings, and trajectory prediction**.

---

## 📂 Repository Structure
```
├── docs/                  # Documentation and related manuscripts
├── src/                   # Core source code for CPO, AAE, and DIC
├── data/                  # Sample data and simulation settings
├── results/               # Experimental results and visualizations
└── README.md              # Project overview (this file)
```

---

## 📜 Citation
If you use this project in your research, please cite the paper (link will be provided after publication).

---

## 📧 Contact
For questions or collaborations, please contact:
- **Lead Author:** [Your Name]  
- **Email:** [your.email@example.com]  
- **GitHub:** [Your GitHub Profile]

---

> ⚠️ **Note:** This repository currently focuses on the **simulation-based framework**. Real-world implementation with hardware calibration and on-road testing is in progress and will be released in future updates.
