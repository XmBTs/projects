# 🎓 Graduate Research Projects

This repository presents the main projects I conducted during my graduate studies, focusing on **multi-robot SLAM** and **autonomous navigation**. [下载并查看项目说明书 (PDF)](./report.pdf)

---

## 🚀 Project 1: Multi-Robot Cooperative SLAM and Autonomous Exploration

[![ROS](https://img.shields.io/badge/ROS-noetic-green.svg)]()  
[![License](https://img.shields.io/badge/license-MIT-blue.svg)]()  

### 🌍 Overview
A bandwidth-efficient **multi-robot cooperative SLAM system** for large-scale exploration.  
Robots exchange **2.5D submaps** under bandwidth-limited communication and achieve global consistency via a **sliding window optimizer**.  

**Key Features:**
- 📡 Low-bandwidth 2.5D submap communication  
- 🧭 Sliding window optimization for global consistency  
- 🤝 Collaborative mapping in distributed environments  

### 📊 Results
- Reduced communication by **>30%** compared with 3D submaps  
- Achieved robust mapping in real-world multi-robot experiments  
<p align="center">
  <img src="muilt_map.png" width="600">
</p>

## 🤖 Project 2: Autonomous UAV Inspection System for Bridge Monitoring
**Duration:** Aug. 2024 – Nov. 2024  
**Role:** Independent Developer  

### 🌍 Overview
This project implements an **autonomous UAV inspection system** designed for bridge monitoring tasks. The system enables a single drone to perform fully autonomous takeoff, multi-waypoint navigation, and precise localization along the bridge.  

### 🛠 Platform
- UAV equipped with **RTK, Livox Mid360 LiDAR, and Realsense D435**  
- Onboard processor: **Intel NUC**  
- Operating system: **Ubuntu 20.04**  

### 📌 Key Features

1. **Bridge Modeling:**  
   - Real-time **RTK + LIO** for initial localization  
   - Construct a matched-frame database and save high-precision bridge point cloud models  

2. **Relocalization:**  
   - Extract keyframe point cloud descriptors and match them with the database  
   - Use **iSAM** for factor graph optimization to obtain accurate UAV poses  

3. **Multi-Waypoint Navigation:**  
   - Developed a **multi-waypoint selection plugin in Rviz**  
   - Designed a **global planner** to select navigation points online based on the bridge model  

### 📊 Results
- UAV successfully performed **autonomous takeoff and multi-point navigation**  
- Relocalization error: **< 0.1 m**  
- Mission success rate: **> 95%**  

<!--## 🤖 Project 2: Autonomous Drone-Based System for Bridge Inspection Missions

### 🌍 Overview
An **Autonomous Drone-Based System for Bridge Inspection Missions** designed for service robots operating in dynamic environments.
The system integrates multi-sensor data and provides robust localization, mapping, and obstacle avoidance.

**Key Features:**
- 🔎 Real-time **RTK + LIO** for initial localization and construct a matched-frame database and save high-precision bridge point cloud models
- 🚧 Real-time obstacle detection & avoidance
- 🛠 ROS-based modular implementation

### 📊 Results
- Successfully deployed in a university building for long-term navigation tests
- Demonstrated reliable performance in dynamic human-populated environments -->

<p align="center">
  <img src="Bridge_inspection.png" width="600">
</p>

### 🎥 Demo Video
- The demos for all the projects introduced above can be viewed by scanning the QR code below.
![Demo](videos_show.png)
