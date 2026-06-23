# LiDAR Mapping, Localization and Change Detection using KISS-SLAM

![Map Registration](results/Map_Registration.png)

## Project Overview

Accurate localization and environmental understanding are fundamental requirements for autonomous driving systems, mobile robotics, digital twins, and large-scale geospatial mapping. This project investigates a complete LiDAR-based mapping and localization workflow using KISS-SLAM and point cloud registration techniques.

The project focuses on generating a reference 3D map from LiDAR measurements, localizing newly acquired scans within the reference environment, and detecting structural changes between temporally separated point cloud datasets. The work was conducted as part of the M.Sc. Geoinformatics Project Seminar at Leibniz University Hannover.

---

## Problem Statement

Autonomous systems continuously operate in dynamic environments where infrastructure, vegetation, vehicles, and urban structures may change over time. Reliable localization requires aligning newly acquired LiDAR scans with an existing reference map while maintaining robustness against sensor noise, partial overlap, and environmental changes.

This project addresses three key challenges:

* Large-scale LiDAR mapping
* Accurate localization through point cloud registration
* Detection of environmental changes between acquisition epochs

---

## Technical Workflow

### 1. LiDAR Mapping

A reference 3D environment was generated using KISS-SLAM from sequential LiDAR measurements. The resulting map serves as a global reference for localization and registration tasks.

### 2. Point Cloud Preprocessing

Point clouds were filtered and prepared for geometric registration. Data quality assessment and preprocessing were performed to improve registration stability.

### 3. Map Registration

Reference and query maps were aligned using iterative geometric registration techniques. The registration pipeline estimates the transformation required to localize the query map within the global reference frame.

### 4. Localization

Localization was achieved through transformation estimation and map alignment, allowing the query map to be accurately positioned within the reference environment.

### 5. Change Detection

Following registration, the aligned point clouds were compared to identify structural differences between acquisition periods and detect environmental changes.

---

## Key Contributions

* Generated large-scale 3D maps using KISS-SLAM
* Developed a complete point cloud registration workflow
* Implemented map localization using geometric alignment techniques
* Investigated ICP-based registration strategies
* Performed temporal change detection on LiDAR point clouds
* Evaluated registration quality and localization performance
* Visualized and analyzed registration results using Open3D

---

## Technologies and Libraries

* Python
* Open3D
* NumPy
* KISS-SLAM
* ICP Registration
* Point Cloud Processing
* LiDAR Mapping
* Spatial Analysis
* 3D Data Processing

---

## Results

The registration pipeline successfully aligned independently acquired LiDAR maps and enabled subsequent change detection analysis. Experimental evaluation demonstrated the effectiveness of geometric registration techniques for localization and environmental monitoring applications.

The repository contains detailed visualizations, implementation notebooks, technical documentation, and project reports.

---

## Applications

* Autonomous Driving
* Mobile Robotics
* Simultaneous Localization and Mapping (SLAM)
* Digital Twin Generation
* Infrastructure Monitoring
* Environmental Change Detection
* Geospatial Intelligence

---

## Repository Structure

```text
code/
├── map_registration/
└── change_detection/

docs/
├── Project Report
└── Registration Documentation

presentations/
└── Seminar Presentation

results/
└── Registration and Change Detection Results
```

---

## Author

**Muhammad Jawad**

M.Sc. Geoinformatics

Leibniz University Hannover

Research Interests:

* Machine Learning
* Computer Vision
* LiDAR Perception
* SLAM
* Autonomous Driving
* State Estimation
* Vision-Language Models
